---
sidebar: auto
prev: ./basic-audio.md
next: ./intermediate-mapping.md
description: Diese Seite wird dir alle Informationen und Ratschläge geben, um deine Maps ansprechend zu gestalten!
---

# Mapping-Grundlagen
_Wenn du noch wenig Erfahrung im Mapping hast, lese die gesamte Seite. Bis aufs letzte Wort. Bis aufs letzte Bild. Diese Seite wird dir alle Informationen und Ratschläge geben, um deine Maps ansprechend zu gestalten!_

* [Glossar](./glossary.md)

## Bereit zum Mappen?
**Hast du...**

1. [x] [Audacity](https://www.audacityteam.org/) und einen der [Map-Editor](./#hilfsmittel-für-mapping) heruntergeladen?
2. [x] [Deine Audio-Datei vorbereitet](./basic-audio.md) und überprüft, dass die eingestellte BPM stimmt und du ein passendes Intro/Outro hast?
3. [x] Deine Songdatei als OGG <a href="./basic-audio.md#exportieren>exportiert</a>?

::: tip Wenn alles vorbereitet ist: SEHR GUT! Jetzt kannst du in den Editor gehen und mappen! Falls nicht, folge den Links für weitere Informationen. :::

## Das Grundlegende
Bevor du ans Mappen gehst, solltest du die Grundlagen verstehen.

### Map-Dateien
Unabhängig vom Editor benötigt jede Map folgendes:

* **Songdatei:** OGG-Format, diese muss vorbereitet sein. Nenne die Datei `song.ogg`
* **Titelbild:** JPG- oder PNG-Format, muss ein Quadrat sein. 512 Pixel pro Seite sind empfohlen. Du benötigst es, um eine Map zu veröffentlichen.  Nenne die Datei `cover.jpg` bzw. `cover.png`
* **Info-Datei:** Enthält alle Metadaten der Map. Einträge in dieser Datei beziehen sich auf alle Schwierigkeiten (z.B. Name des Liedes / Künstlers / Mappers, Name der Songdatei / des Titelbildes, Geschwindigkeit der Noten, etc.). Diese Datei wird von dem Editor automatisch erstellt.
* **Schwierigkeits-Dateien:** Eine pro Schwierigkeit deiner Map. Einträge in diesen Dateien beziehen sich auf jeweils eine Schwierigkeit (z.B. Noten, Licht-Events, etc.). Diese Dateien werden von dem Editor automatisch erstellt.

Einige Editoren erstellen zusätzlich den Ordner `Autosaves`. In diesem befinden sich ältere Versionen deiner Schwierigkeits-Dateien. Wenn du deine Map hochladen willst, benötigst du mindestenst vier Dateien.

::: warning
Sonderzeichen aus anderen Sprache wie Japanisch (日本語/にほんご), Kaomoji (٩(◕‿◕｡)۶), Chinesisch (汉语/漢語), Arabisch (اَلْعَرَبِيَّةُ‎), und Buchstaben mit Akzent (Ä/é/ó) werden nicht vollständig von BeatSaver unterstützt. Das Nutzen dieser Zeichen in den Metadaten oder in Lesezeichen kann zu Problemen führen.
:::

### Arten von Blöcken
<!-- markdownlint-disable MD013 -->
|                        Richtungsblöcke                         |                  Punkt-Blöcke                  |                                                   Bomben                                                    |                                                 Wände                                                 |
|:--------------------------------------------------------------:|:----------------------------------------------:|:-----------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------:|
|        ![Pfeil-Block](~@images/mapping/arrow-block.png)        | ![Punkt-Block](~@images/mapping/dot-block.png) |                                     ![Bombe](~@images/mapping/bomb.png)                                     |                                  ![Wand](~@images/mapping/wall.png)                                   |
| Müssen in die Richtung des<br />Pfeils geschlagen werden |  Können aus jeder Richtung geschlagen werden   | Ziehen Leben ab, wenn sie mit dem Saber geschlagen werden,<br /> reagieren aber nicht auf den Spieler | Ziehen Leben ab, wenn sich der Spieler darin befindet,<br /> reagieren aber nicht auf die Saber |
<!-- markdownlint-enable MD013 -->

**Anmerkungen zu Wänden:**

* Normale Wände können von jedem sind mit jedem VR-Headset kompatibel. Unerfahrene Mapper sollten nur diese Art von Wand benutzen.
* Es gibt ein paar "hacky" Wände, die keine weiteren Mods (wie z. B. Mapping Extensions) benötigen: "Fast Walls" (fliegen schneller als normale Wände), "Hyper Walls" (fliegen sehr schnell), und "Fake Walls" (sehen aus wie normale Wände, ziehen dem Spieler aber kein Leben ab).
* Diese Wände werden von manchen Editoren unterstützt. Da sie Spielmechaniken ausnutzen, sind sie jedoch nicht für das Ranglistensystem zugelassen.
* Weitere Informationen findest du zu Basisspiel-Wänden unter [Mapping für Anfänger](./intermediate-mapping.md) und zu "extravaganten" Mapping/Noodle Extensions-Wänden unter [Fortgeschrittenes Mapping](./extended-mapping.md)

**Anmerkungen zu Bomben:**

* Die Hitbox der Bomben ist kleiner als die eines Blocks, und sogar kleiner als das Model selbst.
* Bomben sind schwer zu erkennen, wenn keine Licht-Effekte benutzt werden. Stelle sicher, dass es nicht dunkel ist, wenn Bomben auftauchen. Weitere Informationen unter [Lighting-Grundlagen](./basic-lighting.md).
* Bomben können auch getroffen werden, nachdem sie an dem Spieler vorbei geflogen sind.

### Block-Verteilung
Die Verteilung der Blöcke hängt von der Schwierigkeit und der Zielgruppe ab, die du erreichen willst. Anfänger können von einer gleichmäßigen Verteilung aller Reihen überfordert werden, während erfahrene Spieler damit keine Probleme haben. Die Verteilung hängt bei gleicher Schwierigkeit auch von dem Mapping-Stil ab.

Weitere Informationen zu Nutzung der Reihen in [Schwierigkeit Einschätzen](#schwierigkeitsgrad-einschätzen-down-mapping).

::: tip Wenn du [Mediocre Map Assistant 2](./mediocre-map-assistant.md) als Editor verwendest, kannst du <kbd>SHIFT</kbd>+<kbd>TAB</kbd> verwenden, um die Statistiken über das <kbd>Stat Panel</kbd> anzuschauen. :::

## Timing & Rhythmus
Bevor du ernsthaft mit dem Mappen anfängst, musst du dir Gedanken über den Rhythmus des Liedes machen, das du mappst. Du wirst die Blöcke auf einem oder mehereren Hauptinstrumente des Liedes platzieren: Dem Drumbeat, dem Leitinstrument, dem Bass, den Synths, oder dem Gesang.

Um die Blöcke im Rhythmus zu platzieren, musst du die Cursor-Präzision variieren. Die meisten (aber nicht alle) Lieder werden 1/1, 1/2 oder 1/4 Cursor-Präzision benötigen, um den Beat zu treffen. Einige Lieder können 1/3 Cursor-Präzision durch Triolen benötigen, die für das unerfahrene Ohr schwer von 1/4 zu unterscheiden sind. Für die meisten Lieder benötigst du nicht weniger als 1/4 Cursor-Präzision, *auch* wenn du Vocals mappst.

::: warning  
90% der Zeit führt hohe Präzision (1/8, 1/16, 1/32, or 1/64) dazu, dass deine Map nicht richtig getimed ist. Wenn du eine sehr hohe Präzision benötigst, damit deine Noten richtig getimed sind, hast du deine Audiodatei nicht richtig vorbereitet. STOP und schaue die [Audiosetup-Grundlagen](./basic-audio.md) an, um sicher zu stellen, dass das Lied synchron ist! :::

|                            1/1 Cursor-Präzision                            |                            1/2 Cursor-Präzision                            |                            1/3 Cursor-Präzision                            |                            1/4 Cursor-Präzision                            |
|:--------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| ![Screenshot von 1/1 Cursor-Präzision](~@images/mapping/1-1_precision.png) | ![Screenshot von 1/2 Cursor-Präzision](~@images/mapping/1-2_precision.png) | ![Screenshot von 1/3 Cursor-Präzision](~@images/mapping/1-3_precision.jpg) | ![Screenshot von 1/4 Cursor-Präzision](~@images/mapping/1-4_precision.png) |
|                           1 Block pro Taktschlag                           |                          2 Blöcke pro Taktschlag                           |                          3 Blöcke pro Taktschlag                           |                          4 Blöcke pro Taktschlag                           |

Wenn du dich an das Timing deiner Map setzt, willst du dir WIRKLICH sicher sein, dass die Waveform im Editor mit den großen Strichen der Editorspur übereinstimmt. Wenn deine Waveform nicht richtig ausgerichtet ist, schaue dir die Wiki-Seite zu [Audiosetup-Grundlagen](./basic-audio.md) erneut an.

::: danger ACHTUNG  
Wenn deine Waveform nicht richtig ausgerichtet ist, wird es **sehr** schwierig sein, deine Blöcke richtig zur Musik zu platzieren. Stelle es vor dem Mappen richtig ein, ansonsten musst deine Map später überarbeiten! :::

|                            Audio nicht richtig ausgerichtet                            |                                  Audio korrekt synchronisiert                                  |
|:--------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------:|
| ![Editor-Ansicht mit falsch synchronisiertem Audio](~@images/mapping/audio-broken.png) | ![Editor-Ansicht mit zur Editorspur synchronisiertem Audio](~@images/mapping/audio-synced.png) |
|      Benötigt Audiobearbeitung, Start Offset, oder du verwendest die falsche BPM       |                                   Du bist bereit zu Mappen!                                    |

### Timing-Noten
Überlege dir, den Mapping-Prozess mit Platzhalter- oder "Timing"-Noten zu starten. Mit "Punkt-Blöcken" als Platzhalter kannst du leicht sehen, ob deine Map richtig getimed ist und ob du zusäzliche Betonung benutzten willst, **bevor** du eine Menge Zeit mit den Patterns verbringst. Achte darauf, dass die Schlaggeräusche des Editors im Takt des Beats sind.

::: tip  
Nicht jeder verwendet Timing Notizen, aber sie können eine hilfreiche Methode sein, um sicherzustellen, dass deine Maps als neuer Mapper richtig getimt sind. :::

### Overmapping & Undermapping
Platziere bewusst Blöcke, die zur Musik passen. Platziere nicht mehr Blöcke als nötig, nur um die Karte schwierig zu gestalten. Einige Songs waren nie dazu gedacht, superdichte ExpertPlus Maps zu sein, und das ist ok.

* **Overmapping** ist die (schlechte) Praxis, mehr Blöcke zu platzieren als Töne vorhanden sind. Tue es nicht.
* **Undermapping** ist die sehr akzeptable Praxis des Überspringens einiger Noten/Schläge (besonders bei niedrigeren Schwierigkeiten).

### Betonung & Konsistenz
Wir gehen in [Intermediate Mapping](./intermediate-mapping.md) näher darauf ein, aber als neuer Mapper solltest du zumindest die grundlegenden Ideen von Betonung und Konsistenz verstehen und wie sie sich auf die Map auswirken.

**Emphasis** ist, wie viel "Gewicht" du jedem Treffer gibst.

* Betrachte den Basis-Sound deines Mappings als einen einzelnen Hit (einen Block), einschließlich leiser oder chilligere Abschnitte
* Wenn der Sound "größer" ist oder zwei verschiedene Instrumente auf denselben Beat schlagen, kannst du über einen Doppelschlag oder einen Stack (zwei Blöcke) nachdenken.
* Nur für die größten Töne im Lied kannst du einen Doppelturm (vier Blöcke, zwei für jede Hand) oder ein anderes schwergewichtiges Muster verwenden, aber viele Lieder brauchen diese Betonung nicht.

Viele neue Mapper wollen instinktiv die ganze Zeit Doppelschläge verwenden, aber denke daran, dass diese eine starke Betonung darstellen, und wenn *jeder Klang* betont wird, dann fühlt sich <em x id="3">nichts</em> so an, als hätte es zusätzliches Gewicht.

Man kann es auch so sehen, dass die Energie und Anstrengung des Schlags der Energie und Kraft des Klangs entsprechen soll. Niemand schreit bei jedem Gesang oder bei jeder Instrumenten-Note aus voller Kehle. Du willst, dass die kraftvollen Noten, der kraftvollen Gesang aus dem Rest des Songs herausstechen. Auch wenn der größte Teil des Liedes laut oder (Deiner Meinung nach) betont klingt, gibt es immer Noten, die darüber liegen. Sei es durch Lautstärke oder durch Energie. Wenn du also mappst schaue, was deine Basisenergie ist, und mappe diese als Einzelperson. Bei allem, was darüber hinausgeht, kannst du Towers/Doubles/Windows/Jumps machen, was immer am besten zu dieser Energie passt.

**Konsistenz** bedeutet, den gleichen Klang mit dem gleichen Gewicht abzubilden, wenn er erscheint.  
Konsistent abzubilden bedeutet NICHT immer, zu kopieren/einzufügen/zu spiegeln, auch wenn dies in manchen Fällen angebracht ist. Wenn du z. B. einen bestimmten großen Sound als Double zuweist, sollte dieser Sound immer mit einem Double zugewiesen werden.

## Bewährte Praktiken für Pattern
Dieser Abschnitt beschreibt die Grundsätze, die man für eine spielbare und angenehme Map befolgen sollte.

**Cyrix** hat ein zusammenfassendes Video, [Patterns to Avoid as a New Mapper](https://www.youtube.com/watch?v=mgGaqZ20Scw), zu den häufigsten Problemen, die in diesem Abschnitt behandelt werden, erstellt.

### Vision Blocks
Vision Blocks sind alle Pattern, die die Sicht des Spielers verdecken und das Lesen der Map erschweren, wenn nicht sogar unmöglich machen. Die Hauptursache für Vision Blocks ist die Verwendung der beiden mittleren Positionen der Spur. Das Risiko einer Blockade besteht immer, wenn die mittlere Reihe verwendet wird.

**Vision Blocks können vermieden werden durch:**

* Nicht die beiden mittleren Positionen der Spur verwenden oder
* Sicher zu stellen, dass Blöcke, die auf etwas in der mittleren Reihe folgen, entweder weit genug entfernt sind oder an einer anderen Stelle rechts oder links vom Block stehen.
* Zu vergewissern, dass der Spieler entweder durch Hindernisse oder Muster zur Seite gedrängt wird, damit die mittleren Positionen den Spieler nicht mehr vollständig blockieren.

<!-- markdownlint-disable MD013 -->
|                        Ideale Blockplatzierung                         |                              Vision Block Platzierung                               |
|:----------------------------------------------------------------------:|:-----------------------------------------------------------------------------------:|
|     ![Keine Vision Blocks](~@images/mapping/no-vision-blocks.jpg)      |                   ![Face Notes](~@images/mapping/face-notes.jpg)                    |
| Wenn du anfängst, halte dich<br />an die Begrenzung der Strecke. | Diese werden als "Face Notes" bezeichnet.<br />Vermeide sie als neuer Mapper. |
<!-- markdownlint-enable MD013 -->

::: tip  
**Mediocre Map Assistant 2** verfügt über einen eingebauten, praktischen Fehlerprüfer, der Vision Blocks finden kann. Weitere Informationen findest du im [MMA2 User Guide](./mediocre-map-assistant.md#error-checker). :::

### Double Directionals & Resets
Double Directionals (oder DDs) erhält man, wenn zwei Blöcke der gleichen Farbe innerhalb einer sehr kurzen Zeitspanne in die gleiche Richtung laufen. Diagonals oder jede Änderung von nur 45 Grad zwischen den Blöcken werden als DDs mit den beiden Kardinalrichtungen betrachtet, die sie kombinieren.

::: align center ![Blue up right diagonal block](~@images/mapping/bnur.png)ist eine DD mit beiden ![Blue up block](~@images/mapping/bnu.png) und ![Blue diagonal block](~@images/mapping/bnr.png) :::

Bei doppelten Richtungswechseln verdoppelt der Spieler seine Schwunggeschwindigkeit im Vergleich zu einem "normalen" Aufwärts-/Abwärtsmuster. Sie müssten nach unten schwingen und dann die Hand wieder nach oben bringen, um erneut nach unten zu schwingen, was eine Menge unnötiger Bewegung bedeutet. Wechsel die Richtung jedes zweiten Blocks für einen besseren Fluss.

Viele neue Mapper verwenden DDs, um das Gefühl des Schlagzeugspiels zu simulieren. Auch wenn sich das *anfühlt*, als ob es Sinn machen würde, haben Trommeln einen Rückstoß, wenn man sie schlägt, und imaginäre Computerblöcke... nicht. Das Spiel heißt Beat Saber, nicht Beat Drummer!

|                             Standard Flow                             |                            Double Directionals                            |
|:---------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| ![Image of standard up down flow](~@images/mapping/standard-flow.jpg) | ![Image of double directionals](~@images/mapping/double-directionals.jpg) |
|                       Eine gute Mapping-Praxis                        |                           Yikes! Tu dies nicht.                           |

**Resets** DDs *haben* ihren Nutzen (typischerweise in "tänzerischen" Karten), wenn man dem Spieler genug Zeit gibt, seine Hände in die neutrale Position zurückzusetzen. Dies bedeutet in der Regel, dass keine DD's innerhalb von 2 Beats für "normale" bpm Songs und länger für hohe bpm Songs.

::: warning  
Wenn du absichtliche DDs in einer tanzähnlichen Karte verwendest, musst du deine NJS langsamer und den Spawn-Offset länger machen, damit der Spieler genug Zeit hat zu reagieren. :::

::: danger
Handgelenksrückstellungen sind, wenn du den Vorhand-/Rückhand Flow eines Musters mitten im Spiel änderst, so dass der Spieler sein Handgelenk abrollen muss, um den Flow zurückzustellen. Du kannst die normale menschliche Körpermechanik stören und die Spieler einem ernsthaften Risiko von Gelenkschäden aussetzen. Verwende keine Resets mit hoher Präzision!
:::

Wenn zwischen den Noten längere Zeit verstreicht, wird der Spieler seine Armposition neu einstellen, so dass es oft besser ist, den neuen Abschnitt mit einem Abwärtsblock zu beginnen.  In zeitlichen Grauzonen, wie z. B. 3 Sekunden ohne Noten, liegt es am Mapper, den Spieler zurückzusetzen oder den Fluss fortzusetzen.

Möchten du mehr über Resets wissen? Lies [Intermediate Mapping](./intermediate-mapping.md)!

### DO: Mapping mit Flow
Außerhalb der leichten und normalen Schwierigkeiten ist das Mapping mit Flow ein absolutes Muss. Der menschliche Körper ist eine unglaubliche Maschine, aber es gibt bestimmte Bewegungsabläufe in den Gelenken und die Verwendung von Bewegungsmustern, die diese Mechanik verletzen, welches ein Rezept für die Verletzung des Spielers ist.

Parity ist das Konzept, dass jede Blockrichtung entweder mit einem Rückhand- oder einem Vorhandschwung gespielt wird. Alternating between foreswing and backhand swings with each block gives a smooth motion between each hit:

* A **forehand** swing is the motion where the block is hit with the **palm** of the hand
* A **backhand** swing is the motion where the block is hit with the **back** of the hand

The diagram below illustrates how straining it is playing a note as either swing (mirrored for red). Without proper lead in for harsher swings, the player is likely to reset:

|                     Forehand Swings                      |                     Backhand Swings                      |
|:--------------------------------------------------------:|:--------------------------------------------------------:|
| ![Forehand Strain](~@images/mapping/forehand_strain.png) | ![Backhand Strain](~@images/mapping/backhand_strain.png) |

This video illustrates the concept of parity: [YouTube](https://youtu.be/e0YlLwBz7Vk)

A thing important to keep in mind, especially if you are new to the game or mapping, is that the concept of parity is most obvious for wrist players. If you do not play with your palm directly facing the ground, then you might struggle to understand why some parity breaks are uncomfortable. Remember that while it may feel fine to you, players have different grips and styles. Proper parity feels good for everyone, not just some playstyles.

::: tip  
When proper flow is achieved the player should be physically capable of getting full points on each block, even if they don’t have the skill or interest in doing so. See the [Scoring](/grips-and-tricks.md#scoring) section of the wiki for more info. :::

|                              0° Angle                              |                              45° Angle                               |                              90° Angle                               |                               135° Angle                               |                               180° Angle                               |
|:------------------------------------------------------------------:|:--------------------------------------------------------------------:|:--------------------------------------------------------------------:|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| ![0 degree angle change between blocks](~@images/mapping/0deg.png) | ![45 degree angle change between blocks](~@images/mapping/45deg.png) | ![90 degree angle change between blocks](~@images/mapping/90deg.png) | ![135 degree angle change between blocks](~@images/mapping/135deg.png) | ![180 degree angle change between blocks](~@images/mapping/180deg.png) |
|                              No. (DD)                              |                               No. (DD)                               |                                Maybe.                                |                                  Yes.                                  |                                  Yes.                                  |

**Basic Flow Concepts:**

* The higher your note precision, the more you want to stick to 180° (up/down) and 135° (up/down/diagonal) patterns.
* Larger angle changes should only be considered with enough time to play smoothy.
* Make sure that you have the right setup (the pattern immediately before) and escape (the pattern immediately after) for a comfortable swing at whatever speed you’re mapping.
* Be conscious of your timing, you can get away with more in slower BPM songs with the same note precision than you can in high BPM songs. Map for the style of song you’ve selected.

### DON'Ts: Verbotene Patterns
These are called forbidden patterns for a reason. There is no reason in the world to use these because they're dangerous to either the player's hardware, the player's joints, or they go against the scoring system. You may have played maps that included these but that doesn't make them ok.

#### Handclaps
|                              Abbildung                               |                             Editor-Ansicht                              | Erklärung                                                                                                                                                                                                                                                                                                                                                                                    |
|:--------------------------------------------------------------------:|:-----------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a handclap](~@images/mapping/controller-smash.png) | ![Editor view of a handclap](~@images/mapping/controller-smash-alt.png) | Pointing blocks at each other may cause the player to smash their controllers together when playing for max points. Don’t do it, no exceptions.<br /><br />Note: Different VR sets have different controllers. Vive wands are much bigger than Oculus touch controllers and Index knuckles... don’t put your players’ hardware at risk! *AKA Controller clash, Controller smash* |

#### Hammer Hits
|                            Abbildung                             |                           Editor-Ansicht                            | Erklärung                                                                                                                                     |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a hammer hit](~@images/mapping/hammer-hit.png) | ![Editor view of a hammer hit](~@images/mapping/hammer-hit-alt.png) | Any directional block pointing towards a bomb on the same plane is just evil (and undermines the scoring system). Don’t do it. No exceptions. |

#### Entkörperte Noten
|                                  Abbildung                                   |                                 Editor-Ansicht                                  | Erklärung                                                                                                                                                                                                                            |
|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of disembodied notes](~@images/mapping/disembodied-notes.png) | ![Editor view of disembodied notes](~@images/mapping/disembodied-notes-alt.png) | Do not hide blocks on the other side (or inside) of walls. Most of the time, these are simple mistakes that people don’t find because they don’t adequately playtest their maps (NOTE: Always [playtest](./#playtesting) your maps!) |

#### Schnelles Wall Dodge
|                                 Abbildung                                  |                                Editor-Ansicht                                 | Erklärung                                                                                                                                                                                                                                                                                                                         |
|:--------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of rapid wall dodge](~@images/mapping/rapid-wall-dodge.png) | ![Editor view of rapid wall dodge](~@images/mapping/rapid-wall-dodge-alt.png) | Keep head movement slow and predictable. Do not force the player to very quickly move from one side of their play space to the other. Wall dodges are fine (and fun!) to use but allow *at least* 1.5 beats for the player to switch sides for higher BPM songs. You don’t want to risk them bumping into things or falling over. |

#### Danger Dash
|                            Abbildung                             |                           Editor-Ansicht                            | Erklärung                                                                                                                                                                                                                                                                                                    |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of danger dash](~@images/mapping/danger-dash.png) | ![Editor view of danger dash](~@images/mapping/danger-dash-alt.png) | Never force the player into the far edge of their playspace with 3-width walls or a 2-width wall in the middle. Walls that encompass the two middle columns gives the player very little room to play, and you don’t know how large their play area is or how far they will dash in response to these walls. |

#### Spam von Bomben
|                          Abbildung                           |                         Editor-Ansicht                          | Erklärung                                                                                                                                                                                                                                                                                 |
|:------------------------------------------------------------:|:---------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of bomb spam](~@images/mapping/bomb-spam.png) | ![Editor view of bomb spam](~@images/mapping/bomb-spam-alt.png) | Bombs are good for forcing precision, or for punctuating silence, but overuse of bombs should be avoided. Also note that most people hate bombs in general, so they should be used sparingly.<br /><br />**Note:** Precision bombs shouldn't be used more than once per beat. |

#### Kreuze
|                      Abbildung                       |                     Editor-Ansicht                      | Erklärung                                                                                                                                                                                                                                                                                                  |
|:----------------------------------------------------:|:-------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of cross](~@images/mapping/cross.png) | ![Editor view of cross](~@images/mapping/cross-alt.png) | This large, awkward pattern is difficult to read and can lead to smashed controllers, tangled arms, and ugly vision blocks. Players will likely not read it correctly the first time they see it, but even if they do, it’s not a satisfying motion anyway. Consider using a different pattern altogether. |

#### Versteckte Blöcke
|                               Abbildung                               |                              Editor-Ansicht                              | Erklärung                                                                                                                                                                                                                                                                           |
|:---------------------------------------------------------------------:|:------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of hidden blocks](~@images/mapping/stacked-hidden.png) | ![Editor view of hidden blocks](~@images/mapping/stacked-hidden-alt.png) | Blocks should never be stacked on top of one another or in walls. Any combination of blocks are technically stackable in the editor (including bombs and walls). Sometimes these are hard to spot if two identical blocks are stacked. Use the error checker in MMA2 to find these! |

