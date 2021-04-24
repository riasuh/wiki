---
sidebar: auto
---

# PC Modding

## Voorwoord

::: danger DISCLAIMER Door mods te gebruiken, begrijp je dat:

* Je ervaart mogelijks problemen die niet voorkomen in de onaangepaste versie van het spel. 99,9% van de bugs, crashes en lag zijn te wijten aan mods.
* Mods worden vrijwel altijd onbruikbaar bij game updates en dat is normaal - wees geduldig en blijf respectvol wanneer dit gebeurt, want de modders zijn vrijwilligers met andere dingen in hun leven naast het maken van mods.
* Beat Games probeert niet met opzet ervoor te zorgen dat mods niet meer werken. Ze willen enkel aan hun eigen code werken en soms maakt dit mods onbruikbaar, maar dit betekent dus niet dat ze expres mods in de weg zitten.

Val de ontwikkelaars niet aan voor problemen gerelateerd aan het gebruik van mods, en vice versa - de modders en spel ontwikkelaars zijn twee aparte groepen. Wees gewoon geen eikel. :::

:::warning WEES VOORZICHTIG TIJDENS HET INSTALLEREN VAN MODS Beat Saber zal je **nooit** vragen om het als administrator te starten.

Als je een mod hebt gedownload en geïnstalleerd en je krijgt het gebruikersaccountbeheer pop-up, **klik dan NIET** op "Ja", en rapporteer dit alsjeblieft. Wat je hebt geïnstalleerd is een kwaadaardige mod!

Als je niet zeker weet of iets wat je hebt geïnstalleerd malware is of niet, ***vraag het dan aan iemand in onze Discord***. :::

Beat Saber heeft ingebouwde ondersteunding voor zelfgemaakte nummers, dus als dat alles is wat je nodig hebt, dan heb je geen extra mods nodig! Het is echter een goed idee om `SongCore` te installeren, omdat deze mod de basis functionaliteit van het spel uitbreid door het verbeteren van laadtijden en functionaliteit te bieden aan andere mods zoals een in-game downlodaer voor nummers, een kunstmatige leaderboards, afspeellijsten, enz.

::: warning Waarschuwing Deze gids is geschreven voor PC modding op Windows.  
Als je een Quest hebt, ga dan naar de [Quest Modding pagina](/nl/quest-modding.md).  
Als je Linux gebruikt, ga dan naar de [Linux pagina](/nl/modding/linux.md) of [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/blob/master/README.md) :::

Als je tegen problemen aanloopt, ga dan naar de [ondersteuningspagina](./support) en probeer de oorzaak van het probleem te identificeren voordat je het vraagt in de Discord server. De kans is groot dat het antwoord dat je zoekt al op die pagina staat!

::: warning Ik heb een video tutorial bekeken op YouTube, maar ik liep vast / het werkte niet. Waarom? Wij van de BSMG raden het **sterk** af om video tutorials te gebruiken voor het modden. Vaak vinden we dat de inhoud veroudered is, of dat ze incompleet zijn, of dat ze fouten, of gewoon incorrecte informatie bevatten.

