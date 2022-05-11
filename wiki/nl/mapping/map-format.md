---
sidebar: auto
prev: ./intermediate-mapping.md
next: false
description: Neem een diepe duik in het formaat van een Beat Saber level.
---

# Level formaat
Er zijn enkele gevallen waar de beschikbare programma's en level editors niet elke functionaliteit bieden die je wilt. Je voelt je misschien ook geïnspireerd om een programma of level editor te maken gewoon voor de lol.

Klein probleempje dus. Wat *precies* gaat er in een level bestand? Dit is belangrijk om te begrijpen bij het ontwikkelen van nieuwe programma's, scripts en editors.

Deze pagina helpt je om de interne werking van een volledig Beat Saber level te begrijpen en informatie te verkrijgen over wat elk eigenschap en waarde betekend.

## Schemas
Een *schema* is eigenlijk een set van regels voor een specifiek soort bestand. Ze hebben een lijst met regels die je *mag* breken, en regels die je *niet* mag breken.

Beat Saber bevat zijn eigen schema; het definieert wat het formaat van een Beat Saber level moet zijn en dat is wat we hier gaan uitleggen.

### BeatSaver schema
De leden van de community zijn echter samen gekomen en hebben hun eigen schema gemaakt, wat regels die door Beat Saber's eigen schema zijn vastgesteld forceert, maar ook *nieuwe* regels maakt en stelt om te volgen.