#### Hitbox-Missbrauch
|                                Abbildung                                |                                    Editor-Ansicht                                    | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|:-----------------------------------------------------------------------:|:------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of some hitbox abuse](~@images/mapping/hitbox-abuse.png) | ![Alternate llustration of some hitbox abuse](~@images/mapping/hitbox-abuse-alt.png) | Leave room for the player to swing at each block. In the patterns depicted here, there is not enough room for the saber to slice each block without hitting the other. These are technically still possible to hit, but only by coming in at an angle, and if you have to come in at an angle, you may as well change the block direction to a diagonal anyway.<br /><br />The illustration below from Split, one of the game developers, shows the size of the block hitbox. The **large** outer box is for good hits and the small inner box is for bad hits.<br />![Illustration of block collider hitboxes](~@images/mapping/hitbox-from-split.jpg) |

#### Wide Precision
|                               Abbildung                                |                              Editor-Ansicht                               | Erklärung                                                                                                                                                     |
|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of wide precision](~@images/mapping/wide-precision.png) | ![Editor view of wide precision](~@images/mapping/wide-precision-alt.png) | These bombs are incredibly hard to avoid for players with short arms. When the player swings through these blocks, their arms come inward, and hit the bombs. |

### MAYBE: Sehr Situationsbedingte Patterns
These patterns are OK to use but only in very specific circumstances or with very specific setup. It’s best to steer clear of these until you’re much more comfortable with mapping.

