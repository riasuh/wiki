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

::: warning Sonderzeichen aus anderen Sprache wie Japanisch (日本語/にほんご), Kaomoji (٩(◕‿◕｡)۶), Chinesisch (汉语/漢語), Arabisch (اَلْعَرَبِيَّةُ‎), und Buchstaben mit Akzent (Ä/é/ó) werden nicht vollständig von BeatSaver unterstützt. Das Nutzen dieser Zeichen in den Metadaten oder in Lesezeichen kann zu Problemen führen. :::

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

::: danger Handgelenksrückstellungen sind, wenn du den Vorhand-/Rückhand Flow eines Musters mitten im Spiel änderst, so dass der Spieler sein Handgelenk abrollen muss, um den Flow zurückzustellen. Du kannst die normale menschliche Körpermechanik stören und die Spieler einem ernsthaften Risiko von Gelenkschäden aussetzen. Verwende keine Resets mit hoher Präzision! :::

Wenn zwischen den Noten längere Zeit verstreicht, wird der Spieler seine Armposition neu einstellen, so dass es oft besser ist, den neuen Abschnitt mit einem Abwärtsblock zu beginnen.  In zeitlichen Grauzonen, wie z. B. 3 Sekunden ohne Noten, liegt es am Mapper, den Spieler zurückzusetzen oder den Fluss fortzusetzen.

Möchten du mehr über Resets wissen? Lies [Intermediate Mapping](./intermediate-mapping.md)!

### DO: Mapping mit Flow
Außerhalb der leichten und normalen Schwierigkeiten ist das Mapping mit Flow ein absolutes Muss. Der menschliche Körper ist eine unglaubliche Maschine, aber es gibt bestimmte Bewegungsabläufe in den Gelenken und die Verwendung von Bewegungsmustern, die diese Mechanik verletzen, welches ein Rezept für die Verletzung des Spielers ist.

Parity ist das Konzept, dass jede Blockrichtung entweder mit einem Rückhand- oder einem Vorhandschwung gespielt wird. Die schwarze Linie im Diagramm unten veranschaulicht diese Unterscheidung zwischen Vorhand (unter der Linie) und Rückhand (über der Linie) für die linke und rechte Seite.

::: align center ![Parity diagram showing the forehand/backhand line for each block color](~@images/mapping/parity_diagram.jpg) :::

Beim Mapping mit Flow strebst du danach, diese Parity Linie immer mit einer möglichst natürlichen Bewegung zu überschreiten. Der Spieler sollte bei jedem Schlag immer zwischen Vorhand und Rückhand wechseln.