In plaats daarvan is het beter de geschreven gidsen te volgen die hier op de wiki beschikbaar zijn, of om hulp te vragen in de [BSMG Discord](https://discord.gg/beatsabermods). :::

## Installatieprogramma's

### Mod Assistant
> **DIT IS OP HET MOMENT DE AANBEVOLEN MOD INSTALLER.**

__**Start het spel minstens 1 keer op**** voordat je probeert het spel te modden! Dit geldt ook als je je spel opnieuw installeert.

Een simpel Beat Saber mod installatie programma vergelijkbaar met mod manager, maar met extra functies zoals het verwijderen van mods en het controleren van versies! Download het op [Assistant's GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Hoe kom ik aan meer nummers
::: tip Hint De meeste levels in de "Top All", "Rating", "Downloads" of "Plays" sorteerfilters werden gemaakt voordat er best practices voor het maken van levels werden vastgelegd. Probeer levels van tussen eind 2019 en nu te downloaden voor de beste custom levels ervaring. :::

::: warning Waarschuwing Het is een goed idee om periodiek een back-up te maken van jouw `CustomLevels` map, omdat er een kleine kans is dat het wordt gereset als het spel update!

Deze map bevindt zich in jouw installatie map: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### In-game Downloader
Met de `BeatSaver Downloader` mod kan je nummers downloaden terwijl je in het spel door de `MORE SONGS` menu knop op het `MODS` scherm te gebruiken. Dit download nummers rechtstreeks van [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) is de hoofd database van custom levels gemaakt door de community. Veel andere programma's en websites verbeteren de ervaring van het downloaden van custom levels, maar deze website is de plek waar ze opgeslagen worden. Om de nummers te installeren die van de site zijn gedownload, pak deze nummers uit in een map en plaats deze map in `Beat Saber/Beat Saber_Data/CustomLevels`. Je kan ook gebruik maken van de in-game downloader mod, of Mod Assistant's OneClick™ Install functie.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) is een website die probeert het vinden van fantastische nummers om te spelen veel makkelijker te maken. Het doet dit door de duizenden nummers van BeatSaver te categoriseren en laat je deze sorteren op het genre en vele andere attribuut labels. Ook heeft het een volledig sociale functie waar spelers nummers kunnen bekijken en hierop commentaar kunnen geven. Een van de meest gebruikte functies is de "Curator Recommended" functie waar een team de meeste nummers die elke dag uitkomen spelen en de nummers die het meest opvallen aanbevelen om deze [automatisch in het spel downloaden](https://bsaber.com/beatsync/).

### Apps voor het beheren van je nummers

Er zijn op dit moment geen werkende apps voor het beheren van je nummers beschikbaar.

### Afspeellijsten
Hiervoor moet je de [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod installeren.

Daarna kan je één van de onderstaande twee dingen doen:

* Gebruik de `Install playlists` knop in het Opties tabblad in Mod Assistant.
* Plaats de afspeellijst in `Beat Saber/Playlists` en selecteer de titel van de afspeellijst in het spel en klik dan op download all songs.

Je zou in het spel de afspeellijst naast de custom levels albums moeten kunnen zien. De mod ondersteunt ook het beheren van afspeellijsten in het spel.

## Installatie Map
_Waar is Beat Saber geïnstalleerd?_

### Standaard locatie
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Andere locaties
**Als je de installatiemap hebt verplaatst naar een andere schijf, dan kan het op de onderstaande locatie staan.** Vervang de schijfletter `F` door degene van de schijf waarop je spel is geïnstalleerd.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Handmatige installatie
Een mod installatie programma is de aanbevolen manier om mods te installeren. Zie de sectie [hierboven](#installers). Als je het spel al hebt gemodificeerd en alleen mods wil installeren die niet in de installer beschikbaar zijn, ga dan direct door naar stap 4.

::: warning WEES VOORZICHTIG TIJDENS HET INSTALLEREN VAN MODS Het modden van je spel met niet goedgekeurde mods, zoals de mods die gevonden worden in het `#pc-mods` kanaal, komt met risico's. Waaronder de mogelijkheid op kwaadaardige software dat zich gedraagt als een normale mod.

Beat Saber zal jou **NOOIT** vragen om het als administrator uit te voeren.

Als je een mod hebt gedownload en geïnstalleerd en je krijgt het Gebruikersaccountbeheer prompt, **klik dan NIET** op accepteer, en rapporteer dit alsjeblieft. Als je niet zeker weet of iets wat je hebt geïnstalleerd malware is of niet, ***vraag het dan aan iemand in onze discord***. :::

**Start het spel op zijn minst 1 keer** voordat je probeert het spel te modden! Dit geldt ook voor het opnieuw installeren van je spel.

### BSIPA installeren

1. Download [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Navigeer naar jouw [installatiemap.](#install-folder) En pak de inhoud van de BSIPA zip hierin uit. ![Directory Clean](~@images/beginners-guide/directory-clean.png "Directory Clean") ![Directory Ipa](~@images/beginners-guide/directory-ipa.png "Directory Ipa")
3. Dubbel-klik op IPA.exe om het spel te modificeren. Alle mods in de `Plugins` map worden nu geladen bij het starten van het spel. Als er foutmeldingen zijn, dan heb je waarschijnlijk stap 2 niet correct gevolgd. ![Directory Patched](~@images/beginners-guide/directory-patched.png "Directory Patched")

### Installeer mods

4. Download de mod(s) die je wilt installeren, of het vanaf GitHub is, het [BSMG Discord](https://discord.com/invite/beatsabermods) `#pc-mods` kanaal,  [BeatMods](https://beatmods.com/#/mods) of van andere bronnen. **Zorg ervoor dat je alle afhankelijkheden download die vereist zijn door de mod(s).** ![Directory Plugins](~@images/beginners-guide/directory-plugins.png "Directory Plugins")
5. Sommige mods hebben installatie-instructies, sommige niet. Over het algemeen kun je de inhoud van de zip naar je Beat Saber installatiemap slepen en neerzetten, de bestanden in de zip zouden naar de bijbehorende mappen moeten gaan.

## Het de-installeren van mods
Verwijder de .dll van de `Plugins` map, of klik op de `Uninstall` knop in Mod Assistant.

## Waar kan je verder gaan

* [Grepen en Trucs](./grips-and-tricks.md)
* [Nummers maken](/nl/mapping/)
* [Custom Sabers](/nl/models/custom-sabers.md)
* [Custom Avatars](/nl/models/custom-avatars.md)
* [Custom Platforms](/nl/models/custom-platforms.md)
* [Speel custom levels in mulitplayer](https://discord.com/invite/gezGrFG4tz)
* [Het maken van mods](/nl/modding/)

## Heb je vragen?
Bezoek de hulp kanalen in de [BSMG Discord](https://discord.gg/beatsabermods)!