#### Flicks
|                       Abbildung                        |                      Editor-Ansicht                       | Erklärung                                                                                                                                                                                                                                                                                                                                                                        |
|:------------------------------------------------------:|:---------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a flick](~@images/mapping/flick.png) | ![Editor view of a flick](~@images/mapping/flick-alt.png) | "Flicks" of two or more blocks of the same color at 1/4 precision are a difficulty spike, regardless of song tempo. It is the precision here that is important, not the patterns since these examples follow proper flow techniques. Even though flicks are more easily playable in lower tempo songs, they are incredibly difficult to use appropriately and should be avoided. |

#### Dreiecke
|                         Illustration                         |                           Editor View                           | Explanation                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:------------------------------------------------------------:|:---------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of a triangle](~@images/mapping/triangle.png) | ![Editor view of a triangle](~@images/mapping/triangle-alt.png) | Triangles are patterns that cause incredibly uncomfortable resets due to excession rotation in one direction. The pattern breaks the forehand/backhand mechanic. See the [Mapping with Flow](#do-mapping-with-flow) to revisit this explanation.<br /><br />**Note 1:** Not all triangle shaped patterns are cursed triangles. <br /><br />**Note 2:** This sort of pattern plays differently at Hard difficulties and below when there are a couple of beats between each swing but stay away at Expert and ExpertPlus. |

#### Incorrect Side Hits
|                                      Abbildung                                       |                                     Editor-Ansicht                                      | Erklärung                                                                                                                                                                                                                                                                                                                                 |
|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of upside down side hits](~@images/mapping/upside-down-side-hits.png) | ![Editor view of upside down side hits](~@images/mapping/upside-down-side-hits-alt.png) | Generally speaking, when making a double crossover, you should put RED on top when slicing left, and put BLUE on top when slicing right. This is a best practice because you don’t have to move your opposite hand as far. The exception is Expert/ExpertPlus, but  **only** if the flow of patterns leads to these placements naturally. |

