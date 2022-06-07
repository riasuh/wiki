---
sidebar: auto
prev: ./basic-mapping.md
next: ./intermediate-lighting.md
description: Leer hoe je handmatig aan de slag gaat met het verlichten van je level!
---

# Basis verlichting
_Maak van Beat Saber een lichtere plek door je levels handmatig te verlichten._

* [Woordenlijst](./glossary.md)

---

Elk level moet een soort verlichting hebben. Als je eenmaal de hulpmiddelen kent die tot je beschikking zijn, kan simpele handmatige verlichting erg gemakkelijk zijn. [Deze link](https://streamable.com/s/x7zj0/vrugyj) is een videovoorbeeld van zeer eenvoudige handmatige verlichting.

::: tip OPMERKING Het voorbeeld gebruikt [Map Color Overrides](#map-color-overrides). Je hoeft geen AaltopahWi of Skeelie te zijn om geweldige verlichting te maken! :::

## Soorten verlichting
De beschikbare lichttypes zijn consistent in elk van de ingebouwde spelomgevingen, ze kunnen zich in een andere positie bevinden of in sommige gevallen niet aanwezig zijn.

* **Center Lights:** Over het algemeen verlichting aan de zijkant van het spoor, onder het spoor, en soms de chevron aan het eind van het spoor. Soms "Bottom/Back/Side" of "BBS" lichten genoemd.
* **Side/Top lasers:** Set van roterende lasers aan de zijkanten van het spoor of boven/onder het spoor, afhankelijk van de omgeving dat je hebt geselecteerd. Rotatie is ingesteld met behulp van de Laser Speed functie.
* **Back Lasers:** Statische lasers, vaak in een "X" patroon aan het eind van het spoor, achter de chevron.
* **Ring Lights:** Lichten aan de binnenkant van de grote buitenringen die in bijna alle omgevingen draaien.
* **Ring Spins:** Gebruikt om beweging in de ringen te creëren. In omgevingen met zowel een binnenste als een buitenste ring draaien de ring spins beide ringen tegelijkertijd.
* **Ring Zooms:** Wordt gebruikt om de innerlijke ringen in en uit te zoomen in omgevingen die deze hebben. Heeft geen invloed op de buitenste ring.
* **Laser Speed:** Verandert de snelheid van de side laser rotaties van stationair (0) tot heel snel (20). Stel het onafhankelijk in voor de rechter en de linker side lasers. Back top lasers bewegen niet. Laser speed is lineair waardoor **2** twee keer zo snel is als **1** en **5** vijf keer zo snel is als **1**.
* **Boost Event:** Verandert de licht kleuren tussen twee paar kleuren. Off gebruikt het eerste paar kleuren. On gebruikt het tweede paar (boost) kleuren. Er is geen fade of flash optie voor dit evenement.

## Verlichtingsevenementen
Elk type verlichting kan gebruik maken van vier verschillende verlichtingsevenementen.

* **On:** Zet een lamp aan die aan blijft totdat je een ander evenement type plaatst.
* **Off:** Het uitschakelen van een lamp kan evenveel of meer impact hebben dan als het aan aanzetten ervan.
* **Flash:** knippert feller dan een standaard "on" evenement en blijft aan totdat je een ander evenement type plaatst.
* **Fade:** knippert feller dan een standaard "on" evenement maar word langzaam minder fel en gaat dan uit.

::: warning OPMERKING   
Het is onmogelijk om de duur van een fade out te bepalen, of om een fade in te gebruiken met standaard verlichting. Aangepaste fade tijden vereisen Chroma, dit zal worden besproken in Geavanceerde Verlichting (binnenkort beschikbaar). :::

## Beste werkwijzen & technieken
> "De enige verkeerde verlichting is **GEEN** verlichting.... of een lichtmap."  
> ~ Skeelie

Goed verlichten is een kunst, wat betekent dat het veel subjectiever is dan het maken van levels. Er zijn relatief weinig beste werkwijzen om aan de slag te gaan, en eenvoudige handmatige verlichting is bijna onmogelijk om slecht te doen.

**TranquillizeMe** heeft een verlichtingstutorial gecreëerd, [Beat Saber Lighting Techniques Tutorial](https://www.youtube.com/watch?v=EDbPRN_u3jc), met details van handige verlichtingstechnieken en algemene tips voor verlichting.

::: warning OPMERKING   
Verlichtingsvoorbeelden zijn niet realistisch in de editors die nu beschikbaar zijn, dus het is belangrijk om deze vaak in het spel te bekijken. Zie [Het bekijken van jouw verlichting](#previewing-your-lights) voor sommige programma's die kunnen helpen. :::

### Sneltoetsen
Elke level-editor werkt anders met verlichting, dus zorg dat je de sneltoetsen leert kennen en hoe de plaatsingen werken in je eigen editor. Verlichtingsneltoetsen variëren per editor. Raadpleeg de gebruikershandleiding van jouw editor of lees de README of verwijs naar deze handige lijst [Cross-Editor Sneltoetsen](./editor-keybinds.md).

### Het toewijzen van verlichtingsevenementen
Level makers die hun eerste level verlichten moeten beginnen met het toewijzen van specifieke [verlichtingstypen](#lighting-types) aan specifieke instrumenten, en vanuit daar verder gaan een meer ervaring opdoen. Deze methode produceert meestal niet de meest opwindende shows, maar het is moeilijk om het verkeerd te doen. Het ziet er misschien uit als:

* **Track Lights:** Bass of Kick Drum
* **Lasers:** Melodie
* **Ring Lights:** Synth A of Cymbals
* **Ring Zoom:** Synth B

Zodra dit type basisstructuur op zijn plek is en je comfortabeler bent met hoe alles werkt, kan je bedenken waar je misschien dingen wilt aanpassen om daar nadruk op te leggen. Het instellen van een strikt patroon is noodzakelijk om impact te creëren voor wanneer je een aanpassing maakt; als je alles accentueert, dan accentueer je niks (dit geld ook voor blokplaatsing!).

#### Een voorbeeld van verlichtingsmentor, LittleAsi
> Normaal verlicht ik de melodie met alle drie de lasers (vocaal en instrumentaal op verschillende kleuren, of primaire instrumentaal en accenten op een andere kleur), drums op de ring lichten, en of bas of iets harmonisch zoals synths op de Bottom/back/Side (BBS) (soms een beetje veel omdat ze de BBS-intensiteit hebben verhoogd). Als de drums te betrokken zijn om alleen op de ringlichten te gaan of er is niets anders op zijn plaats voor de BBS, verplaats ik de kick drum naar BBS. Als de drums echt dominant zijn, doe ik soms de back-top laser op de snare om daarna de ringlichten aan de cymbals te wijden. De talrijke mogelijkheden voor het veranderen van lasergedrag en uiterlijk, maken ze echter de beste kandidaat voor het volgen van de melodie. Ik heb 0 snelheid lasers gebruikt voor gesloten hi-hat met verschillende snelheden voor open hi-hat en cymbal crashes, Maar het hoeft zeker geen specifieke manier te zijn (alleen intern samenhangend).

### Laser Speed Resetten
Dezelfde laser speed twee keer op rij instellen zal ervoor zorgen dat deze wordt gereset naar een willekeurige positie. Bijvoorbeeld, de speed instellen op 1 voor elke snare hit zal ervoor zorgen dat de laser posities willekeurig worden gepaald zonder dat ze ooit hun rotatie snelheid veranderen.

Als je de laser speed niet reset, zal het voor altijd blijven draaien met die snelheid totdat het veranderd word.

### Off Event plaatsing
De geluiden binnen een liedje hebben zelden een precies eindpunt, dus er is niet altijd een "juiste" tijd om het `Off` evenement te plaatsen. Wees er van bewust wanneer je ervoor kiest om de lichten die zijn gekoppeld aan specifieke geluiden of instrumenten uit te zetten, en pas dit consistent toe tijdens het lied.

Wees voorzichtig met het plaatsen van off evenementen precies tussen twee lichten in, omdat dit een onbedoeld stroboscoop effect kan veroorzaken.

## Standaard Omgevingen
Er zijn verschillende ingebouwde omgevingen in Beat Saber die deel uitmaken van het basisspel en met een paar klikken eenvoudig kunnen worden gebruikt.

::: warning OPMERKING Aangepaste omgevingsmodellen (platforms) gemaakt door de community bestaan, maar vereisen de Custom Platforms mod die momenteel niet beschikbaar is via Mod Assistant. Er kan een bèta versie beschikbaar zijn in het `#pc-mods` kanaal van de BSMG Discord. :::

De basisstructuur van elke omgeving is meestal hetzelfde. In de [Mediocre Map Assistant 2](./mediocre-map-assistant.md) editor ziet het lichtspoor er als volgt uit:

::: align center ![Screenshot of the MMA2 lighting track from the top down](~@images/mapping/mma2-lighting-track.jpg) :::

### Omgevingsvoorbeelden
|          Video en Schermafbeelding (klik om de volledige grootte te openen)          | Omgeving                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|:------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|      ![Afbeelding van de standaard omgeving](~@images/mapping/default_env.jpg)       | **The First (Default) Environment**<br />**Info.dat Name:** `DefaultEnvironment` <br />**Default Colors:** Red & Blue<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :white_check_mark: (both squares) <br />**Ring Zoom:** :white_check_mark: (inner square)<br />**Equalizer:** :white_check_mark:<br />**Note:** As of 1.6 Back Top Lasers are below the Track Lasers <br /><br />**Video Preview:** [YouTube](https://youtu.be/ab7kjMsIBHA)                                                                                                                                                                                                                                                                                       |
|       ![Afbeelding van de Origins omgeving](~@images/mapping/origins_env.jpg)        | **Origins Environment**<br />**Info.dat Name:** `OriginsEnvironment`<br />**Default Colors:** Yellow & Pink notes, Blue & Light Blue lights<br /><br />**Lasers:** :white_check_mark:<br />**Ring Spin:** :white_check_mark:<br />**Ring Zoom:** :x:<br />**Equalizer:** :white_check_mark: <br /><br /> **Video Preview:** [YouTube](https://youtu.be/Ysvm5N9V1wU)                                                                                                                                                                                                                                                                                                                                                                                                         |
|      ![Afbeelding van de Triangle omgeving](~@images/mapping/triangle_env.jpg)       | **Triangle Environment**<br />**Info.dat Name:** `TriangleEnvironment`<br />**Default Colors:** Red & Blue<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :white_check_mark: (square and triangle) <br />**Ring Zoom:** :white_check_mark: (triangle)<br />**Equalizer:** :white_check_mark:<br />**Note:** As of 1.6 Back Top Lasers are below the Track Lasers <br /><br />**Video Preview:** [YouTube](https://youtu.be/FhAg4Awl0k0)                                                                                                                                                                                                                                                                                               |
|          ![Afbeelding van de Nice omgeving](~@images/mapping/nice_env.jpg)           | **Nice Environment**<br />**Info.dat Name:** `NiceEnvironment`<br />**Default Colors:** Red & Blue<br /><br />**Lasers:** :white_check_mark: (top & bottom)<br />**Ring Spin:** :white_check_mark: (both squares)<br />**Ring Zoom:** :white_check_mark: (inner square)<br />**Equalizer:** :white_check_mark:<br />**Note:** As of 1.6 Back Top Lasers are below the Track Lasers <br /><br />**Video Preview:** [YouTube](https://youtu.be/LrLFf6fspiw)                                                                                                                                                                                                                                                                                                           |
|    ![Afbeelding van de Big Mirror omgeving](~@images/mapping/big-mirror_env.jpg)     | **Big Mirror Environment**<br />**Info.dat Name:** `BigMirrorEnvironment`<br />**Default Colors:** Red & Blue<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :white_check_mark: <br />**Ring Zoom:** :x:<br />**Equalizer:** :white_check_mark: <br /><br />**Video Preview:** [YouTube](https://youtu.be/lmWeJL8Qxh4)                                                                                                                                                                                                                                                                                                                                                                                                                        |
|   ![Afbeelding van de Imagine Dragons omgeving](~@images/mapping/dragons_env.jpg)    | **Imagine Dragons Environment**<br /> **Info.dat naam:** `DragonsEnvironment`<br /> **Standaard kleuren:** Rood & Blauw<br /><br /> **Lasers:** :white_check_mark: (links & rechts)<br /> **Ring Spin:** :white_check_mark: (vierkant en helix)<br /> **Ring Zoom:** :white_check_mark: (helix)<br /> **Equalizer:** :white_check_mark:<br /> **Opmerking:** De Back Top Laser is de twee rails aan de meest buitenste randen van het scherm. Het zal altijd de tegenovergestelde kleur verlichten dan wat je ingesteld hebt. <br /><br />**Video Preview:** [YouTube](https://youtu.be/tSzvvbDK71s)                                                                                                                                                                |
|           ![Afbeelding van de K/DA omgeving](~@images/mapping/kda_env.jpg)           | **K/DA Environment**<br /> **Info.dat naam:** `KDAEnvironment`<br /> **Standaard kleuren:** Oranje & Paars<br /><br /> **Lasers:** :white_check_mark: (links & rechts)<br /> **Ring Spin:** :x:<br /> **Ring Zoom:** :x:<br /> **Equalizer:** :x:<br /> **Opmerking:** Ring Light positie verlicht de vijf rails bovenin. De lichten in het midden van de pijlen gaan nooit uit. <br /><br />**Video Preview:** [YouTube](https://youtu.be/knXgpnW5NWQ)                                                                                                                                                                                                                                                                                                                   |
|    ![Afbeelding van de Monstercat omgeving](~@images/mapping/monstercat_env.jpg)     | **Monstercat Environment**<br /> **Info.dat naam:** `MonstercatEnvironment`<br /> **Standaard kleuren:** Rood & Blauw<br /><br /> **Lasers:** :white_check_mark: (links & rechts)<br /> **Ring Spin:** :white_check_mark:<br /> **Ring Zoom:** :x: <br /> **Equalizer:** :white_check_mark:<br /> **Opmerking:** Sinds 1.6 zijn Back Top Lasers onder de Track Lasers. Ring Licht position verlicht de vijf rails bovenin. <br /><br />**Video Preview:** [YouTube](https://youtu.be/Er3OCUmSK-0)                                                                                                                                                                                                                                                                     |
|     ![Afbeelding van de Crab Rave omgeving](~@images/mapping/crab-rave_env.jpg)      | **Crab Rave Environment**<br /> **Info.dat naam:** `CrabRaveEnvironment`<br /> **Standaard kleuren:** Groen & Blauw<br /><br /> **Lasers:** :white_check_mark: (links & rechts)<br /> **Ring Spin:** :white_check_mark:<br /> **Ring Zoom:** :x: <br /> **Equalizer:** :white_check_mark: <br /> **Opmerking:** Sinds 1.6 zijn Back Top Lasers onder de Track Lasers. Ring Licht position verlicht de vijf rails bovenin. <br /><br />**Video Preview:** [YouTube](https://youtu.be/xTXHCTBYkck)                                                                                                                                                                                                                                                                      |
|    ![Afbeelding van Panic! at the Disco omgeving](~@images/mapping/panic_env.jpg)    | **Panic! at the Disco Environment**<br /> **Info.dat naam:** `PanicEnvironment`<br /> **Standaard kleuren:** Rood & Blauw<br /><br /> **Lasers:** :white_check_mark: (links & rechts)<br /> **Ring Spin:** :white_check_mark: <br /> **Ring Zoom:** :white_check_mark: <br /> **Equalizer:** :white_check_mark:<br /> **Opmerking:** De Ring Lights zijn veel feller in deze omgeving dan andere. <br /><br />**Video Preview:** [YouTube](https://youtu.be/2UJ8-edr4xU)                                                                                                                                                                                                                                                                                            |
|     ![Afbeelding van de Rocket League omgeving](~@images/mapping/rocket_env.jpg)     | **Rocket League Environment**<br />**Info.dat Name:** `RocketEnvironment`<br />**Default Colors:** Orange & Blue<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :x:<br />**Ring Zoom:** :x:<br />**Equalizer:** :x: <br /><br />**Video Preview:** [YouTube](https://youtu.be/glgMeDJopIM)                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|     ![Afbeelding van de Green Day omgeving](~@images/mapping/green-day_env.jpg)      | **Green Day Environment**<br />**Info.dat Name:** `GreenDayEnvironment`<br />**Default Colors:** Green & Cyan<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :white_check_mark: <br />**Ring Zoom:** :white_check_mark:<br />**Equalizer:** :x:<br />**Video Preview:** [YouTube](https://youtu.be/QLw4Rg-mHKE)                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| ![Afbeelding van de Green Day Grenade omgeving](~@images/mapping/gd-grenade_env.jpg) | **Green Day Grenade Environment**<br />**Info.dat Name:** `GreenDayGrenadeEnvironment`<br />**Default Colors:** Green & Cyan<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :x:<br />**Ring Zoom:** :x: <br />**Equalizer:** :x:<br />**Video Preview:** [YouTube](https://youtu.be/DIzLR65HyN0)                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
|     ![Afbeelding van de Timbaland omgeving](~@images/mapping/timbaland_env.jpg)      | **Timbaland Environment**<br /> **Info.dat naam:** `TimbalandEnvironment`<br /> **Standaard kleuren:** Grijze & Blauwe blokken, Blauwe & Blauwe lichten (dezelfde kleuren)<br /><br /> **Lasers:** :white_check_mark: (linker & rechter lichten zijn parellel aan de ringen)<br /> **Ring Spin:** :white_check_mark: <br /> **Ring Zoom:** :white_check_mark: <br /> **Equalizer:** :white_check_mark:<br /> **Opmerking:** De "Timbaland" tekst aan de zijkant gaat nooit uit. Laser speed beïnvloed de Back Top Lasers op de linker en rechter ringen. <br /><br />**Video Preview:** [YouTube](https://youtu.be/ZMNrCbSxBVM)                                                                                                                                     |
|       ![Afbeelding van de FitBeat omgeving](~@images/mapping/fitbeat_env.jpg)        | **FitBeat Environment**<br /> **Info.dat naam:** `FitBeatEnvironment`<br /> **Standaard kleuren:** Gele & Roze blokken, Oranje & Blauwe lichten<br /><br /> **Lasers:** :white_check_mark: (links & rechts)<br /> **Ring Spin:** :white_check_mark: (buitenste lasers en helix) <br /> **Ring Zoom:** :white_check_mark: (helix) <br /> **Equalizer:** :white_check_mark: <br /> **Opmerking:** Back Top Lasers zullen licht geven in de tegenovergestelde kleur dan wat je hebt ingesteld. <br /><br />**Video Preview:** [YouTube](https://youtu.be/PNucTPiPBn8)                                                                                                                                                                                                  |
|   ![Afbeelding van de Linkin Park omgeving](~@images/mapping/linkin-park_env.jpg)    | **Linkin Park Environment**<br />**Info.dat Name:** `LinkinParkEnvironment`<br />**Default Colors:** Red & Blue-Grey notes, Beige & White lights, Orange & Blue boost lights <br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :white_check_mark: (controls laser spread) <br />**Ring Zoom:** :x: <br />**Equalizer:** :white_check_mark: (on side wall) <br /><br />**Video Preview:** [YouTube](https://youtu.be/nl8_sHYnP7k) <br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/BhMQ8KS2rZk)                                                                                                                                                                                                                         |
|           ![Afbeelding van de BTS omgeving](~@images/mapping/bts_env.jpg)            | **BTS Environment**<br />**Info.dat Name:** `BTSEnvironment`<br />**Default Colors:** Pink & Purple notes, Pink & Purple lights, Light Pink & Light Blue boost lights<br /><br />**Lasers:** :white_check_mark: (left & right)<br />**Ring Spin:** :white_check_mark: (background pillars) <br />**Ring Zoom:** :white_check_mark: (track pillars) <br />**Equalizer:** :x: <br />**Note:** BTS logo in the center never turns off.<br /><br />**Video Preview:** [YouTube](https://youtu.be/HrGK2puKBhI) <br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/HYnVROsLBBs)                                                                                                                                                                      |
|  ![Afbeelding van de Kaleidoscope omgeving](~@images/mapping/kaleidoscope_env.jpg)   | **Kaleidoscope Environment**<br />**Info.dat Name:** `KaleidoscopeEnvironment`<br />**Default Colors:**  Red & Black notes, Red & White lights, Red & Magenta boost lights<br /><br />**Lasers:** :white_check_mark: <br />**Ring Spin:** :white_check_mark:<br />**Ring Zoom:** :white_check_mark:<br />**Equalizer:** :x:<br /><br />**Video Preview:** [YouTube](https://youtu.be/6zgH3QcN_T8) <br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/eZBd7-yb284)                                                                                                                                                                                                                                                                                    |
|       ![Image of Interscope environment](~@images/mapping/interscope_env.jpg)        | **Interscope Environment**<br />**Info.dat Name:** `InterscopeEnvironment`<br />**Default Colors:**  Yellow & Pink notes, Purple & White lights, Cool Red & Cool White boost lights<br /><br />**Lasers:** :white_check_mark: <br />**Ring Spin:** :white_check_mark: (cars) <br />**Ring Zoom:** :white_check_mark: (cars and extra laser spread) <br />**Equalizer:** :white_check_mark:<br />**Extra Events**: 6 and 7 control extra lights. 16 and 17 control car hydraulics.<br /><br />**Video Preview:** [YouTube](https://youtu.be/pnaNPD5ljqI)<br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/GmJpF2VA-6E)                                                                                                                       |
|         ![Image of Skrillex environment](~@images/mapping/skrillex_env.jpg)          | **Skrillex Environment**<br />**Info.dat Name:** `SkrillexEnvironment`<br />**Default Colors:**  Red & Black notes, Pink & Turquoise lights, Neon Red & Neon Green boost lights<br /><br />**Lasers:** :white_check_mark: <br />**Ring Spin:** :white_check_mark: (first ring spin)<br />**Ring Zoom:** :white_check_mark: (second ring spin) <br />**Equalizer:** :x:<br />**Extra Events**: 6 and 7 control extra lights. <br /><br />**Video Preview:** [YouTube](https://youtu.be/Uk0JugoZ3w4)<br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/-SD5F3b7Q3g)                                                                                                                                                                              |
|        ![Image of Billie Eilish environment](~@images/mapping/billie_env.jpg)        | **Billie Eilish Environment**<br />**Info.dat Name:** `BillieEnvironment`<br />**Default Colors:**  Yellow & Light Grey notes, Orange & Cream lights, Red & White Blue boost lights<br /><br />**Lasers:** :white_check_mark: (sun rays)<br />**Ring Spin:** :white_check_mark: (controls rain)<br />**Ring Zoom:** :white_check_mark: (controls sun rays and side beams) <br />**Equalizer:** :x:<br />**Extra Events**: 6, 7, 10, and 11 control extra lights. <br />**Note:** This is the first environment use events 10 and 11 and these events only function on map version `2.5.0` or later.<br /><br />**Video Preview:** [YouTube](https://youtu.be/R53QcGlo80Q)<br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/Kgm6Xn7xcNQ) |
|           ![Image of Spooky environment](~@images/mapping/spooky_env.jpg)            | **Spooky Environment**<br />**Info.dat Name:** `HalloweenEnvironment`<br />**Default Colors:**  Orange & Black notes, Red & Light Blue lights, Green & Light Purple boost lights<br /><br />**Lasers:** :white_check_mark:<br />**Ring Spin:** :x:<br />**Ring Zoom:**:x: <br />**Equalizer:** :x:<br /><br />**Video Preview:** [YouTube](https://youtu.be/TbX3Z3mU2y8)<br />                                                                                                                                                                                                                                                                                                                                                                                            |
|             ![Image of Gaga environment](~@images/mapping/gaga_env.jpg)              | **Lady Gaga Environment**<br />**Info.dat Name:** `GagaEnvironment`<br />**Default Colors:** Pink & Green notes, Yellow & Magenta lights, Orange & Blue boost lights<br /><br />**Lasers:** :white_check_mark: (electricity) <br />**Ring Spin:** :x:<br />**Ring Zoom:**:x: <br />**Equalizer:** :x:<br />**Extra Events**: 6, 7, 10, and 11 control additional lightning. 16, 17, 18, and 19 control additional tower height control. <br /><br />**Video Preview:** [YouTube](https://youtu.be/FRNLFW4P3RQ)<br /> **Official Showcase & Tutorial**: [YouTube](https://youtu.be/2DJmcQjjCl0)                                                                                                                                                                      |
|            ![Image of Weave environment](~@images/mapping/weave_env.jpg)             | **Weave Environment**<br />**Info.dat Name:** `WeaveEnvironment`<br />**Default Colors:** Red & Blue notes, Red & Blue lights, Magenta & White boost lights<br /><br />**Note** Lights require using the new lighting system in map version `3.0.0` to function.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
|     ![Image of Glass Desert environment](~@images/mapping/glass-desert_env.jpg)      | **Glass Desert Environment**<br />**Info.dat Name:** `GlassDesertEnvironment`<br />**Default Colors:**  Yellow & Pink notes, Blue & Light Blue lights<br /><br />**Lasers:** :white_check_mark: <br />**Ring Spin:** :x:<br />**Ring Zoom:** :x:<br />**Equalizer:** :white_check_mark:<br />**Note:** This is the first 360&deg; environment. 360 levels MUST use this and it's not useable for standard levels. Ring Light position controls the horizontal outer rail. Back Top Laser position controls the six rails at the top. <br /><br />**Video Preview:** [YouTube](https://youtu.be/K3rqWNG5pn8)                                                                                                                                                             |

### Stel je omgeving in
Nieuwe standaard omgevingen worden redelijk vaak beschikbaar gemaakt, wat betekent dat level editors niet altijd de volledige lijst beschikbaar hebben. Als de omgeving die je wilt gebruiken geen optie is in de instellingen van je favoriete editor, moet je je `info.dat` bestand bewerken om de omgevingsnaam toe te voegen.

1. Bepaal welke omgeving je wilt gebruiken en kopieer vervolgens de `Info.dat naam` uit [omgevingsvoorbeelden](#omgevingsvoorbeelden) hierboven.
2. Open jouw `Info.dat` bestand in een tekst bewerker naar keuze.
3. Scroll naar beneden naar de `"_environmentName":` sectie.
4. Plak de naam die je gekopieerd hebt in stap 1.

> **LET OP:** Je kan geen custom platform gebruiken in dit veld. Dit wordt besproken in [Geavanceerde verlichting](./advanced-lighting.md#custom-environments).

## Map color overrides
Je kunt je eigen level-kleurenschema forceren in het spel, zolang de gebruiker de SongCore mod geïnstalleerd heeft en de `Enable Custom Song Colors` optie in de mod instellingen aan heeft.

Sinds Beat Saber versie 1.4 kunnen gebruikers de Rood/Groen/Blauw (RGB) kleuren van blokken, verlichting en muren voor hun spel instellen. Maar, deze worden overgeschreven met de kleuren die gedefinieerd zijn in het `Info.dat` bestand als de gebruiker de `Enable Custom Song Colors` optie aan heeft.

::: tip Bij het kiezen van color overrides voor de blokken. Het is **STERK** aanbevolen dat je rode/warme/agressieve kleuren aan de linkerkant en blauwe/koude/zachte kleuren aan de rechterkant houdt om verwarring van de spelers te voorkomen. :::

Zie [standaard omgevingskleuren](./lighting-defaults.md) voor een lijst van standaard kleuren die in de omgevingen worden gebruikt.

[ChroMapper](./#chromapper), [MMA2](./#mediocre-map-assistant-2), and [Beatmapper](./#beatmapper-app), natively support color overrides. Bekijk hun respectievelijke gidsen voor meer informatie.

### Color overrides handmatig toevoegen

1. Bepaal welke RGB-kleuren jij jouw blokken en/of verlichting en/of muren wilt laten zijn. Gebruik een kleurenschema programma zoals [Paletton](https://paletton.com/#uid=1000u0kllllaFw0g0qFqFg0w0aF) om complementaire kleuren te vinden.
   * Jouw rood, groen en blauw waarden moeten worden veranderd van de normale 0-255 schaal naar de 0-1 schaal. Gebruik een site zoals [EasyRGB](https://www.easyrgb.com/en/convert.php) om jouw waarden te veranderen.
2. Open jouw `Info.dat` bestand in een tekst bewerker naar keuze.
3. Scroll naar beneden naar de `"_customData": {` sectie van het niveau waar je een kleur aan wilt geven.
    * Het gebruik van de globale `"_customData": {` buiten de `"_difficultyBeatmapSets": [` reeks werkt mogelijk niet zoals verwacht.
4. Plak de codeblokken hieronder die je wilt forceren in de `_customData` accolades (`{` en `}`) en vervang vervolgens de `"r":`, `"g":`, en `"b":` waarden met wat je hebt gekozen in stap 1.
   * De `"r":` en `"g":` waarden **moeten** komma's hebben erna.

Zie de lijnen 29-60 en 69-100 van deze [Pastebin clip](https://pastebin.com/x9zEiHxR) voor een voorbeeld van deze codeblokken in actie in een `.DAT` bestand.

## Jouw verlichting bekijken
Deze programma's zullen ervoor zorgen dat PC Beat Saber gebruikers hun verlichting nauwkeuriger kunnen bekijken. De meeste editors laten geen levensechte verlichtingseffecten zien.

### In-game met FPFC
First Person Flying Controller (FPFC) is een startparameter wat gebruikt kan worden door Steam of Oculus gebruikers. FPFC opent Beat Saber op je computer en laat je het besturen met je toetsenbord en muis.

While a map is playing, pressing:

* `P` **P**auses the map
* `M` Returns to **m**enu if paused
* `R` **R**estarts the map if paused
* `C` Unpauses and **c**ontinues playing

You will need the SiraUtil mod in order move the camera while a map is playing. Without it, the camera is fixed in the floor at an undesirable angle. Install SiraUtil from Mod Assistant and run Beat Saber to create a config json file. SiraUtil also adds additional useful features such as camera FOV, sensitivity, and rebindable pause and exit controls. Edit the `SiraUtil.json` file in your `UserData` folder to tweak settings.

**For Steam Users:**

Open the game properties and add `fpfc` to the Steam launch options in the General tab. ![Fpfc launch options](~@images/mapping/fpfc.png)

**For Oculus Users:**

1. Rechtsklik op Beat Saber.exe en maak een snelkoppeling.
2. Bewerk het doel en voeg "fpfc" toe aan het einde ervan. Bijv: `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber.exe" fpfc`.

After installing the mods and adding the launch parameter you can then now move around and pause in a map. The default toggle key to switch between headset and mouse/keyboard control is <kbd>G</kbd>.

:::warning NOTE

* If you go back into vr and the game doesn't load in the headset either:
  * Press the <kbd>G</kbd> key until the headset displays the game  
    **==OR==**
  * Quit the game, remove the launch option, and relaunch the game.

* If the mod doesn't seem to be working, make sure the in-game Smooth Camera setting is disabled.

* For difficulties other than Expert+, the game defaults to a `No Flicker` option for lighting which reduces the amount of strobes and ring spin events shown. Check to make sure this `Player Option` setting is set what you intend to view! :::

### Online met BS Viewer
[BS Viewer](https://skystudioapps.com/bs-viewer/) by **+1 Rabbit** is an online tool that is a convenient way to checkout how your map might look in game without the game. Just upload your map zip to the website and preview! Unfortunately **IOS and Safari are currently not supported.**

## Bijdragen
Content in this section was authored by [LittleAsi](./mapping-credits.md#littleasi) and [Kolezan](./mapping-credits.md#kolezan) or derived from guides by [Puds](./mapping-credits.md#puds) and [MandyNasty](./mapping-credits.md#mandynasty). With visual media contributions from [Aeroluna](./mapping-credits.md#aeroluna) and [Bullet](./mapping-credits.md#bullet).