Dieses Video veranschaulicht die Grundlagen der Parity: [YouTube](https://youtu.be/tLQK4gN3bDc)

Eine wichtige Sache, die man im Auge behalten sollte, besonders wenn man neu im Spiel oder im Mapping ist, ist, dass das Konzept der Parity für Spieler aus dem Handgelenk am offensichtlichsten ist. Wenn du nicht so spielst, dass deine Handfläche direkt zum Boden zeigt, kannst du vielleicht nicht verstehen, warum manche Parity Umbrüche unangenehm sind. Denke daran, dass es sich für dich vielleicht gut anfühlt, aber Spieler haben unterschiedliche Griffe und Stile. Angemessene Parity ist für alle gut, nicht nur für bestimmte Spielstile.

::: tip  
Wenn der richtige Spielfluss erreicht ist, sollte der Spieler körperlich in der Lage sein, bei jedem Block die volle Punktzahl zu erreichen, auch wenn er nicht die Fähigkeit oder das Interesse hat, dies zu tun. Weitere Informationen findest du im [Scoring](/grips-and-tricks.md#scoring) Abschnitt des Wikis. :::

|                             0° Winkel                              |                              45° Winkel                              |                              90° Winkel                              |                              135° Winkel                               |                              180° Winkel                               |
|:------------------------------------------------------------------:|:--------------------------------------------------------------------:|:--------------------------------------------------------------------:|:----------------------------------------------------------------------:|:----------------------------------------------------------------------:|
| ![0 degree angle change between blocks](~@images/mapping/0deg.png) | ![45 degree angle change between blocks](~@images/mapping/45deg.png) | ![90 degree angle change between blocks](~@images/mapping/90deg.png) | ![135 degree angle change between blocks](~@images/mapping/135deg.png) | ![180 degree angle change between blocks](~@images/mapping/180deg.png) |
|                             Nein. (DD)                             |                              Nein. (DD)                              |                         Eventuell in E/N/H.                          |                                  Ja.                                   |                                  Ja.                                   |

**Grundlegende Flow-Konzepte:**

* Je höher deine Notenpräzision ist, desto eher solltest du dich an 180° (auf/ab) und 135° (auf/ab/diagonal) Muster halten.
* 90° Übergänge, die die Parity Linie kreuzen, sollten nur mit 1-2 Beats dazwischen in Betracht gezogen werden, mehr, wenn deine Map ein hohes Tempo hat. Vermeide 90° Übergänge bei Expert und ExpertPlus vollständig.
* Vergewisser dich, dass du das richtige Setup (das Muster unmittelbar davor) und das richtige Escape (das Muster unmittelbar danach) für einen komfortablen Schwung bei jeder Geschwindigkeit hast, die du abbilden willst.
* Achten auf dein Timing. Bei Tempo unter 160 BPM kannst du mit geringerer Notenpräzision mehr erreichen als bei Songs mit hohen BPM. Map für den von deinen gewählten Songstil.

### DON'Ts: Verbotene Patterns
Diese werden nicht ohne Grund als verbotene Pattern bezeichnet. Es gibt keinen Grund in der Welt, diese zu verwenden, da sie entweder für die Hardware des Spielers oder seine Gelenke gefährlich sind oder dem Punktesystem zuwiderlaufen. Du hast vielleicht Maps gespielt, die diese enthalten, aber das macht sie nicht gut.

#### Handclaps
|                              Abbildung                               |                             Editor-Ansicht                              | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
|:--------------------------------------------------------------------:|:-----------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a handclap](~@images/mapping/controller-smash.png) | ![Editor view of a handclap](~@images/mapping/controller-smash-alt.png) | Wenn man Blöcke aufeinander richtet, kann es passieren, dass der Spieler seine Controller zusammenschlägt, wenn er um maximale Punkte spielt. Tu es nicht, keine Ausnahmen.<br /><br />Hinweis: Verschiedene VR-Sets haben unterschiedliche Controller. Vive Wands sind viel größer als Oculus Touch Controller und Index Knuckles... gefährde nicht die Hardware deiner Spieler! *AKA Controller clash, Controller smash* <br /><br /> [Beispiel-Video](https://clips.twitch.tv/FantasticTenderTortoiseDancingBanana) |

#### Hammer Hits
|                            Abbildung                             |                           Editor-Ansicht                            | Erklärung                                                                                                                                                       |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a hammer hit](~@images/mapping/hammer-hit.png) | ![Editor view of a hammer hit](~@images/mapping/hammer-hit-alt.png) | Jeder Directional Block, der auf eine Bombe in der gleichen Ebene zeigt, ist einfach nur böse (und untergräbt das Punktesystem). Tue es nicht. Keine Ausnahmen. |

#### Entkörperte Noten
|                                  Abbildung                                   |                                 Editor-Ansicht                                  | Erklärung                                                                                                                                                                                                                                                     |
|:----------------------------------------------------------------------------:|:-------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of disembodied notes](~@images/mapping/disembodied-notes.png) | ![Editor view of disembodied notes](~@images/mapping/disembodied-notes-alt.png) | Verstecke keine Blöcke auf der anderen Seite (oder innerhalb) von Wänden. Meistens handelt es sich dabei um einfache Fehler, die die Leute nicht finden, weil sie ihre Maps nicht ausreichend testen (HINWEIS: [Playteste ](./#playtesting) deine Maps immer) |

#### Schnelles Wall Dodge
|                                 Abbildung                                  |                                Editor-Ansicht                                 | Erklärung                                                                                                                                                                                                                                                                                                                                                                            |
|:--------------------------------------------------------------------------:|:-----------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of rapid wall dodge](~@images/mapping/rapid-wall-dodge.png) | ![Editor view of rapid wall dodge](~@images/mapping/rapid-wall-dodge-alt.png) | Halte die Kopfbewegung langsam und vorhersehbar. Zwinge Spieler nicht, sich sehr schnell von einer Seite ihres Spielraums zur anderen zu bewegen. Wall Dodges sind in Ordnung (und machen Spaß!), aber erlaube *mindestens* 1,5 Schläge, damit der Spieler bei Liedern mit höherem BPM die Seite wechseln kann. Du willst nicht riskieren, dass sie an etwas anstoßen oder umfallen. |

#### Danger Dash
|                            Abbildung                             |                           Editor-Ansicht                            | Erklärung                                                                                                                                                                                                                                                                                                                           |
|:----------------------------------------------------------------:|:-------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of danger dash](~@images/mapping/danger-dash.png) | ![Editor view of danger dash](~@images/mapping/danger-dash-alt.png) | Zwinge den Spieler niemals an den äußersten Rand seines Spielraums mit einer 3-breiten Wand oder einer 2-breiten Wand in der Mitte. Walls, die die beiden mittleren Säulen umschließen, geben dem Spieler sehr wenig Spielraum, und man weiß nicht, wie groß sein Spielbereich ist oder wie weit er auf diese Walls reagieren wird. |

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
|                          Abbildung                           |                         Editor-Ansicht                          | Erklärung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
|:------------------------------------------------------------:|:---------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of a triangle](~@images/mapping/triangle.png) | ![Editor view of a triangle](~@images/mapping/triangle-alt.png) | Triangles are patterns that cause incredibly uncomfortable wrist resets  when used at high precision and speed. The pattern breaks the forehand/backhand mechanic and can injure your player. See the [Mapping with Flow](#do-mapping-with-flow) to revisit this explanation.<br /><br />**Note 1:** Not all triangle shaped patterns are cursed triangles. Make sure you are always crossing the parity line with each swing.<br /><br />**Note 2:** This sort of pattern plays differently at hard difficulties and below when there are a couple of beats between each swing but stay away at Expert and ExpertPlus. |

#### Incorrect Side Hits
|                                     Illustration                                     |                                       Editor View                                       | Explanation                                                                                                                                                                                                                                                                                                                               |
|:------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| ![Illustration of upside down side hits](~@images/mapping/upside-down-side-hits.png) | ![Editor view of upside down side hits](~@images/mapping/upside-down-side-hits-alt.png) | Generally speaking, when making a double crossover, you should put RED on top when slicing left, and put BLUE on top when slicing right. This is a best practice because you don’t have to move your opposite hand as far. The exception is Expert/ExpertPlus, but  **only** if the flow of patterns leads to these placements naturally. |

#### Rapid Crossovers
|                                 Abbildung                                 |                                Editor-Ansicht                                | Erklärung                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ![Illustration of rapid crossovers](~@images/mapping/rapid-crossover.png) | ![Editor view of rapid crossovers](~@images/mapping/rapid-crossover-alt.png) | Give the player time to prepare, and don’t make them cross sides too fast or too often. This pattern takes time to process and it’s a larger motion in-game than it looks in the editor. Also, never put this pattern in the top row. It's also recommended to offset the hits and put one of the two notes on the bottom row to reduce handclap risk. |

#### Wide Inward Doubles
|                                Illustration                                 |                                     Editor View                                     | Explanation                                                                                                                                                                                                                                                                                                           |
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
|                                     Abbildung                                      |                                    Editor-Ansicht                                     | Erklärung                                                                                                                                                                                                                                                                                                                                                                    |
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
Many mappers tend to map the difficulty level at which they play but there are plenty of benefits to mapping lower difficulties:

* Full spreads widen your audience leading to more downloads
* They look more professional when cruising for new maps... like official game maps

The actual difficulty level of a song is a combination of note density, pattern complexity, and note speed and spawn point. When down-mapping it’s important to understand what skills players at different levels have and how to use that information to develop a sense of progression in your levels.

### Relative Schwierigkeit
Maps should always have a progression of complexity from Easy through Expert+. The actual difficulty range of these levels in terms of note density has been creeping up since the game first came out.

While it’s best to stick within conventional ranges to start, as long as your levels have a clear progression of difficulty they don’t need to fit neatly into a box. If you’re only doing one difficulty you should stay within the expected range. Your map’s difficulty should fit the song - a 200 BPM Camellia song is going to be more challenging than a 120 BPM pop song.

::: align center ![A table of NPS values from official content](~@images/mapping/ost-extras-nps.png) :::

The above table of average notes per second (NPS) for the OST Extras shows how tracks like "What The Cat!?" are quite dense at the highest difficulty and the easy is also more dense than other easy levels. In each of these cases there is still a progression from Easy to ExpertPlus.

### Pattern-Komplexität
Map difficulty should come from pattern complexity with a great deal of attention given to how well they flow together. You might have a lower density expert, for example, that includes a lot of technical patterns that require more time to adequately sightread.

::: tip  
Remember that you are teaching players different patterns and sight reading skills with your maps. Make sure you give them time to react before you throw something new at them at each level of difficulty. :::

<!-- markdownlint-disable MD013 -->
| Difficulty | Pattern Notes                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|:----------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|    Easy    | &#8227; All cardinal directions (down, left, right, the occasional up)<br /> &#8227; Knock yourself out with DDs. Players will reset after every hit at this speed.<br />&#8227; Use up/down doubles for big emphasis if the music calls for it before or after a break.<br />&#8227; Blocks placed generally every other beat (depending on tempo)<br />&#8227; Very few obstacles, if any, which are easy to avoid with no simultaneous notes<br />&#8227; Almost all blocks should be in the bottom row. Use the middle row as a flourish for emphasis.Use the top row very sparingly with dot notes only<br />&#8227; Red stays in lanes 1 and 2, Blue stays in lanes 3 and 4                                                                                                                                                                                                                                                                                                                     |
|   Normal   | &#8227; All cardinal directions and the very occasional diagonal with lots of time to react and recover<br />&#8227; Begin to introduce up/down flow, especially anywhere you have notes that are close together, but DDs are still present especially after breaks<br />&#8227; Up/down and left/right doubles used for emphasis as appropriate<br />&#8227; Blocks generally placed every beat to two beats - mix it up a bit<br />&#8227; Keep your obstacles easy to avoid but start to introduce blocks sprinkled in with lots of time to react<br />&#8227; Almost all blocks still on the bottom row but higher use of middle row sides. Keep top notes rare and still as dots<br />&#8227; OK to let your red start drifting into lane 3 and your blues into lane 2 but still not crossing over each other                                                                                                                                                                                    |
|    Hard    | &#8227; All cardinal directions and limited diagonals with time to react<br />&#8227; Flow is now critical unless you have a break of 5+ beats. Try to cross the parity line with every swing.<br />&#8227; All doubles are fair game including inverted doubles with sabers going opposite directions, ok to start introducing stacks with plenty of reaction time<br />&#8227; Notes mostly every beat with some 1/2 beats and the occasional 1/4 thrown in with the rhythm.<br />&#8227; Keep 1/2 sections short, no more than 6-8 beats without a break. If a burst of 1/4 is used, keep it to 3-4 blocks with a break.<br />&#8227; All obstacles are fair game but make sure you are not creating vision blocks<br />&#8227; Mixing bottom, middle, and top rows with top notes transitioning from dots to directional blocks<br />&#8227; Any color, any lane is fine but give lots of reaction time before any occasional "true" crossover where the players arms have to cross to hit. |
|   Expert   | &#8227; Anything goes in expert but players are still improving sight reading skills. Keep patterns either fast and basic or slower and more technical... combine the two and you have an ExpertPlus!<br />&#8227; All note types viable here in any proportion<br />&#8227; Flow is critical; DDs will make or break your map<br />All emphasis options on the table including sliders with 1/16 or greater precision<br />&#8227; Mostly 1/2 beats with 1/4 mixed in to fit the rhythm. Make sure there is the occasional break in long streams.<br />&#8227; All obstacles are fair game but make sure you are not creating vision blocks.<br />&#8227; Expert introduces a lot more jumps,  though they still require enough reaction time<br />&#8227; Crossovers should be used wisely and not combined with other weird patterns.                                                                                                                                                        |
| ExpertPlus | &#8227; Welcome to the wild wild west! You can throw any good mapping practices at your player here.<br />&#8227; At high tempo and note density, patterns you could use effectively at hard and maybe expert start to become cursed. Players are often using their wrists instead of arm movements so body mechanics change at this level.<br />&#8227; Breaking the parity line with every swing is now crucial. You will get skewered if you don’t<br />&#8227; Stay away from triangles, DDs, and VBs.<br />&#8227; Be careful of sudden speed increases from 1/4 precision gallops and 1/4 single hand hits (flicks).                                                                                                                                                                                                                                                                                                                                                                                        |
<!-- markdownlint-enable MD013 -->

### Notendichte
Notes per Second is a measure of note density - how many notes does the player have to hit in a certain amount of time. The values below are from the [OST Analysis Spreadsheet](https://drive.google.com/open?id=13wyoviJAplYOrsMocOA7YNXJxVRHd74G7z4U2jhCZa4) which shows NPS ranges for all OST, Extras, and DLC content.

| Difficulty | Notes per Second                            |
|:----------:|:------------------------------------------- |
|    Easy    | 0.8 - 2.2 NPS                               |
|   Normal   | 1.1 - 3.2 NPS                               |
|    Hard    | 1.7 - 4.2 NPS                               |
|   Expert   | 2.4 - 6.5 NPS (yes, you read that right)    |
| ExpertPlus | 3.2 - 8.7 NPS (no upper limit here, really) |

### Note Jump Speed
There are several terms related to how the speed of gameplay feels. These are all interrelated and modified by the song’s tempo:

* **Note Jump Speed (NJS)** ist die Geschwindkeit, mit der die Noten auf den Spieler zukommen. Je höher die Zahl ist, desto schneller sind die Blöcke.
* **Jump Distance** (also known as **Spawn Distance**) is how far down the track the blocks will spawn in distance (meters).
* **Half Jump Duration** is how far in advance blocks appear in time (beats).
* **Spawn Distance Offset** (also known as **Spawn Distance Modifier**) is a modifier which increases the jump distance. This can make the NJS feel slower since the blocks will spawn further away and the player has more time to react.

Summary video demonstrating the effect of these values in-game: [YouTube](https://youtu.be/S70CDoWjdwk), [Streamable](https://streamable.com/2l7fz9).

Changing the NJS or Offset values will modify the half jump and jump distance. Community editors will show you how these values change when making adjustments. Fine-tuned NJS and offset are a matter of personal taste but try to hit a half jump of 2 or 3 beats and a jump distance of 26-30 meters.

::: warning Jump distance should run on the higher end of this range for expert and lower difficulties. Very dense ExpertPlus maps often have very short jump distances to minimize clutter. :::

| Schwierigkeit | Note Jump Speed Range |
|:-------------:|:--------------------- |
|     Easy      | 10 NJS                |
|    Normal     | 10 NJS                |
|     Hard      | 12-14 NJS             |
|    Expert     | 14-16 NJS             |
|  ExpertPlus   | 16+ NJS               |

When mapping very fast Expert+ maps, make sure you increase the Note Jump Speed, though you shouldn’t need to go higher than 22. This will make the notes come at the player faster with more space in between them, increasing readability.

::: warning NOTE  
Setting your NJS really high is **not** the right way to increase difficulty. Use higher note density and more complex patterns (with good flow). :::

For more information, see the [Note Jump Speed & Jump Distance](./intermediate-mapping.md#note-jump-speed-jump-distance) section in [Intermediate Mapping](./intermediate-mapping.md).

## Playtesting
Already mentioned in detail on the [Mapping Home Page](./#playtesting) it’s important enough to mention again here:

1. Test your own work early and often, especially when you’re just starting out!
2. If you can’t test your own work have a friend play it. Just remember that a friend may be more likely to say "that’s awesome, man!" than to give you honest advice and risk hurting your feelings... even if that’s what you need.
3. Even if you test your own work you can become "map blind" because you know it so well and may not see playability issues
4. Use the `#testplays` channel on BSMG wisely. There are experienced mappers who will play your pre-release map and provide constructive feedback. Sometimes there’s a LOT of constructive feedback and that’s ok. Those experienced mappers were once newbies with terrible maps themselves. If you’ve read and absorbed the info on this page you will be much better off!

**HAPPY MAPPING!** Visit `#mapping-discussion` on the BSMG Discord with questions!

## Credits
Content in this section has been derived from guides by [Awfulnaut](./mapping-credits.md#awfulnaut) and [Hexagonial](./mapping-credits.md#hexagonial).