#### Rapid Crossovers
|                               Illustration                                |                                 Editor View                                  | Explanation                                                                                                                                                                                                                                                                                                                                            |
|:-------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of rapid crossovers](~@images/mapping/rapid-crossover.png) | ![Editor view of rapid crossovers](~@images/mapping/rapid-crossover-alt.png) | Give the player time to prepare, and don’t make them cross sides too fast or too often. This pattern takes time to process and it’s a larger motion in-game than it looks in the editor. Also, never put this pattern in the top row. It's also recommended to offset the hits and put one of the two notes on the bottom row to reduce handclap risk. |

#### Wide Inward Doubles
|                                  Abbildung                                  |                                   Editor-Ansicht                                    | Erklärung                                                                                                                                                                                                                                                                                                             |
|:---------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of inward doubles](~@images/mapping/wide-inward-doubles.png) | ![Editor view of wide inward doubles](~@images/mapping/wide-inward-doubles-alt.png) | Inward facing double blocks on the edges or downward facing blocks on the top row are very difficult to hit for small/short players, and uncomfortable for the rest. This should generally be avoided. The exception is Expert/ExpertPlus, but  **only** if the flow of patterns leads to these placements naturally. |

#### Excessive Towers
|                                 Abbildung                                  |                                Editor-Ansicht                                 | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
|:--------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of excessive towers](~@images/mapping/excessive-towers.png) | ![Editor view of excessive towers](~@images/mapping/excessive-towers-alt.png) | Placing 3 blocks of the same color, vertically or horizontally, may seem fun, but you can achieve the same "hard hitting" effect with just 2. 3 feels excessive in-game. Even when using 2, don’t place anything directly behind them, since visibility will be low.<br /><br />At Expert/+ if you are going to use this for major emphasis, each block needs to be staggered after each other at 1/16 (<200 bpm) or 1>200 bpm) precision, turning this into what is known as a slider. |