Dit door de community gemaakte schema wordt gebruikt door BeatSaver, die [je hier kunt vinden](https://github.com/lolPants/beatmap-schemas). Bij het uploaden van je level naar BeatSaver, controleert het met deze schemabestanden om te bepalen of het geschikt is om te uploaden. Een belangrijke verandering in dit schema is de opname van `_customData` objecten verspreid over level bestanden, die hier worden uitgelegd.

Je kunt door het BeatSaver Schema lezen om een beter inzicht te krijgen in wat er in een Beat Saber level hoort, en zorg ervoor dat je eigen programma de juiste levels uitvoert die kunnen worden geüpload naar BeatSaver.

## `Info.dat`
`Info.dat` is het belangrijkste bestand voor een Beat Saber level. Het beschrijft de basis metadata van jouw level, het verwijst ook naar de bestanden die gebruikt worden voor de niveaus, omslagfoto en audio.

:::warning
Het is uiterst belangrijk dat je dit correct doet, anders zal het level niet laden in Beat Saber.
:::

### Base Object
Hier is het basisformaat voor een `Info.dat` bestand. Merk op dat de difficulty beatmap sets weg zijn gelaten, deze worden later op de pagina uitgelegd.

```json
{
    "_version": "2.0.0",
    "_songName": "Voorbeeld Nummer",
    "_songSubName": "",
    "_songAuthorName": "Nummer Atiest",
    "_levelAuthorName": "Jij",
    "_beatsPerMinute": 120,
    "_shuffle": 0,
    "_shufflePeriod": 0.5,
    "_previewStartTime": 31.5,
    "_previewDuration": 7,
    "_songFilename": "song.ogg",
    "_coverImageFilename": "cover.jpg",
    "_environmentName": "BigMirrorEnvironment",
    "_allDirectionsEnvironmentName" : "GlassDesertEnvironment",
    "_songTimeOffset": 0,
    "_customData": {
        // Elke custom data komt hier.
    // Als dit leeg is, moet dit volledig worden verwijderd.
  },
    "_difficultyBeatmapSets": [
        // Difficulty beatmap sets (en difficulty beatmaps) worden later op de pagina uitgelegd.
    // Check de zijbalk!
  ]
}
```

#### _version
Dit veld beschrijft de versie van het level-formaat dat we gebruiken. Currently, Beat Saber's map info format is on version `2.0.0`.

#### _songName
Dit veld beschrijft de naam van jouw nummer.

#### _songSubName
Dit veld beschrijft alle extra titels die in jouw nummer zouden kunnen komen. Deze kunnen bestaan uit het volgende:

* Extra artiesten (zoals speciale artiesten)
* Elke variatie in productie (Song remix, VIP, etc.)

#### _songAuthorName
Dit veld beschrijft de hoofdartiest, groep, band, merk, enz. voor het lied.

#### _levelAuthorName
Dit veld beschrijft de persoon die het level heeft gemaakt. Dat ben jij! Of, degene die een level maakt met jouw programma of level editor.

#### _beatsPerMinute
Dit beschrijft de Beats Per Minute (BPM) van jouw nummer. Dit is een floating point nummer, dus BPM waarden met decimalen worden ondersteund.

#### _shuffle
Dit en [`_shufflePeriod`](#shuffleperiod) zijn ongewoon in de community. Als je liedje "zwaait", waar sommige beats in een maat opzettelijk een offset hebben tegenover de rest, kan je potentiële timing problemen op je level corrigeren door `_shuffle` en [`_shufflePeriod`](#shuffleperiod) te gebruiken.

`_shuffle` geeft aan hoe ver objecten zich bewegen wanneer bepaald wordt dat deze op een swing beat zijn. Een positieve waarde betekent dat ze vooruit in de tijd worden verplaatst en een negatieve waarde betekent dat ze terug in de tijd worden verplaatst.

Het totale hoeveelheid waarmee ze worden verplaatst wordt beschreven in [`_shufflePeriod`](#shuffleperiod), omdat ze allebei samenwerken om die waarde te produceren.

#### _shufflePeriod
`_shufflePeriode` wordt gebruikt om te bepalen* wanneer* een swing beat zal plaatsvinden. Specifieker, het is de tijd (in beats) waar een swing beat zal plaatsvinden.

Maar helaas is het ingewikkelder dan dit. Beat Saber wisselt tussen een swing beat en een normale beat met behulp van deze waarde. Laten we bijvoorbeeld aannemen dat je een `_shufflePeriode` hebt van `0.25`. Dit vertelt Beat Saber dat, elke `0.25` beats, het zal afwisselen tussen een swing beat en een normale beat, en zal een offset toepassen als het in een swing beat terechtkomt.

De offset waarde die wordt toegepast op objecten op een swing beat is ongeveer gelijk aan `_shuffle * _shufflePperiod` beats.

Om dit hopelijk beter te begrijpen is hier een tabel van beats, of ze nu een swing beat zijn of niet. en de *werkelijke* beat objecten die op die tijdstippen zullen spawnen. Voor dit voorbeeld, gaan we ervan uit dat
`_shuffle</a> 0.2` is, en dat `_shufflePeriode 0.25` is.</p> 

| Beat van levelbestand | Is het een Swing Beat? | Resulterende beat |
| --------------------- | ---------------------- | ----------------- |
| 0                     | Nee                    | 0                 |
| 0.25                  | Ja                     | 0,3               |
| 0.5                   | Nee                    | 0.5               |
| 0.75                  | Ja                     | 0.8               |
| 1                     | Nee                    | 1                 |
| 1.25                  | Ja                     | 1.3               |
| 1.5                   | Nee                    | 1.5               |
| 1.75                  | Ja                     | 1.8               |




#### _previewStartTime

Dit bepaalt de starttijd (in seconden) voor het in-game voorbeeld van je level. Dit is een floating point nummer, dus waarden met decimalen worden ondersteund.



#### _previewDuration

Dit bepaalt de duur (in seconden) van het in-game voorbeeld van je level. Dit is een floating point nummer, dus waarden met decimalen worden ondersteund.



#### _songFilename

Dit is de lokale locatie naar het audiobestand van je level. In de meeste gevallen zijn de levelbestanden in dezelfde map dus dan is dit alleen de naam en de extensie voor jouw audiobestand (bijvoorbeeld `song.ogg`).



#### _coverImageFilename

Dit is de lokale locatie naar de omslagfoto van je level. Zowel de `.jpg` als `.png` bestandstypen zijn ondersteund. Vergelijkbaar met [`_songFilename`](#songfilename), is dit is meestal alleen de naam en extensie voor de omslagfoto (bijvoorbeeld `cover.jpg`).



#### _environmentName

Dit definieert de interne ID voor de omgeving die het level gebruikt. Om een volledige lijst met geldige omgevingen te krijgen, zie de `Info.dat` namen van elke omgeving in de [Omgevingsvoorbeelden](./basic-lighting.md#omgevingsvoorbeelden) sectie.



#### _allDirectionsEnvironmentName

Dit definieert de interne ID voor de omgeving die het level gebruikt tijdens het spelen in 360 graden of 90 graden levels. Dit is een verplicht veld, ook al bevat het level geen 360 of 90 graden niveaus. Om een volledige lijst met geldige 360 graden omgevingen te krijgen, zie de `Info.dat` namen van elke omgeving in de [Omgevingsvoorbeelden](./basic-lighting.md#omgevingsvoorbeelden) sectie.



#### _songTimeOffset

Dit is de manier van Beat Saber om off-sync audio aan te pakken. This offsets the audio in game, based off the value of `_songTimeOffset` in seconds.

:::warning Hit sounds worden ook beïnvloed door dezelfde offset. We raden de level maker aan om hun audio bestand te synchroniseren *voordat* ze beginnen met het maken van hun level, zoals beschreven in de [Standaard audio setup gids](./basic-audio.md), om elke behoefte aan `_songTimeOffset` en verwante alternatieven te omzeilen. :::



#### _customData

Dit is een optioneel veld dat gegevens bevat die niet gerelateerd zijn aan het officiële Beat Saber level formaat. Als er geen custom data is, dan moet dit object volledig verwijderd worden.

De exacte specificaties over wat er in `_customData` gaat, ligt er helemaal aan de content dat gemaakt is door de community die het nodig heeft. Daarom kunnen we hier niet alle `_customData` velden vermelden. Je moet je eigen onderzoek doen in de Beat Saber community om level editors, programma's of mods te vinden die dit `_customData` object gebruiken.



#### _difficultyBeatmapSets

Dit is een lijst van alle [Difficulty Beatmap Sets](#difficulty-beatmap-sets) gedefinieerd in het level.



### Difficulty Beatmap Sets

Difficulty Beatmap Sets zijn groepen van niveaus, die allemaal onder één kenmerk vallen. Deze vertegenwoordigen jouw Standard, No Arrow, One Saber, en andere kenmerken.



```json
{
  // ... De rest van de Info.dat ...
  "_songTimeOffset": 0,
    "_difficultyBeatmapSets": [
        {
            "_beatmapCharacteristicName": "Standard",
            "_difficultyBeatmaps": [
                // Difficulty beatmap worden later op de pagina uitgelegd.
        // Check de zijbalk!
      ]
    }
  ]
}
```




#### _beatmapCharacteristicName

Dit is de naam van het kenmerk dat aan deze level set is gekoppeld.

Hieronder staan alle veelgebruikte kenmerken. Hoewel ze geen tot weinig "regels" aan zich vast hebben in Beat Saber, hebben ze nog steeds een doel, en zouden ze gevold moeten worden door beide de level editor en de level maker die het level maakt.

Bepaalde kenmerken, die in de onderstaande lijst zijn gemarkeerd, komen niet van het basis spel; maar ze worden toegevoegd door externe mods zoals SongCore. Deze modded kenmerken werken alleen als de gebruiker mods heeft geïnstalleerd die ze toevoegen. en zullen *niet* verschijnen op unmodded kopieën van Beat Saber en kan ervoor zorgen dat het level niet geladen wordt.

| Naam van het karakteristiek | Inbegrepen in het spel | Waar het voor bedoeld is                                                                                      |
|:---------------------------:|:----------------------:| ------------------------------------------------------------------------------------------------------------- |
|         `Standaard`         |           ✔️           | Standaard levels die de standaard gidsen volgen.                                                              |
|         `NoArrows`          |           ✔️           | Beperkt blokken tot Dot (alle richtingen) blokken.                                                            |
|         `OneSaber`          |           ✔️           | Beperkt blokken tot de rechter (blauwe) blokken, en schakelt de linker (rode) blokken uit.                    |
|         `360Degree`         |           ✔️           | Schakelt rotatie evenementen in zonder beperking op de totale rotatie.                                        |
|         `90Degree`          |           ✔️           | Schakelt rotatie evenementen in, maar beperkt deze tot een totale rotatie van 45 graden naar links en rechts. |
|         `Lightshow`         |           ❌            | De plek voor levels die alleen maar verlichtingsevenementen bevatten.                                         |
|          `Lawless`          |           ❌            | Modded levels en modcharts kunnen hier veilig worden geplaatst. Er gelden geen regels hiervoor.               |




#### _difficultyBeatmaps

Dit is een lijst van [Difficulty Beatmaps](#difficulty-beatmaps) gedefinieerd in dit level set.



### Difficulty Beatmaps

Difficulty Beatmaps zijn elk "niveau" van een level. Ze bevatten informatie dat anders is per niveau, zoals [Note Jump Speed](#notejumpmovementspeed), en de locatie van het niveaubestand.



```json
{
  // ... De rest van de Info.dat ...
  "_songTimeOffset": 0,
    "_difficultyBeatmapSets": [
        {
            "_beatmapCharacteristicName": "Standard",
            "_difficultyBeatmaps": [
                {
                    "_difficulty": "ExpertPlus",
                    "_difficultyRank": 9,
                    "_beatmapFilename": "StandardExpertPlus.dat",
                    "_noteJumpMovementSpeed": 18,
                    "_noteJumpStartBeatOffset": 0,
                    "_customData": {
                        // Elke custom data zal hier komen.
            // Als dit leeg is, moet dit volledig worden verwijderd.
          }
        }
      ]
    }
  ]
}
```




#### _difficulty

Dat is het interne niveau, wat geleest word door Beat Saber.

In tegenstelling tot wat je zou kunnen denken, is dit *niet* maar een normale tekenreeks, maar eerder een opsomming. Hier is een lijst van alle geldige niveaus:

* `Easy`
* `Normal`
* `Hard`
* `Expert`
* `ExpertPlus`



#### _difficultyRank

Dit is de sorteervolgorde in het nummerselectie scherm in Beat Saber.

Hoewel dit een gewoon geheel getal is, maakt het veel gebruikte [BeatSaver Schema](#beatsaver-schema) dit nóg een opsomming, gebaseerd op de bovenstaande [`_difficulty`](#difficulty) waarde:

| `_difficulty` | BeatSaver's verwachte `_difficultyRank` |
| ------------- |:---------------------------------------:|
| `Easy`        |                    1                    |
| `Normal`      |                    3                    |
| `Hard`        |                    5                    |
| `Expert`      |                    7                    |
| `ExpertPlus`  |                    9                    |




#### _beatmapFilename

Dit is de locatie van het niveaubestand, wat de blokken, obstakels en verlichtingsevenementen bevat.

Vergelijkbaar met de [`_songFilename`](#songfilename) en [`_coverImageFilename`](#coverimagefilename) van eerder, in veel gevallen is dit alleen maar de naam en extensie (altijd `.dat`) naar het level bestand.

Bij het maken van *nieuwe* niveaus, wordt het aanbevolen dat de naam een van de kenmerken is voor het niveaus parent [Beatmap Set](#difficulty-beatmap-sets), gevolgd door de [`_difficulty`](#difficulty) waarde. Bijvoorbeeld, dit specifieke niveau moet er voor zorgen dat het niveaubestand `StandardExpertPlus.dat` heet.



#### _noteJumpMovementSpeed

Note Jump Movement Speed (afgekort tot "Note Jump Speed", of gewoon "NJS") is de snelheid waarmee objecten de speler naderen, in meters per seconde. Informatie over aanbevolen NJS waarden kan worden gevonden in de [Intermediare mapping pagina](./intermediate-mapping.md#note-jump-speed-spawn-distance). Dit kan een floating point nummer zijn voor preciezere snelheden.

Dit word gebruikt samen met de ingestelde BPM van het nummer om 2 belangrijke waardes te berekenen, genaamd Jump Duration en Jump Distance.

* Jump Duration is de hoeveelheid beats waar objecten actief kunnen zijn.
* Jump Distance is de totale hoeveelheid afstand dat objecten nodig hebben om binnen die Jump Duration te reizen.

De speler staat precies in het midden van deze twee waarden, dus de meeste mappers vinden het handiger om Half Jump Distance en Half Jump Duration te hebben.

* Half Jump Distance is de afstand vanaf de speler waar de objecten spawnen. Sommige mappers noemen dit het "Spawn Point".
* Half Jump Duration is de hoeveelheid beats die nodig zijn voordat het bij de speler is. Het is ook de hoeveelheid beats, vooruit in de tijd, waar objecten spawnen.



#### _noteJumpStartBeatOffset

Deze waarde geld als een directe offset voor de Half Jump Duration, uitgelegd in [`_noteJumpMovementSpeed`](#notejumpmovementspeed), wat op zijn buurt de Jump Distance beinvloed. Dit kan een floating point nummer zijn om een preciezere Jump Duration te krijgen.



#### _customData

Dit is een optioneel veld dat gegevens bevat die niet gerelateerd zijn aan het officiële Beat Saber level formaat. Als er geen custom data is, dan moet dit object volledig verwijderd worden.

De exacte specificaties over wat er in `_customData` gaat, ligt er helemaal aan de content dat gemaakt is door de community die het nodig heeft. Daarom kunnen we hier niet alle `_customData` velden vermelden. Je moet je eigen onderzoek doen in de Beat Saber community om level editors, programma's of mods te vinden die dit `_customData` object gebruiken.



## Difficulty File (v3)

Each Difficulty Beatmap contains a corresponding file which defines the notes, obstacles, events, and other objects for that particular difficulty.

This version was introduced in Beat Saber version 1.20.0.



### Basisobject



```json
{
  "version":"3.0.0", // There must be no whitespace after :
  "bpmEvents": [],
  "rotationEvents": [],
  "colorNotes": [],
  "bombNotes": [],
  "obstacles": [],
  "sliders": [],
  "burstSliders": [],
  "waypoints": [],
  "basicBeatmapEvents": [],
  "colorBoostBeatmapEvents": [],
  "lightColorEventBoxGroups": [],
  "lightRotationEventBoxGroups": [],
  "basicEventTypesWithKeywords": {},
  "useNormalEventsAsCompatibleEvents": false
}
```




#### version

This field describes the version of the map format we are using.



#### bpmEvents

This is an array of [BPM Event](#bpm-events) objects for the map.



#### rotationEvents

This is an array of [Rotation Event](#rotation-events) objects for the map.



#### colorNotes

This is an array of [Color Note](#color-notes) objects for the map.



#### bombNotes

This is an array of [Bomb Note](#bomb-notes) objects for the map.



#### obstacles

This is an array of [Obstacle](#obstacles-2) objects for the map.



#### sliders

This is an array of [Slider](#sliders-2) objects for the map.



#### burstSliders

This is an array of [Burst Slider](#burst-sliders) objects for the map.



#### waypoints

::: tip NOTE
This is a stub section.
::: This is used to control BTS TinyTAN figures. Some information can be found in this [document](https://docs.google.com/spreadsheets/d/1spW7LS-RvenLQBVXJl9w_iOwqr9r_ozxYo3JUlXq9Lc).



#### basicBeatMapEvents

This is an array of [Basic Event](#basic-beatmap-events) objects for the map.



#### colorBoostBeatmapEvents

This is an array of [Boost Event](#color-boost-beatmap-events) objects for the map.



#### lightColorEventBoxGroups

This is an array of Light Color Group Event objects for the map. ::: tip NOTE
This is a stub section. Documentation is a work in progress.
:::



#### lightRotationEventBoxGroups

This is an array of Light Rotation Group Event objects for the map. ::: tip NOTE
This is a stub section. Documentation is a work in progress.
:::



#### basicEventTypesWithKeywords

::: tip NOTE
This is a stub section. Documentation is a work in progress.
:::



#### useNormalEventsAsCompatibleEvents

This is a boolean. ::: tip NOTE
This is a stub section. Documentation is a work in progress.
:::



### Bpm Events



```json
{
  "b": 10.0,
  "m": 128.0,
}
```


:::danger As of Beat Saber `1.20.0`, Official BPM Changes are still not complete. An official mapper has advised against using this event in its current state. :::



#### b

The time, in beats, where this object reaches the player.



#### m

A float representing the new bpm. Any `b` in objects after this point will be adjusted to the new bpm.



### Rotation Events



```json
{
  "b": 10.0, // Beat
  "e": 0,    // Event type
  "r": 15.0, // Rotation
}
```




#### b

The time, in beats, where this object reaches the player.



#### e

| `e` | Resultaat                                                                             |
|:---:| ------------------------------------------------------------------------------------- |
| `0` | Early rotation. Rotates future objects, while also rotating objects at the same time. |
| `1` | Late rotation. Rotates future objects, but ignores rotating objects at the same time. |




#### r

A float which represents clockwise rotation (as viewed from above).



### Color Notes



```json
{
  "b": 10.0, // Beat
  "x": 1,
  "y": 0,
  "c": 0,    // Color
  "d": 1,    // Direction
  "a": 0     // Angle offset
}
```




#### b

The time, in beats, where this object reaches the player.



#### x

An integer number, from 0 to 3, which represents the column where this note is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### y

An integer number, from 0 to 2, which represents the layer where this note is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### c

An integer which represents the color of the note. 

| `c` | Result |
|:---:| ------ |
| `0` | Red    |
| `1` | Blue   |




#### d

This indicates the cut direction for the note.

| `d` | Resultaat       |
|:---:| --------------- |
| `0` | Omhoog          |
| `1` | Omlaag          |
| `2` | Links           |
| `3` | Rechts          |
| `4` | Links boven     |
| `5` | Rechts boven    |
| `6` | Links onderin   |
| `7` | Rechts onderin  |
| `8` | Elke (Dot blok) |




#### a

An integer number which represents the additional counter-clockwise angle offset applied to the note's cut direction in degrees. This has no effect on angles created due to snapping (e.g. dot stack, slanted windows).



### Bomb Notes



```json
{
  "b": 10.0, // Beat
  "x": 1,
  "y": 0
}
```




#### b

The time, in beats, where this object reaches the player.



#### x

An integer number, from 0 to 3, which represents the column where this note is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### y

An integer number, from 0 to 2, which represents the layer where this note is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



### Obstacles



```json
{
  "b": 10.0, // Beat
  "x": 1,
  "y": 0,
  "d": 5,    // Duration
  "w": 1,    // Width
  "h": 3     // Height
}
```




#### b

The time, in beats, where this object reaches the player.



#### x

An integer number, from 0 to 3, which represents the column where this obstacle is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### y

An integer number, from 0 to 2, which represents the layer where base of the obstacle is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2. 

| `y` | Result            |
|:---:| ----------------- |
| `0` | Grounded obstacle |
| `1` | Prone obstacle    |
| `2` | Crouch obstacle   |




#### d

The time, in beats, that the obstacle extends for (duration). While `d` can go into negative numbers, be aware that this has some unintended effects.



#### w

An integer which which represents the width of the obstacle. While `w` can go into negative numbers, be aware that this has some unintended effects.



#### h

An integer numbers from 1 to 5, which represents the height of the obstacle. While `h` can go into negative numbers, be aware that this has some unintended effects.



### Sliders

These describe arcs. If the head or tail of an arc matches a note's time and position, then the arc will connect with the note and alter how the note is scored.



```json
{
  "b": 10.0,  // Head Beat
  "c": 0,     // Color
  "x": 1,     // Head x
  "y": 0,     // Head y
  "d": 1,     // Head direction
  "mu": 1.0,  // Head multiplier
  "tb": 15.0, // Tail Beat
  "tx": 2,    // Tail x
  "ty": 2,    // Tail y
  "tc": 1,    // Tail direction
  "tmu": 1.0, // Tail Multiplier
  "m": 1,     // Mid-anchor mode
}
```




#### b

The time, in beats, where this head of this object reaches the player.



#### c

An integer which represents the color of the note. 

| `c` | Result |
|:---:| ------ |
| `0` | Red    |
| `1` | Blue   |




#### x

An integer number, from 0 to 3, which represents the column where the head of the arc is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### y

An integer number, from 0 to 2, which represents the layer where the head of the arc is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### d

An integer number which represents the head direction of the arc.

| `d` | Resultaat      |
|:---:| -------------- |
| `0` | Up             |
| `1` | Down           |
| `2` | Left           |
| `3` | Right          |
| `4` | Up Left        |
| `5` | Up Right       |
| `6` | Down Left      |
| `7` | Down Right     |
| `8` | Any (Dot Note) |




#### mu

A float which represents how far the arc goes from the head of the arc. If head direction is a dot, this does nothing.



#### tb

The time, in beats, where this tail of this object reaches the player.



#### tx

An integer number, from 0 to 3, which represents the column where the tail of the arc is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### ty

An integer number, from 0 to 2, which represents the layer where the tail of the arc is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### tc

An integer number which represents the tail direction of the arc.

| `tc` | Resultaat      |
|:----:| -------------- |
| `0`  | Up             |
| `1`  | Down           |
| `2`  | Left           |
| `3`  | Right          |
| `4`  | Up Left        |
| `5`  | Up Right       |
| `6`  | Down Left      |
| `7`  | Down Right     |
| `8`  | Any (Dot Note) |




#### tmu

A float which represents how far the arc goes from the tail of the arc. If tail direction is a dot, this does nothing.



#### m

An integer number which represents how the arc curves from the head to the mid point of the arc under certain conditions:

* Head and tail `x` are equal; and
* Head and tail cut direction are equal **OR** their angle difference is 180

:::warning NOTE Currently angle difference is NOT an absolute value. These means only half of the opposing direction pairs will meet these conditions. These pairs are (head -> tail):

* Down -> Up
* Right -> Left
* DownRight -> UpLeft
* UpRight -> DownLeft :::

| `m` | Resultaat         |
|:---:| ----------------- |
| `0` | Straight          |
| `1` | Clockwise         |
| `2` | Counter-Clockwise |




### Burst Sliders

These describe chain and links. If the head of a chain matches a note's time and position, then the chain will connect with the note and alter how the note is scored.



```json
{
  "b": 10.0,  // Beat
  "x": 1,     // Head x
  "y": 0,     // Head y
  "c": 0,     // Color
  "d": 1,     // Head direction
  "tb": 15.0, // Tail Beat
  "tx": 2,    // Tail x
  "ty": 2,    // Tail y
  "sc": 3,    // Segment count
  "s": 0.5    // Squish factor
}
```




#### b

The time, in beats, where this head of this object reaches the player.



#### c

An integer which represents the color of the note. 

| `c` | Result |
|:---:| ------ |
| `0` | Red    |
| `1` | Blue   |




#### x

An integer number, from 0 to 3, which represents the column where the head of the arc is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### y

An integer number, from 0 to 2, which represents the layer where the head of the arc is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### d

An integer number which represents the head direction of the arc.

| `d` | Resultaat                             |
|:---:| ------------------------------------- |
| `0` | Up                                    |
| `1` | Down                                  |
| `2` | Left                                  |
| `3` | Right                                 |
| `4` | Up Left                               |
| `5` | Up Right                              |
| `6` | Down Left                             |
| `7` | Down Right                            |
| `8` | ~~Any (Dot Note)~~ Functions as down. |




#### tb

The time, in beats, where this tail of this object reaches the player.



#### tx

An integer number, from 0 to 3, which represents the column where the tail of the arc is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### ty

An integer number, from 0 to 2, which represents the layer where the tail of the arc is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### sc

An integer number, greater than 0, which represents the number of segments in the burst slider. The head counts as a segment.



#### s

A float which represents squish factor. This is the proportion of how much of the path from `(x,y)` to `(tx, ty)` is used by the chain. This does not alter the shape of the path. Values greater than 1 will extend the path beyond the specified end point.

:::danger
Do not set squish factor to 0. This will crash the game.
:::



### Basic BeatMap Events



```json
{
  "b": 10.0, // Equivalent to _time
  "et": 1,   // Equivalent to _type
  "i": 1,    // Equivalent to _value
  "f": 1.0   // Equivalent to _floatValue
}
```


See [Events](#events-2) in v2 for information of what these equivalent properties represent.



### Color Boost Beatmap Events



```json
{
  "b": 10.0,
  "o": true
}
```




#### b

The time, in beats, where this object reaches the player.



#### o

A boolean which determines whether boost lighting is on or off.  



## Difficulty File (v2)

Each Difficulty Beatmap contains a corresponding file which defines the notes, obstacles, events, and other objects for that particular difficulty.

Version `2.6.0` was introduced in Beat Saber version 1.20.0.  
Version `2.5.0` was introduced in Beat Saber version 1.18.0.  
Version `2.2.0` was introduced in Beat Saber version 1.13.1.



### Base Object



```json
{
  "_version": "2.6.0",
  "_notes": [],
  "_sliders": [], // Introduced in version 2.6.0
  "_obstacles": [],
  "_events": [],
  "_waypoints": [], // Introduced in version 2.2.0
  "_customData": {
    // Any custom data will go here.
    // If empty, this should be removed entirely.
  }
}
```




#### _version

This field describes the version of the map format we are using.



#### _notes

This is an array of [Note](#notes-2) objects for the map.



#### _sliders

This is an array of [Slider](#sliders-4) objects for the map.



#### _obstacles

This is an array of [Obstacle](#obstacles-4) objects for the map.



#### _events

This is an array of [Event](#events-2) objects for the map.



#### _waypoints

::: tip NOTE
This is a stub section.
::: This is used to control BTS TinyTAN figures. Some information can be found in this [document](https://docs.google.com/spreadsheets/d/1spW7LS-RvenLQBVXJl9w_iOwqr9r_ozxYo3JUlXq9Lc).



#### _customData

This is an optional field that contains data unrelated to the official Beat Saber level format. If no custom data exists, this object should be removed entirely.

The exact specifics of what goes in `_customData` is entirely dependent on community-created content that needs them. As such, we cannot list all `_customData` fields here. You will have to do your own searching throughout the Beat Saber community to find map editors, tools, or mods that use this `_customData` object.



### Notes



```json
{
  "_time": 10,
  "_lineIndex": 1,
  "_lineLayer": 0,
  "_type": 0,
  "_cutDirection": 1,
  "_customData": {
    // Any custom data will go here.
    // If empty, this should be removed entirely.
  }
}
```




#### _time

The time, in beats, where this object reaches the player.



#### _lineIndex

An integer number, from 0 to 3, which represents the column where this note is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### _lineLayer

An integer number, from 0 to 2, which represents the layer where this note is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### _type

This indicates the type of note there is. Currently, there are 4 known types, but 1 remains unused:

| `_type` | Resultaat         |
|:-------:| ----------------- |
|   `0`   | Left (Red) Note   |
|   `1`   | Right (Blue) Note |
|   `2`   | Unused            |
|   `3`   | Bomb              |




#### _cutDirection

This indicates the cut direction for the note.

| `_cutDirection` | Resultaat      |
|:---------------:| -------------- |
|       `0`       | Up             |
|       `1`       | Down           |
|       `2`       | Left           |
|       `3`       | Right          |
|       `4`       | Up Left        |
|       `5`       | Up Right       |
|       `6`       | Down Left      |
|       `7`       | Down Right     |
|       `8`       | Any (Dot Note) |




#### _customData

This is an optional field that contains data unrelated to the official Beat Saber level format. If no custom data exists, this object should be removed entirely.

The exact specifics of what goes in `_customData` is entirely dependent on community-created content that needs them. As such, we cannot list all `_customData` fields here. You will have to do your own searching throughout the Beat Saber community to find map editors, tools, or mods that use this `_customData` object.



### Sliders

These describe arcs. If the head or tail of an arc matches a note's time and position, then the arc will connect with the note and alter how the note is scored.



```json
{
  "_colorType": 1,
  "_headTime": 10.0,
  "_headLineIndex": 0,
  "_headLineLayer": 0,
  "_headControlPointLengthMultiplier": 1.0,
  "_headCutDirection": 0,
  "_tailTime": 20.0,
  "_tailLineIndex": 1,
  "_tailLineLayer": 1,
  "_tailControlPointLengthMultiplier": 1.0,
  "_tailCutDirection": 1,
  "_sliderMidAnchorMode": 0,
  "_customData": {
    // Any custom data will go here.
    // If empty, this should be removed entirely.
  }
}
```




#### colorType

This indicates the color of the arc:

| `_colorType` | Result            |
|:------------:| ----------------- |
|     `0`      | Left (Red) Note   |
|     `1`      | Right (Blue) Note |




#### headTime

The time, in beats, where this head of this object reaches the player.



#### headLineIndex

An integer number, from 0 to 3, which represents the column where the head of the arc is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### headLineLayer

An integer number, from 0 to 2, which represents the layer where the head of the arc is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### headControlPointLengthMultiplier

A float which represents how far the arc goes from the head of the arc. If head direction is a dot, this does nothing.



#### headCutDirection

An integer number which represents the head direction of the arc.

| `_headCutDirection` | Result         |
|:-------------------:| -------------- |
|         `0`         | Up             |
|         `1`         | Down           |
|         `2`         | Left           |
|         `3`         | Right          |
|         `4`         | Up Left        |
|         `5`         | Up Right       |
|         `6`         | Down Left      |
|         `7`         | Down Right     |
|         `8`         | Any (Dot Note) |




#### tailTime

The time, in beats, where this tail of this object reaches the player.



#### tailLineIndex

An integer number, from 0 to 3, which represents the column where the tail of the arc is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### tailLineLayer

An integer number, from 0 to 2, which represents the layer where the tail of the arc is located. The bottommost layer is located at layer 0, and inceases to the topmost layer located at index 2.



#### tailControlPointLengthMultiplier

A float which represents how far the arc goes from the tail of the arc. If tail direction is a dot, this does nothing.



#### tailCutDirection

An integer number which represents the tail direction of the arc.

| `_tailCutDirection` | Result         |
|:-------------------:| -------------- |
|         `0`         | Up             |
|         `1`         | Down           |
|         `2`         | Left           |
|         `3`         | Right          |
|         `4`         | Up Left        |
|         `5`         | Up Right       |
|         `6`         | Down Left      |
|         `7`         | Down Right     |
|         `8`         | Any (Dot Note) |




#### sliderMidAnchorMode

An integer number which represents how the arc curves from the head to the mid point of the arc under certain conditions:

* Head and tail `LineIndex` are equal; and
* Head and tail `CutDirection` are equal **OR** their angle difference is 180

:::warning NOTE Currently angle difference is NOT an absolute value. These means only half of the opposing direction pairs will meet these conditions. These pairs are (head -> tail):

* Down -> Up
* Right -> Left
* DownRight -> UpLeft
* UpRight -> DownLeft :::

| `_sliderMidAnchorMode` | Result            |
|:----------------------:| ----------------- |
|          `0`           | Straight          |
|          `1`           | Clockwise         |
|          `2`           | Counter-Clockwise |




#### customData

This is an optional field that contains data unrelated to the official Beat Saber level format. If no custom data exists, this object should be removed entirely.

The exact specifics of what goes in `_customData` is entirely dependent on community-created content that needs them. As such, we cannot list all `_customData` fields here. You will have to do your own searching throughout the Beat Saber community to find map editors, tools, or mods that use this `_customData` object.



### Obstacles



```json
{
  "_time": 10,
  "_lineIndex": 1,
  "_type": 0,
  "_duration": 10,
  "_width": 1,
  "_customData": {
    // Any custom data will go here.
    // If empty, this should be removed entirely.
  }
}
```




#### _time

The time, in beats, where this object reaches the player.



#### _lineIndex

An integer number, from 0 to 3, which represents the column where the left side of the obstacle is located. The far left column is located at index 0, and increases to the far right column located at index 3.



#### _type

An integer number which represents the state of the obstacle.

| `_type` | Result           |
|:-------:| ---------------- |
|   `0`   | Full height wall |
|   `1`   | Crouch/duck wall |




#### _duration

The time, in beats, that the obstacle extends for. While `_duration` can go into negative numbers, be aware that this has some unintended effects.



#### _width

How many columns the obstacle takes up. A `_width` of `4` will mean that this wall will extend the entire playable grid. While `_width` can go into negative numbers, be aware that this has some unintended effects.



#### _customData

This is an optional field that contains data unrelated to the official Beat Saber level format. If no custom data exists, this object should be removed entirely.

The exact specifics of what goes in `_customData` is entirely dependent on community-created content that needs them. As such, we cannot list all `_customData` fields here. You will have to do your own searching throughout the Beat Saber community to find map editors, tools, or mods that use this `_customData` object.



### Events



```json
{
  "_time": 10,
  "_type": 1,
  "_value": 3,
  "_floatValue" : 1.00, // Introduced in version 2.5.0
  "_customData": {
    // Any custom data will go here.
    // If empty, this should be removed entirely.
  }
}
```




#### _time

The time, in beats, where this object reaches the player.



#### _type

An integer number which represents what exact kind of event this object represents.

| `_type` | Result                                                                                                           |
|:-------:| ---------------------------------------------------------------------------------------------------------------- |
|   `0`   | Controls lights in the `Back Lasers` group.                                                                      |
|   `1`   | Controls lights in the `Ring Lights` group.                                                                      |
|   `2`   | Controls lights in the `Left Rotating Lasers` group.                                                             |
|   `3`   | Controls lights in the `Right Rotating Lasers` group.                                                            |
|   `4`   | Controls lights in the `Center Lights` group.                                                                    |
|   `5`   | (Previously unused) Controls boost light colors (secondary colors).                                              |
|   `6`   | (Previously unused) Controls extra left side lights in some environments.                                        |
|   `7`   | (Previously unused) Controls extra right side lights in some environments.                                       |
|   `8`   | Creates one ring spin in the environment.                                                                        |
|   `9`   | Controls zoom for applicable rings. Is not affected by [`_value`](#value).                                       |
|  `10`   | (Previously unused) (Previously Official BPM Changes.)<br/>Billie environment - Controls left side lasers  |
|  `11`   | (Previously unused) <br/>Billie environment - Controls right side lasers.                                  |
|  `12`   | Controls rotation speed for applicable lights in `Left Rotating Lasers`.                                         |
|  `13`   | Controls rotation speed for applicable lights in `Right Rotating Lasers`.                                        |
|  `14`   | (Previously unused) 360/90 Early rotation. Rotates future objects, while also rotating objects at the same time. |
|  `15`   | (Previously unused) 360/90 Late rotation. Rotates future objects, but ignores rotating objects at the same time. |
|  `16`   | Interscope environment - Lowers car hydraulics<br/>Gaga environment - Controls middle left tower height    |
|  `17`   | Interscope environment - Raises car hydraulics<br/>Gaga environment - Controls middle right tower height   |
|  `18`   | Gaga environment - Controls outer left tower height                                                              |
|  `19`   | Gaga environment - Controls outer right tower height                                                             |


:::danger Just because an event type is listed as unused, does *not* mean you are freely available to use it!

Beat Games is known to repurpose previously unused event types for certain features, such as the introduction of 360&deg; / 90&deg; levels. This has broken some Beat Saber maps that make use of legacy MediocreMapper BPM Changes, as well as maps that used Custom Platforms that took advantage of the unused event types. :::



#### _value

Depending on the aforementioned [`_type`](#type) of the event, the `_value` of it can do different things.



##### Verlichting besturen

It's default behavior is controlling brightness and color of lights, and follows this table:

| `_value` | Result                                                                                      |
|:--------:| ------------------------------------------------------------------------------------------- |
|   `0`    | Turns the light group off.                                                                  |
|   `1`    | Changes the lights to blue, and turns the lights on.                                        |
|   `2`    | Changes the lights to blue, and flashes brightly before returning to normal.                |
|   `3`    | Changes the lights to blue, and flashes brightly before fading to black.                    |
|   `4`    | (Previously Unused.)<br/>Changes the lights to blue by fading from the current state. |
|   `5`    | Changes the lights to red, and turns the lights on.                                         |
|   `6`    | Changes the lights to red, and flashes brightly before returning to normal.                 |
|   `7`    | Changes the lights to red, and flashes brightly before fading to black.                     |
|   `8`    | Changes the lights to red by fading from the current state.                                 |


`_value` 4 and 8 were introduced in Beat Saber version `1.18.0` (Billie Eilish patch). These events will only transition from Off and On (0, 1, and 4 )events. They will do nothing if transitions fade and flash events (2, 3, 6, and 7).



##### Het besturen van Boost Colors

| `_value` | Result                                                            |
|:--------:| ----------------------------------------------------------------- |
|   `0`    | Turns the event off - switches to first (default) pair of colors. |
|   `1`    | Turns the event on - switches to second pair of colors.           |




##### Rings besturen

When the event is used to control ring zoom, the `_value` of the event does nothing.

When the event is used to control ring spin, the `_value` only affects cars in the Interscope environment and does nothing in other environments.



##### Auto's besturen

| `value` | Result                                            |
|:-------:| ------------------------------------------------- |
|   `0`   | Affects all the cars. Does not affect hydraulics. |
|   `1`   | Affects all the cars.                             |
|   `2`   | Affects the left cars.                            |
|   `3`   | Affects the right cars.                           |
|   `4`   | Affects the front-most cars.                      |
|   `5`   | Affects the front-middle cars.                    |
|   `6`   | Affects the back-middle cars.                     |
|   `7`   | Affects the back-most cars.                       |




##### Official BPM Changes (before version 2.5.0)

When the event is used to control the BPM, the `_value` represents the new BPM.

The new BPM does not shift internal [`_time`](#time-2) values for future objects. Instead, it essentially recalculates internal game values (Such as Half Jump Duration and Jump Distance) to match the effect of playing the map at the new BPM.

One caveat to this is that the `_value` must *always* be an integer, and does not support floating point numbers (No decimals).

:::warning As of Beat Saber `1.10.0`, Official BPM Changes are broken, and produce unwanted effects when used in a level.

If you absolutely want to work around this, you must create a new BPM Change event so that:

1. Dit nieuwe evenement *moet* exact dezelfde [_time</code>](#time-2) waarde hebben als de BPM change evenement dat je correct wilt laten starten.
2. Dit nieuwe evenement *moet* exact dezelfde `_value` als de vorige BPM change hebben, of de [`_beatsPerMinute`](#beatsperminute) gedefinieerd in [`Info.dat`](#info-dat).

3. Dit nieuwe evenement *moet* gebeuren voor de BPM change dat je correct wilt laten starten, *ookal hebben ze dezelde [`_time`](#time-2) waarden.* :::



##### Laser Rotation Speed besturen

When the event is used to control laser speed for a group of lights, the `_value` is used as a multiplier to their base rotational velocity.

If `_value` is `0`, the random rotation offset for each laser will also be reset, causing all rotating lasers to line up perfectly.



##### 360/90 rotatie besturen

When the event is used to control rotation in a 360/90 degree level, the `_value` is used to add rotation equal to the following table:

| `_value` | Result                      |
|:--------:| --------------------------- |
|   `0`    | 60 Degrees Counterclockwise |
|   `1`    | 45 Degrees Counterclockwise |
|   `2`    | 30 Degrees Counterclockwise |
|   `3`    | 15 Degrees Counterclockwise |
|   `4`    | 15 Degrees Clockwise        |
|   `5`    | 30 Degrees Clockwise        |
|   `6`    | 45 Degrees Clockwise        |
|   `7`    | 60 Degrees Clockwise        |




#### _floatValue

Depending on the aforementioned [`_type`](#type) of the event, the `_floatValue` of it can do different things.



##### Controlling Lights

When the event is used to control lights, the `_floatValue` determines the brightness of the light.



##### Official BPM Changes

:::danger As of Beat Saber `1.18.0`, Official BPM Changes are still not complete. An official mapper has advised against using this event in its current state. ::: When the event is used to control the BPM, the `_floatValue` represents the new BPM. This will also alter the Note Jump Speed proportional to the change in BPM.



#### _customData

This is an optional field that contains data unrelated to the official Beat Saber level format. If no custom data exists, this object should be removed entirely.

The exact specifics of what goes in `_customData` is entirely dependent on community-created content that needs them. As such, we cannot list all `_customData` fields here. You will have to do your own searching throughout the Beat Saber community to find map editors, tools, or mods that use this `_customData` object.



## Credits

The content on this page was authored by [Caeden117](./mapping-credits.md#caeden117) and [Bullet](./mapping-credits.md#bullet) with help from [Kival Evan](./mapping-credits.md#kival-evan) and GalaxyMaster.
