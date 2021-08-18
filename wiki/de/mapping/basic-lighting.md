---
sidebar: auto
prev: ./basic-mapping.md
next: ./intermediate-lighting.md
description: Lerne, wie du deine Map manuell zum leuchten bringen kannst!
---

# Lighting-Grundlagen
_Machen Beat Saber zu einem helleren Ort, indem Du Deine Maps manuell beleuchtest._

* [Glossar der Begriffe](./glossary.md)

---

Jede Karte muss eine Art von Beleuchtung haben. Wenn Du die Dir zur Verfügung stehenden Werkzeuge kennst, kann eine einfache manuelle Beleuchtung sehr einfach sein. [Dieser Link](https://streamable.com/s/x7zj0/vrugyj) ist ein Videobeispiel für eine sehr einfache manuelle Beleuchtung

::: tip HINWEIS Das Beispiel verwendet [Map Color Overrides](#map-color-overrides). Du musst kein AaltopahWi oder Skeelie sein, um tolle Beleuchtung zu machen! :::

## Beleuchtungsarten
Die verfügbaren Beleuchtungstypen sind in jeder der eingebauten Spielumgebungen gleich, Diese können sich jedoch an leicht unterschiedlichen Positionen befinden oder in einigen Fällen nicht vorhanden sein.

* **Zentrumslichter:** Allgemeine Lichter entlang der Seite der Schiene, unterhalb der Schiene und manchmal ein Chevron an der Rückseite der Schiene. Manchmal auch "Bottom/Back/Side"- oder "BBS"-Leuchten genannt.
* **Seiten/Aufsatzlaser:** Sätze von rotierenden Lasern an den Seiten der Strecke oder oberhalb/unterhalb der Strecke, je nachdem, welche Umgebung Du ausgewählt hast. Die Rotation wird mit der Funktion Lasergeschwindigkeit eingestellt.
* **Hintergrundlaser:** Statische Laser, oft in einem "X"-Muster am hinteren Teil der Strecke, hinter dem Chevron.
* **Ringlichter:** Lichter, die an der Innenseite der großen Außenringe angebracht sind, die sich in fast allen Umgebungen drehen.
* **Ringdrehungen:** Wird verwendet, um Bewegung in den Ringen zu erzeugen. In Umgebungen mit einem inneren und einem äußeren Ring, beide Ringe drehen sich gemeinsam.
* **Ring Zooms:** Wird verwendet, um den inneren Ring in Umgebungen, die ihn haben, zu zoomen und zu entzoomen. Hat keinen Einfluss auf den Außenring.
* **Lasergeschwindigkeit:** Ändert die Geschwindigkeit der Rotation des Seitenlasers von stationär (0) bis sehr schnell (20). Unabhängig für den rechten und linken Seitenlaser einstellen. Back-Top Laser bewegen sich nicht. Die Lasergeschwindigkeit steigt linear an, so dass **2** doppelt so schnell ist wie **1** und **5** ist fünfmal so schnell wie **1**.
* **Boost-Ereignis:** Ändert Beleuchtungsfarben zwischen zwei Farbpaaren. Aus verwendet er das erste Paar von Farben. An verwendet er das zweite (Boost-)Farbpaar. Für dieses Ereignis gibt es keine Überblend- oder Blitzoption.

## Lighting Events
Jeder Beleuchtungstyp kann vier verschiedene Beleuchtungsereignisse nutzen.

* **An:** Schaltet ein Licht ein, das eingeschaltet bleibt, bis du einen anderen Ereignistyp platzierst.
* **Aus:** Das Ausschalten eines Lichts kann die gleiche Wirkung haben wie das Einschalten, oder sogar mehr.
* **Blinken:** Blinkt kurz heller als ein Standard-Ereignis "Ein" und bleibt dann an, bis du einen anderen Ereignistyp platzierst.
* **Abblenden:** Blinkt kurz heller als ein Standard "Ein"-Ereignis und wird dann nach ein paar Sekunden ausgeblendet.

::: warning HINWEIS  
Es ist nicht möglich, die Dauer einer Ausblendung zu steuern oder eine Einblendung mit Standardbeleuchtung zu verwenden. Für benutzerdefinierte Überblendzeiten ist Chroma erforderlich, das im Abschnitt "Erweiterte Beleuchtung" (Kommt bald) behandelt wird. :::

## Bewährte Praktiken & Techniken
> "The only bad lights are **NO** lights.... or lightmap."  
> ~ Skeelie

Beleuchtung ist eine Kunst, was bedeutet, dass sie viel subjektiver ist als Mapping. Es gibt relativ wenige Best Practices für den Einstieg und eine einfache manuelle Beleuchtung ist fast unmöglich, schlecht zu machen.

**TranquillizeMe** hat ein Beleuchtungs-Tutorial erstellt, [Beat Saber Lighting Techniques Tutorial](https://www.youtube.com/watch?v=EDbPRN_u3jc), in dem nützliche Beleuchtungstechniken und allgemeine Tipps zur Beleuchtung beschrieben werden.

::: warning NOTE  
Die Beleuchtungsvorschau ist in den derzeit verfügbaren Editoren nicht realistisch, daher ist es wichtig, dass du deine Lichter oft im Spiel überprüfst. Unter [Previewing Your Lights](#vorschau-der-lichter) findest du einige Tools, die dir dabei helfen können. :::

### Tastenbelegung
Jeder Map-Editor handhabt die Beleuchtung anders, daher sollte man sich mit den Tastenbelegungen und der Funktionsweise der Platzierung im Editor der Wahl vertraut machen. Die Tastenkombinationen für die Beleuchtung variieren je nach Editor. Konsultiere den User Guide oder die Readme Datei des Editors oder lies diese hilfreiche Liste [Editorübergreifende Tastaturbelegungen](./editor-keybinds.md).

### Licht-Ereignisse zuweisen
Mapper, die ihre erste Map beleuchten, sollten damit beginnen, bestimmten [Beleuchtungstypen](##beleuchtungtypen) Instrumenten zuzuordnen, und dann mit zunehmender Erfahrung von dort aus weitergehen. Diese Methode führt normalerweise nicht zu den aufregendsten Shows, aber es ist schwer, es zu vermasseln. Das könnte so aussehen:

* **Track Lights:** Bass oder Kick Drum
* **Lasers:** Melodie
* **Ring Lights:** Synth A oder Cymbals
* **Ring Zoom:** Synth B

Sobald diese Art von Grundstruktur vorhanden ist und du mit der Funktionsweise vertraut bist, kannst du darüber nachdenken, an welchen Stellen du etwas ändern möchtest, um Akzente zu setzen. Die Festlegung eines strengen Musters ist notwendig, um eine Wirkung zu erzielen, wenn du eine Änderung vornimmst; wenn du alles betonst, betonst du nichts(das gilt auch für die Blockplatzierung!).

#### Ein Beispiel von Lighting Mentor, LittleAsi
> Normalerweise beleuchte ich die Melodie mit allen drei Lasern (Gesang und Instrumental auf verschiedenen Farben, oder primäres Instrumental und Akzente auf einer anderen Farbe), das Schlagzeug auf den Ringlichtern und entweder den Bass oder etwas Harmonisches wie Synthesizer auf dem Bottom/Back/Side (BBS) (manchmal ein bisschen viel, da die BBS-Intensität erhöht wurde). Wenn das Schlagzeug zu aufwendig ist, um es allein auf die Ringleuchten zu packen, oder es nichts anderes Passendes für die BBS gibt, verschiebe ich die Kick Drum auf die BBS. Wenn die Trommeln wirklich dominant sind, würde ich vielleicht den Back-Top-Laser auf Snare-Betrieb setzen, um die Ringlichter den Becken zu widmen. Die zahlreichen Möglichkeiten, das Verhalten und Aussehen von Lasern zu verändern, machen sie jedoch zum besten Kandidaten für die Melodieverfolgung. Ich habe jedoch Laser der Geschwindigkeit 0 für die geschlossene Hi-Hat und verschiedene Geschwindigkeiten für die offene Hi-Hat und Becken-Crashs verwendet. Es muss also definitiv nicht auf eine bestimmte Art und Weise sein (nur intern konsistent).

### Lasergeschwindigkeit zurücksetzen
Wenn du die gleiche Lasergeschwindigkeit zweimal hintereinander anwendest, wird sie auf eine zufällige Position zurückgesetzt. Wenn du z. B. bei jedem Snare-Treffer die Geschwindigkeit 1 einstellst, werden die Laserpositionen im Takt der Snare zufällig verändert, ohne dass sich ihre Rotationsgeschwindigkeit ändert.

Wenn du die Lasergeschwindigkeit nicht zurücksetzt, dreht er sich so lange konstant mit dieser Geschwindigkeit, bis sie geändert wird.

### Off Event Placement
Die Sounds innerhalb eines Songs haben selten einen genauen Endpunkt, so dass es nicht immer einen "richtigen" Zeitpunkt gibt, um das `Off` Ereignis zu platzieren. Achte darauf, wann du Lichter, die mit bestimmten Sounds oder Instrumenten verbunden sind, ausschaltest, und wende diese Entscheidungen konsequent im gesamten Song an.

Sei vorsichtig, wenn du Ereignisse genau in der Mitte von zwei Leuchten absetzt, da dies manchmal einen unbeabsichtigten Stroboskopeffekt erzeugen kann.

## Standard Umgebungen
In Beat Saber gibt es verschiedene eingebaute Umgebungen, die Teil des Basisspiels sind und mit wenigen Klicks genutzt werden können.

::: warning HINWEIS Von der Community erstellte benutzerdefinierte Umgebungsmodelle (Plattformen) existieren, erfordern jedoch die Mod "Custom Platforms", die derzeit nicht über den Mod Assistant verfügbar ist. Eine Beta-Version kann im `#pc-mods` Kanal des BSMG-Discord verfügbar sein. :::

Die Grundstruktur jeder Umgebung ist meist gleich. Im [Mediocre Map Assistant 2](./mediocre-map-assistant.md) Editor sieht die Beleuchtungsspur wie folgt aus:

::: align center ![Screenshot of the MMA2 lighting track from the top down](~@images/mapping/mma2-lighting-track.jpg) :::

### Umgebungs-Vorschau
|         Video und Screenshot (Anklicken zum Öffnen in voller Größe)         | Umgebung                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|       ![Bild der Standard Umgebung](~@images/mapping/default_env.jpg)       | **Das erste (Standard) Environment**<br />**Info.dat Name:** `DefaultEnvironment` <br />**Standard Farbe:** Red & Blue<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: (Beide Quadrate) <br />**Ring Zoom:** :white_check_mark: (Inneres Quadrat)<br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Ab 1.6 sind die Back Top Laser unter den Track Lasern <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/lUnmb1vx_do)                                                                                                                                                                                                                                                                    |
|      ![Bild der Ursprungs Umgebung](~@images/mapping/origins_env.jpg)       | **Origins Environment**<br />**Info.dat Name:** `OriginsEnvironment`<br />**Standard Farben:** Gelb & Pinke Noten, Blau & Hellblaue Lichter<br /><br />**Laser:** :white_check_mark:<br />**Ring Spin:** :white_check_mark:<br />**Ring Zoom:** :x:<br />**Equalizer:** :white_check_mark: <br /><br /> **Video Vorschau:** [YouTube](https://youtu.be/eo_4i4x_I9I)                                                                                                                                                                                                                                                                                                                                                                                                  |
|      ![Bild der Triangle Umgebung](~@images/mapping/triangle_env.jpg)       | **Triangle Environment**<br />**Info.dat Name:** `TriangleEnvironment`<br />**Standard Farben:** Rot & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: (Quadrat und Dreieck) <br />**Ring Zoom:** :white_check_mark: (Dreieck)<br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Ab 1.6 sind die Back Top Laser unter den Track Lasern <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/fBOYx6o-BAc)                                                                                                                                                                                                                                                                                  |
|          ![Bild der Nice Umgebung](~@images/mapping/nice_env.jpg)           | **Nice Environment**<br />**Info.dat Name:** `NiceEnvironment`<br />**Standard Farben:** Rot & Blau<br /><br />**Laser:** :white_check_mark: (Oben & Unten)<br />**Ring Spin:** :white_check_mark: (Beides Quadrate)<br />**Ring Zoom:** :white_check_mark: (Inneres Quadrat)<br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Ab 1.6 sind die Back Top Laser unter den Track Lasern <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/jwcbMbmurZg)                                                                                                                                                                                                                                                                                         |
|    ![Bild der Big Mirror Umgebung](~@images/mapping/big-mirror_env.jpg)     | **Big Mirror Environment**<br />**Info.dat Name:** `BigMirrorEnvironment`<br />**Standard Farben:** Rot & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts )<br />**Ring Spin:** :white_check_mark: <br />**Ring Zoom:** :x:<br />**Equalizer:** :white_check_mark: <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/dDLDerkwrWY)                                                                                                                                                                                                                                                                                                                                                                                                             |
|   ![Bild der Imagine Dragons Umgebung](~@images/mapping/dragons_env.jpg)    | **Imagine Dragons Environment**<br />**Info.dat Name:** `DragonsEnvironment`<br />**Standard Farben:** Rot & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: (Quadrat und Spirale)<br />**Ring Zoom:** :white_check_mark: (Spirale)<br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Back Top Laser Position sind die beiden Schienen an den äußeren Rändern des Bildschirms. Es leuchtet immer die entgegengesetzte Farbe dessen, was du eingestellt hast. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/3yQAB6ghwR4)                                                                                                                                                            |
|           ![Bild der K/DA Umgebung](~@images/mapping/kda_env.jpg)           | **K/DA Environment**<br />**Info.dat Name:** `KDAEnvironment`<br />**Standard Farben:** Orange & Lila<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :x:<br />**Ring Zoom:** :x:<br />**Equalizer:** :x:<br />**Hinweis:** Die Position Ringlicht beleuchtet die fünf Schienen an der Oberseite. Die Lichter in der Mitte der Pfeile gehen nie aus. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/tCAn5XAwmOc)                                                                                                                                                                                                                                                                                                         |
|    ![Bild der Monstercat Umgebung](~@images/mapping/monstercat_env.jpg)     | **Monstercat Environment**<br />**Info.dat Name:** `MonstercatEnvironment`<br />**Standard Farben:** Rot & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark:<br />**Ring Zoom:** :x: <br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Ab 1.6 befinden sich die Back-Top-Laser unterhalb der Track-Laser. Die Ringlichter beleuchten die fünf Schienen an der Oberseite. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/RNMDtNnYIRs)                                                                                                                                                                                                                                                   |
|     ![Bild der Crab Rave Umgebung](~@images/mapping/crab-rave_env.jpg)      | **Crab Rave Environment**<br />**Info.dat Name:** `CrabRaveEnvironment`<br />**Standard Farben:** Grün & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark:<br />**Ring Zoom:** :x: <br />**Equalizer:** :white_check_mark: <br />**Hinweis:** Ab 1.6 befinden sich die Back-Top-Laser unterhalb der Track-Laser. Die Ringlichter beleuchten die fünf Schienen an der Oberseite. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/gph2cICsN-M)                                                                                                                                                                                                                                                    |
|  ![Bild der Panic! at the Disco Umgebung](~@images/mapping/panic_env.jpg)   | **Panic! at the Disco Environment**<br />**Info.dat Name:** `PanicEnvironment`<br />**Standard Farben:** Rot & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: <br />**Ring Zoom:** :white_check_mark: <br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Ringlichter sind in dieser Umgebung viel heller als in anderen. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/MAVxsDe53a4)                                                                                                                                                                                                                                                                                               |
|     ![Bild der Rocket League Umgebung](~@images/mapping/rocket_env.jpg)     | **Rocket League Environment**<br />**Info.dat Name:** `RocketEnvironment`<br />**Standard Farben:** Orange & Blau<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :x:<br />**Ring Zoom:** :x:<br />**Equalizer:** :x: <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/C6bDsdNTRVk)                                                                                                                                                                                                                                                                                                                                                                                                                                              |
|     ![Bild der Green Day Umgebung](~@images/mapping/green-day_env.jpg)      | **Green Day Environment**<br />**Info.dat Name:** `GreenDayEnvironment`<br />**Standard Farben:** Grün & Türkis<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: <br />**Ring Zoom:** :white_check_mark:<br />**Equalizer:** :x:<br />**Video Vorschau:** [YouTube](https://youtu.be/S0dySYgBMMg)                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ![Bild der Green Day Grenade Umgebung](~@images/mapping/gd-grenade_env.jpg) | **Green Day Grenade Environment**<br />**Info.dat Name:** `GreenDayGrenadeEnvironment`<br />**Standard Farben:** Grün & Türkis<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :x:<br />**Ring Zoom:** :x: <br />**Equalizer:** :x:<br />**Video Vorschau:** [YouTube](https://youtu.be/qjHweeAM3NI)                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|     ![Bild der Timmaland Umgebung](~@images/mapping/timbaland_env.jpg)      | **Timbaland Environment**<br />**Info.dat Name:** `TimbalandEnvironment`<br />**Standard Farben:** Grau & Blaue Noten, Blaue & Blaue Lichter(Gleiche Farben)<br /><br />**Laser:** :white_check_mark: (Links & Rechts Lichter parallel zu den Ringen)<br />**Ring Spin:** :white_check_mark: <br />**Ring Zoom:** :white_check_mark: <br />**Equalizer:** :white_check_mark:<br />**Hinweiss:** Der "Timbaland" Schriftzug an den Seiten schaltet sich nie aus. Die Lasergeschwindigkeit wirkt sich auf die Back-Top Laser am linken und rechten Ring aus. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/cU2IS4m-U4Q)                                                                                                                           |
|       ![Bild der FitBeat Umgebung](~@images/mapping/fitbeat_env.jpg)        | **FitBeat Environment**<br />**Info.dat Name:** `FitBeatEnvironment`<br />**Standard Farben:** Gelbe & Pinke Noten, Orange & Blaue Lichter<br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: (Äußere Laser und Spirale) <br />**Ring Zoom:** :white_check_mark: (Spirale) <br />**Equalizer:** :white_check_mark: <br />**Hinweis:** Back-Top-Laser leuchten in der entgegengesetzten Farbe, die man einstellt. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/9Tg9ordcCi0)                                                                                                                                                                                                                       |
|   ![Bild der Linkin Park Umgebung](~@images/mapping/linkin-park_env.jpg)    | **Linkin Park Environment**<br />**Info.dat Name:** `LinkinParkEnvironment`<br />**Standard Farben:** Rot & Blau-Graue Noten, Beige & Weiße Lichter, Orange & Blaue Boost-Lichter <br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: (steuert die Laserausbreitung) <br />**Ring Zoom:** :x: <br />**Equalizer:** :white_check_mark: (An der Seitenwand) <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/ViZa0LWc8Ro) <br /> **Offizielles Showcase& Tutorial**: [YouTube](https://youtu.be/BhMQ8KS2rZk)                                                                                                                                                                                             |
|           ![Bild der BTS Umgebung](~@images/mapping/bts_env.jpg)            | **BTS Environment**<br />**Info.dat Name:** `BTSEnvironment`<br />**Standard Farben:** Pinke & Lila Noten, Pinke & Lila Lichter, Hellrosa & Hellblaue Booster-Lichter <br /><br />**Laser:** :white_check_mark: (Links & Rechts)<br />**Ring Spin:** :white_check_mark: (Hintergrundpfeiler) <br />**Ring Zoom:** :white_check_mark: (Gleispfeiler) <br />**Equalizer:** :x: <br />**Hinweis:** Das BTS-Logo in der Mitte schaltet sich nie aus.<br /><br />**Video Vorschau:** [YouTube](https://youtu.be/jb49cCmGKDo) <br /> **Offizielles Showcase & Tutorial**: [YouTube](https://youtu.be/HYnVROsLBBs)                                                                                                                                              |
|  ![Bild der Kaleidoscope Umgebung](~@images/mapping/kaleidoscope_env.jpg)   | **Kaleidoscope Environment**<br />**Info.dat Name:** `KaleidoscopeEnvironment`<br />**Standard Farben:** Rot & Schwarze Noten, Rot & Weiße Lichter, Rot & Magenta Booster-Lichter<br /><br />**Laser:** :white_check_mark: <br />**Ring Spin:** :white_check_mark:<br />**Ring Zoom:** :white_check_mark:<br />**Equalizer:** :x:<br /><br />**Video Vorschau:** [YouTube](https://youtu.be/4f8CLg77PCo) <br /> **Offizielles Showcase & Tutorial**: [YouTube](https://youtu.be/eZBd7-yb284)                                                                                                                                                                                                                                                                   |
|    ![Bild der Interscope Umgebung](~@images/mapping/interscope_env.jpg)     | **Interscope Environment**<br />**Info.dat Name:** `InterscopeEnvironment`<br />**Standard Farben:** Gelbe & Pinke Noten, Lila  & Weiße Lichter, Kühle Rote & Kühle Weiße Booster-Lichter<br /><br />**Laser:** :white_check_mark: <br />**Ring Spin:** :white_check_mark: (Autos) <br />**Ring Zoom:** :white_check_mark: (Autos und zusätzliche Laserstreuung) <br />**Equalizer:** :white_check_mark:<br />**Hinweis:** Dies ist die erste Umgebung, in der die Ereignisse 6, 7, 16 und 17 genutzt werden. 6 und 7 steuern zusätzliche Lichter. 16 und 17 steuern die Fahrkorbhydraulik. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/ILILJHnSg_U)<br /> **Offizielles Showcase & Tutorial**: [YouTube](https://youtu.be/GmJpF2VA-6E) |
|  ![Bild der Glass Desert Umgebung](~@images/mapping/glass-desert_env.jpg)   | **Glass Desert Environment**<br />**Info.dat Name:** `GlassDesertEnvironment`<br />**Standard Farben:** Gelbe & Pinke Noten, Blaue & Hellblaue Lichter<br /><br />**Laser:** :white_check_mark: <br />**Ring Spin:** :x:<br />**Ring Zoom:** :x:<br />**Equalizer:** :white_check_mark:<br />**Hinweis :** Dies ist die erste 360&deg; Umgebung. 360 Grad Levels MÜSSEN dies verwenden. Für Standard Levels ist es nicht verwendbar. Die Ringlichtposition steuert die horizontale Außenschiene. Back Top Laserposition steuern die sechs Schienen an der Oberseite. <br /><br />**Video Vorschau:** [YouTube](https://youtu.be/3jUYN8Di-gU)                                                                                                                     |

### Einstellen deiner Umgebung
Neue Standardumgebungen werden relativ häufig verfügbar, was bedeutet, dass Map-Editoren nicht immer die vollständige Liste zur Verfügung haben. Wenn die Umgebung, die du verwenden willst, nicht in den Einstellungen deiner bevorzugten Editors enthalten ist, musst du deine `Info.dat` Datei bearbeiten, um den Umgebungsnamen hinzuzufügen.

1. Entscheide , welche Umgebung du verwenden willst, und kopiere dann den Namen der `Info.dat` aus dem obigen Abschnitt [Umgebungsvorschauen](#umgebungs-vorschau).
2. Öffne deine `Info.dat`-Datei in einem Texteditor deiner Wahl.
3. Scrolle nach unten bis zum `"_environmentName":`Abschnitt.
4. Füge den Namen ein, den du in Schritt 1 kopiert hast.

> **HINWEIS:** Du kannst in diesem Feld keine eigene Plattform verwenden. Dies wird in [Erweiterte Beleuchtung](./advanced-lighting.md###benutzerdefinierte-umgebung) behandelt.

## Map Farbe überschreiben
Du kannst dein eigenes Farbschema für die Map im Game erzwingen, solange der Benutzer die SongCore-Mod installiert und die Option `Enable Custom Song Colors` in den Mod-Einstellungen aktiviert hat.

Seit Beat Saber Version 1.4 können Benutzer die Rot/Grün/Blau (RGB)-Farben von Noten, Lichtern und Wänden für ihr Spiel einstellen. Sie werden jedoch durch die in der `Info.dat` definierten Farben überschrieben, wenn der Benutzer die Option `Benutzerdefinierte Songfarben aktivieren` aktiviert hat.

::: tip Bei der Auswahl von Farbüberlagerungen für die Noten. Es wird **HÖCHSTENS** empfohlen, rötliche/warme/aggressive Farben auf der linken Seite und bläuliche/kalte/weiche Farben auf der rechten Seite zu verwenden, um die Spieler nicht zu verwirren. :::

Unter [Umgebungs-Standardfarben](./lighting-defaults.md) findest du eine Liste der in den Umgebungen verwendeten Standardfarben.

[Beatmapper](./#beatmapper-app), [ChroMapper](./#chromapper-coming-soon), und [MMA2](./#mediocre-map-assistant-2) unterstützen nativ Farb-Überschreibungen. Weitere Informationen findest du in den jeweiligen Handbüchern.

### Manuelles Hinzufügen von Farb-Überschreibungen

1. Entscheide, welche RGB-Farben die Notizen und/oder Lichter und/oder Wände haben sollen. Verwende ein Farbschema-Dienstprogramm wie [Paletton](https://paletton.com/#uid=1000u0kllllaFw0g0qFqFg0w0aF), um komplementäre Farben zu finden.
   * Deine Rot-, Grün- und Blauwerte müssen von der normalen Skala 0-255 in die Skala 0-1 umgewandelt werden. Verwende eine Website wie [EasyRGB](https://www.easyrgb.com/en/convert.php), um die Werte umzurechnen.
2. Öffnen die `Info.dat` Datei im Texteditor deiner Wahl
3. Blättere nach unten zum `"_customData": {` Abschnitt der Schwierigkeit, die du einfärben möchtest.
    * Die Verwendung der globalen `"_customData": {` außerhalb des `"_difficultyBeatmapSets": ` Arrays funktioniert möglicherweise nicht wie erwartet.
4. Füge die Codeblöcke ein, die den Farben entsprechen, die du innerhalb der geschweiften Klammern `_customData` erzwingen möchtest (`{` und `}`), und ersetze dann die Werte `"r":`, `"g":` und `"b":` durch die in Schritt 1 gewählten Werte.
   * Die Werte `"r":` und `"g":` **müssen** mit Kommas versehen werden.

In den Zeilen 29-60 und 69-100 dieses [Pastebin-Clips](https://pastebin.com/x9zEiHxR) findest du ein Beispiel für diese Codeblöcke in Aktion in einer `.DAT` Datei.

## Vorschau der Lichter
Diese Werkzeuge hilft PC Beat Saber Spielern, eine genauere Vorschau ihrer Beleuchtung zu erhalten. Die meisten Editoren zeigen keine naturgetreuen Lichteffekte.

### In-Game mit FPFC
First Person Flying Controller (FPFC) ist ein Startparameter, der sowohl von Steam- als auch von Oculus-Benutzern verwendet werden kann. FPFC öffnet eine Instanz von Beat Saber auf deinem Desktop und erlaubt dir, es mit deiner Tastatur und Maus zu steuern. Du benötigst die SiraUtil Mod, um während der Wiedergabe einer Karte interagieren zu können.

Damit kannst du mit WASD in der Karte "herumfliegen", mit der Taste <kbd>F2</kbd> das Pausenmenü öffnen oder mit der Taste <kbd>ESC</kbd> das Level verlassen (andernfalls musst du den Song zu Ende spielen).

Installiere SiraUtil von Mod Assistant und führe Beat Saber aus, um eine config json-Datei zu erstellen. Bearbeite die Datei `SiraUtil.json` in deinem Ordner `UserData` und ändere `"Enabled": false` in `"Enabled": true` unter FPFCToggle und SongControl und folde dann den unten aufgeführten speicherplattenspezifischen Schritten.

![SiraUtil JSON Setting](~@images/mapping/sirautil-FPFC.png)

**Für Steam User:**

Öffne die Spieleigenschaften und füge `fpfc` zu den Steam Startoptionen in den Einstellungen Allgemein hinzu. ![FPFC Startoptionen](~@images/mapping/fpfc.png)

**Für Oculus Besitzer:**

1. Klicke mit der rechten Maustaste auf Beat Saber.exe und erstelle eine Verknüpfung.
2. Bearbeite das Ziel, um "fpfc" am Ende hinzuzufügen. Zum Beispiel: `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber.exe" fpfc`

Nach der Installation der Mods und dem Hinzufügen des Startparameters kannst du dich nun in einer Karte bewegen und pausieren. Die Umschalttaste zum Umschalten zwischen Headset- und Maus-/Tastatursteuerung ist <kbd>G</kbd>.

:::warning HINWEIS

* Wenn du zurück in VR gehst und das Spiel auch im Headset nicht geladen wird:
  * Drücke die Taste <kbd>G</kbd>, bis das Headset das Spiel anzeigt  
    **==ODER==**
  * Beende das Spiel, entferne die Startoption, und starte das Spiel neu.

* Wenn der Mod nicht zu funktionieren scheint, stelle sicher, dass die Einstellung "Smooth Camera" im Spiel deaktiviert ist. :::

### Online mit BS Viewer
Der [BS Viewer](https://skystudioapps.com/bs-viewer/) von **+1 Rabbit** ist ein Online-Tool, mit dem du bequem überprüfen kannst, wie deine Karte im Spiel aussehen könnte, ohne das Spiel zu starten. Lade einfach deine Karten ZIP auf die Website hoch und sieh dir die Vorschau an! Leider werden **IOS und Safari derzeit nicht unterstützt.**

## Credits
Die Inhalte in diesem Abschnitt wurden von [LittleAsi](./mapping-credits.md#littleasi) und [Kolezan](./mapping-credits.md#kolezan) oder von Anleitungen von [Puds](./mapping-credits.md#puds) und [MandyNasty](./mapping-credits.md#mandynasty) abgeleitet. Mit visuellen Medienbeiträgen von [Aeroluna](./mapping-credits.md#aeroluna) und [Bullet](./mapping-credits.md#bullet).