#### Awkward Curves
|                                      Abbildung                                       |                                     Editor-Ansicht                                      | Erklärung                                                                                                                                                                                                                                                                                                                                                                    |
|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of awkward curved swings](~@images/mapping/awkward-curved-swings.png) | ![Editor view of awkward curved swings](~@images/mapping/awkward-curved-swings-alt.png) | Do not place two or more blocks of the same color together that do not face the same way. It is harder to read, feels awkward, and undermines the scoring system. Often, these patterns are used as a way to introduce flair to a map, but it’s really just a crutch for unimaginative mapping. Instead, add flair by introducing original patterns that flow well together. |

#### Detached Walls
|                               Abbildung                                |                              Editor-Ansicht                               | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of detached walls](~@images/mapping/detached-walls.png) | ![Editor view of detached walls](~@images/mapping/detached-walls-alt.png) | Combine your adjacent/ touching walls for a cleaner, less visually cluttered experience. Click and drag (left to right) to create walls wider than 1 column. Scroll to create walls shorter/longer than one beat (or whatever your cursor precision is set to) and click again to finish placing your wall. Don’t ever cover the entire grid with walls as depicted in the illustration. <br /><br />**Note:** This rule goes out the window when you get into wall mapping with Mapping Extensions, though this is NOT recommended for new mappers. |

#### Extended Crouch
|                                Abbildung                                 |                               Editor-Ansicht                                | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:------------------------------------------------------------------------:|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of extended crouch](~@images/mapping/extended-crouch.png) | ![Editor view of extended crouch](~@images/mapping/extended-crouch-alt.png) | Consider your target audience when using extended sections of top walls. You can't predict all players' physical ability, so use this in moderation. If you have notes immediately following a crouching section, make the starting direction UP, and consider visibility due to the player’s lower position.<br /><br />**Note:** Avoid placing blocks under a crouch wall, but if you must, always place them on the bottom row sides with horizontal slice directions (or dots). |

#### Corner Crouch
|                              Abbildung                               |                             Editor-Ansicht                              | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                   |
|:--------------------------------------------------------------------:|:-----------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of corner crouch](~@images/mapping/corner-crouch.png) | ![Editor view of corner crouch](~@images/mapping/corner-crouch-alt.png) | Consider your target audience when forcing the player to crouch in one corner. As stated above, crouching sections should be kept short because you can't predict all players' physical ability. Forcing the player to additionally move left/right while crouching increases the threshold of full-body range of motion. While this tactic may be fun for some, you don't want to ostracize the players that are incapable of this motion. |

#### Sky Streams
|                            Abbildung                             |                           Editor-Ansicht                            | Erklärung                                                                                                                                                                                                                                                  |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of sky streams](~@images/mapping/sky-streams.png) | ![Editor view of sky streams](~@images/mapping/sky-streams-alt.png) | Avoid repetitive use of blocks in the top row. This causes shoulder strain in addition to top row down notes being annoying to score well on.<br /><br />**Note:** Blocks on the top row in Easy and Normal should be dots and used sparingly. |

#### Visual Clutter
|                               Abbildung                                |                              Editor-Ansicht                               | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|:----------------------------------------------------------------------:|:-------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of visual clutter](~@images/mapping/visual-clutter.png) | ![Editor view of visual clutter](~@images/mapping/visual-clutter-alt.png) | Avoid unnecessary visual clutter. Having a directional block point towards/away from a dot block does not serve any functional purpose, and it’s hard to read at a glance. If you’re telling the player to slice in a particular direction, be consistent and make both blocks directional to increase readability.<br /><br />**Note:** At Expert/+ when making sliders it is common to start with an arrow then use dots afterward. |

#### Easy to Miss Patterns
|                                    Illustration                                    |                                      Editor View                                      | Explanation                                                                                                                                                                                                                                                                                                                                                                  |
|:----------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of overlapping hitboxes](~@images/mapping/overlapping-hitboxes.png) | ![Editor view of overlapping hitboxes](~@images/mapping/overlapping-hitboxes-alt.png) | Generally, try to avoid patterns with overlapping hitboxes, as this makes the pattern difficult to hit consistently. The hitboxes are larger than the note, and most players rarely hit the actual note when they swing, making it easy to hit the smaller hitbox within notes that detects bad hits on patterns like this. See [Hitbox Abuse](#hitbox-abuse) for more info. |

#### Arm Tangles
|                          Illustration                           |                            Editor View                             | Explanation                                                                                                                                                                                                                                                                                                                                                               |
|:---------------------------------------------------------------:|:------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of arm tangles](~@images/mapping/arm-tangle.png) | ![Editor view of arm tangles](~@images/mapping/arm-tangle-alt.png) | Crossing hands is usually fine, but crossing hands and going in opposite directions vertically causes the player’s arms to hit each other. Reverse these colors and you’re good to go. This is only one example of an arm tangle. Always be aware of where you're leaving your player's arms and how they are going to escape from that position to hit the next pattern. |

#### Face Punchers
|                              Editor View                               | Exaplanation                                                                                                                                                                                                                                                                                  |
|:----------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Editor view of a face puncher](~@images/mapping/facepuncher-alt.png) | Face punchers are blocks placed in the opposite top corners pointing outwards. This placement requires the player to perform a large crossover in a direction that potentially causes their controllers to smash into their headset. <br></br> **Never** use a double of face punchers. |

## Schwierigkeitsgrad Einschätzen & Down-Mapping

Many mappers tend to map the difficulty level at which they typically play, but there are plenty of benefits to mapping lower difficulties:

* Full spreads can be played and enjoyed by a wider audience.
* They look professional when cruising for new maps, just like the base game maps.
* Players who are good at the game can use your lower difficulties for training, such as accuracy players.

The difficulty of a map is comprised of a combination of *density* (rhythm choice), *complexity* (pattern choice), and *readability* (NJS and Offset). There should be a smooth progression as you work your way down from Expert+ to Easy. When building lower difficulties, it’s important to understand what skills players at different levels have and try to preserve the map's identity as you work your way down the spread.

For more information on mapping lower difficulties than what is on this page, check out [Downmapping](./downmapping.md).

### Pattern Complexity

Maps should always have a progression of complexity from Easy through Expert+. The difficulty of a map is typically rooted in its complexity, with a great deal of attention given to what a player would typically expect at a respective difficulty level.

:::tip Remember
You are teaching players different patterns and sight-reading skills with your maps. Make sure you give them time to
react before you throw something new at them at each level of difficulty.
:::

<!-- markdownlint-disable MD013 -->
| Difficulty | Pattern Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:----------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|  Expert+   | &#8227; Welcome to the wild west! You can throw any good mapping practices at your player here.<br />&#8227; Parity is expected at this level, especially for high BPM songs. Lower BPM songs may be more lenient but parity breaks are discouraged.<br />&#8227; Always be mindful of common errors, such as resets and vision blocks.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
|   Expert   | &#8227; All note directions are viable here in any proportion.<br />&#8227; All note positions viable here in any proportion. For patterns of wider spacing, give them enough reaction time and be mindful of the player’s stamina.<br />&#8227; Any color, any lane is fine. Crossovers should be used wisely and not combined with other weird patterns.<br />&#8227; Flow is critical. Parity will make or break your map.<br />&#8227; All emphasis options are on the table, including stacks and sliders.<br />&#8227; All obstacles are fair game, but be wary about creating vision blocks.                                                                                                                                                                                                                                                   |
|    Hard    | &#8227; All cardinal directions are viable. Occasional diagonals are fine, but give plenty of time to react and recover.<br />&#8227; All note positions viable here in any proportion. Top row notes are fine, but make sure the spacing is not tiring for the player.<br />&#8227; Any color, any lane is fine. Always provide enough reaction time before a *true* crossover where the player’s arms have to physically cross over each other.<br />&#8227; Flow is critical unless you have an extended break. Try to maintain parity with every swing.<br />&#8227; Most emphasis options are available, including inverted doubles with sabers going opposite directions. Stacks and sliders are fine, but keep them two notes long and don’t overuse them.<br />&#8227; All obstacles are fair game, but be wary about creating vision blocks. |
|   Normal   | &#8227; All cardinal directions are viable. Diagonals are not recommended for this level. All side notes should be treated as forehand hits.<br />&#8227; Notes should lie mostly in the bottom row. Use the middle row as a flourish for emphasis. Use the top row sparingly with dot notes only.<br />&#8227; Keep red notes primarily on the left side and blue on the right. Avoid crossovers entirely.<br />&#8227; Players will tend to reset after every hit, but you can introduce flow when the notes are too close together.<br />&#8227; Inverted doubles are manageable, but don't overuse them. Stacks and sliders should be scarce.<br />&#8227; If obstacles are used, they should be easy to avoid. You can sprinkle in notes simultaneously, but give plenty of time to react and recover.                                           |
|    Easy    | &#8227; All cardinal directions are viable. Diagonals are not recommended for this level. All side notes should be treated as forehand hits.<br />&#8227; Notes should mostly lie in the bottom row. Use the middle row as a flourish for emphasis. Use the top row sparingly with dot notes only.<br />&#8227; Keep red notes primarily on the left side and blue on the right. Avoid crossovers entirely.<br />&#8227; Knock yourself out with parity breaks. Players will reset after every hit.<br />&#8227; Avoid inverted doubles. Sliders and stacks are not recommended.<br />&#8227; If obstacles are used, they should be easy to avoid with no simultaneous notes.                                                                                                                                                                         |
<!-- markdownlint-enable MD013 -->

### Note Density

**NPS** is a measure of note density, or the number of notes measured within a certain interval of time. The NPS ranges for each difficulty will fluctuate depending on the map, but it is common to reduce the note density of each difficulty by **20%** or more as you work your way down the spread.

The table below provides a range of NPS values calculated from all base game maps, so you can use these values as a recommended baseline for where your values may lie. For more information on the typical NPS ranges across each of the base game maps, check out the [Beat Saber Map Analysis](https://docs.google.com/spreadsheets/d/13wyoviJAplYOrsMocOA7YNXJxVRHd74G7z4U2jhCZa4) spreadsheet.

| Schwierigkeit | NPS Ranges  |
|:-------------:|:-----------:|
|   **Easy**    | 0.82 - 2.20 |
|  **Normal**   | 1.05 - 3.22 |
|   **Hard**    | 1.73 - 4.24 |
|  **Expert**   | 2.42 - 6.49 |
|  **Expert+**  | 3.21 - 8.69 |

In general, the rhythm choices across the spread should fit the song. A 200 BPM speed map is going to have a higher note density than a 120 BPM dance map.

### Note Jump Speed

There are several terms related to the speed and readability of the map. These terms are all interrelated and are typically influenced by the song’s tempo:

* **Note Jump Speed** (NJS) is the rate at which blocks move down the track at the player. A higher value will make the notes move faster, while a lower value will make the notes move slower.
* **Jump Distance** (JD, also known as **Spawn Distance**) is a measure of the physical distance (in meters) that a note will travel to reach the player.
* **Half Jump Duration** (HJD) is a measure of time (in beats) from when a note spawns to when it reaches the player.
* **Spawn Distance Offset** (Offset, also known as **Spawn Distance Modifier**) is a modifier that directly affects the Jump Distance. A higher value will make the notes spawn further away from the player, while a lower value will bring the notes closer.

The following video demonstrates the effect of these values in-game:  
[YouTube](https://youtu.be/S70CDoWjdwk) | [Streamable](https://streamable.com/2l7fz9).

Changing the NJS or Offset values will modify the HJD and JD of your map. Community editors will show you how these values change as you make adjustments. Fine-tuned NJS and Offset are a matter of personal taste, so you may need to rely on trial and error to find values that work for you. For lower difficulties, always be wary about putting too many notes on-screen at once based on the values you choose.

The table below provides a range of NJS and JD values from typical community spreads, so you can use these values as a recommended baseline for where your values may lie.

| Difficulty  | NJS Ranges | JD Ranges |
|:-----------:|:----------:|:---------:|
|  **Easy**   |   10-12    |   27-30   |
| **Normal**  |   10-12    |   27-30   |
|  **Hard**   |   10-15    |   24-30   |
| **Expert**  |   12-18    |   24-27   |
| **Expert+** |   15-23    |   24-27   |

## Playtesting
Already mentioned in detail on the [Mapping Home Page](./#playtesting) it’s important enough to mention again here:

1. Test your own work early and often, especially when you’re just starting out!
2. If you can’t test your own work have a friend play it. Just remember that a friend may be more likely to say "that’s awesome, man!" than to give you honest advice and risk hurting your feelings... even if that’s what you need.
3. Even if you test your own work you can become "map blind" because you know it so well and may not see playability issues
4. Use the `#testplays` channel on BSMG wisely. There are experienced mappers who will play your pre-release map and provide constructive feedback. Sometimes there’s a LOT of constructive feedback and that’s ok. Those experienced mappers were once newbies with terrible maps themselves. If you’ve read and absorbed the info on this page you will be much better off!

**HAPPY MAPPING!** Visit `#mapping-discussion` on the BSMG Discord with questions!

## Credits
Content in this section has been derived from guides by [Awfulnaut](./mapping-credits.md#awfulnaut) and [Hexagonial](./mapping-credits.md#hexagonial).
