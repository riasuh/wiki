---
sidebar: auto
prev: ./platforms-guide.md
description: Bobbies Anleitung zur Erstellung von Custom Notes!
---

# Custom Notes Guide
_Bobbies Anleitung zur Erstellung von Custom Notes._

## Einführung
Diese Anleitung erfordert Grundwissen über 3D-Modellierung und die Unity Engine. Einige Dinge sind erforderlich:

* Der Unity Editor - spezifisch, [Unity version 2018.1.6f1](https://download.unity3d.com/download_unity/57cc34175ccf/Windows64EditorInstaller/UnitySetup64-2018.1.6f1.exe)
* Das [Custom Notes Unity-Projekt](https://github.com/legoandmars/CustomNotesUnityProject/archive/master.zip)
* Wenn du nicht bereits ein Mesh hast, das du verwenden kannst, benötigst du ein 3D-Modellierungsprogramm. Ich persönlich empfehle [Blender](https://www.blender.org/)
* Je nachdem, was genau du modellierst, kann eine Bildbearbeitungssoftware wie [Photoshop](https://www.adobe.com/products/photoshop.html) oder[GIMP](https://www.gimp.org/downloads/) erforderlich sein.

## Unity Projekt
::: danger DISCLAIMER
Stelle sicher, dass du die Unity-Version 2018.1.6f1 verwendest!
::: Öffne das Custom Notes Projekt mit Unity.

![Unity Projekt](~@images/models/notes/unity_window.png)

Im Hierarchie-Fenster auf der linken Seite findest du einige Beispiel-Noten.

![Objekthierarchie](~@images/models/notes/02.png)

Wenn du auf eine dieser Beispiel-Noten klickst, siehst du, dass sie mit einem `"NoteDescriptor"` versehen ist.

![NoteDescriptor](~@images/models/notes/03.png)

Lass uns kurz überfliegen, was jede dieser Einstellungen bewirkt.

### Note Name & Autor Name
Dies sollte einfach sein. Der Name der Note und der des Autors wird in der Benutzeroberfläche für die Auswahl der Noten angezeigt, wie in der folgenden Abbildung dargestellt.

![Beispiel für den Namen einer Note und den Namen des Autors im Spiel](~@images/models/notes/04.png)

### Icon
Diese Einstellung nimmt ein Bild auf, das als Symbol verwendet werden soll. Das Symbol wird in der Benutzeroberfläche für die Auswahl von Notizen angezeigt, wie in der Abbildung oben zu sehen.

### Basisnotenpfeile deaktivieren
Wenn diese Einstellung aktiviert ist, werden die Pfeile auf den Noten unsichtbar. Hinweis: Du musst `NoteDotLeft` und `NoteDotRight` gameobjects in deinen Noten haben, wenn du diese Option aktivieren möchtest.

### Verwende Noten Farben
Wenn diese Option aktiviert ist, werden die aktuell eingestellten Noten-Farben des Players verwendet, um Ihre Noten entsprechend zu färben. Damit können deine Noten `CustomColors` unterstützen. Wenn du dies richtig nutzen willst, solltest du unbedingt den Abschnitt lesen, der sich damit beschäftigt, wie du deine Noten mit benutzerdefinierten Farben veränderst.

### Stärke der Noten Farben
Diese Option wird nur verwendet, wenn `Uses Note Color` aktiviert ist. Die Stärke der Noten-Farbe legt fest, wie stark die auf die Noten angewendete Tönung ist und ist standardmäßig auf 1 eingestellt. Je niedriger du diese Zahl einstellst, desto dezenter wird die Tönung sein.

## Noten erstellen
Du solltest bereits ein 3D-Modell haben, das du für deine Noten verwenden möchtest. Für das Tutorial werde ich ein einfaches Dreiecks-Mesh verwenden, das ich in Blender erstellt habe. Fahre fort und importiere dein Modell in das Projekt.

![Importieren in das Unity-Projekt](~@images/models/notes/05.png)

Nachdem du das Modell importiert hast, erstelle ein neues leeres `GameObject` in der Hierarchieansicht und nenne es so, wie du deine Note benennen willst. Ich nenne meine `TriangleNote`.

![Erstellung eines neuen GameObject](~@images/models/notes/07.png)

Klickenim `GameObject` deiner Note auf `Komponente hinzufügen` und füge einen `NoteDescriptor` hinzu. Kümmere dich jetzt nicht darum, irgendwelche Optionen im `NoteDescriptor` zu ändern, das kommt später.

![Hinzufügen eines NoteDescriptors](~@images/models/notes/08.png)

Jetzt können wir damit beginnen, dem Haupt-Spielobjekt unsere Custom Notes "Children" hinzuzufügen. `NoteLeft` und `NoteRight` sind die beiden benötigten Noten. Du kannst aber auch `NoteDotRight`, `NoteDotLeft` oder `NoteBomb` zu deinem Haupt-Spielobjekt hinzufügen. Für dieses Tutorial werde ich nur eine `NoteLeft` und `NoteRight` erstellen.

Erstelle ein neues leeres Spielobjekt innerhalb deines Haupt-Spielobjekts und nenne es `NoteLeft`

![Erstellen eines leeren GameObjects innerhalb von TriangleNote](~@images/models/notes/09.png)

![Darstellung der Hierarchie von TriangleNote und NoteLeft](~@images/models/notes/10.png)

`NoteLeft` wird als eine Art "Container" für alle GameObjects dienen, die Meshes in unserer Notiz enthalten. Wir können unsere Meshes frei positionieren und drehen, wenn wir sie in einem separaten GameObject innerhalb von `NoteLeft` platzieren, was nicht möglich wäre, wenn wir die Mesh-Komponenten einfach direkt zum `NoteLeft` GameObject hinzufügen würden.

Ziehe dein importiertes Mesh auf `NoteLeft` in der Hierarchieansicht.

![Ziehen des Meshes auf NoteLeft](~@images/models/notes/note_drag.png)

![Ziehen des Meshes auf NoteLeft](~@images/models/notes/56.png)

Du solltest nun dein importiertes Mesh als untergeordnetes GameObject von `NoteLeft` sehen. Je nachdem, welches Modellierungsprogramm du verwendet hast, musst du möglicherweise einige Nicht-Mesh-Objekte entfernen. Wenn du in deinem Mesh Objekte mit dem Namen `Camera` oder `Lamp` siehst, **STELLE SICHER, dass du sie löschst!** Wenn du eine Warnung siehst, die besagt, dass "die Prefab-Instanz kaputt geht", drücke "Weiter".

![Hierarchie aufzeigen und auf die Kamera hinweisen](~@images/models/notes/64.png)

![Klicke Weiter auf Warnung](~@images/models/notes/59.png)

Klicke auf das soeben hinzugefügte Objekt und stelle sicher, dass es die Position `(0,0,0)` hat

![Position checken](~@images/models/notes/61.png)

Sobald du das Mesh ausgewählt hast, musst du es richtig skalieren, damit es die Größe einer Note im Spiel hat. Wähle `NoteLeft` und verschiebe es in die Nähe der `TemplateNoteSize`. Die `TemplateNoteSize` sollte das weiße Quadrat in deinem Projekt sein.

::: warning WARNUNG Vergewissere dich, dass du `NoteLeft` wählst, wenn du deine Note verschiebst. Wenn du stattdessen versehentlich die "Children" von `NoteLeft` verschiebst, wird die Mesh nicht ausgerichtet! Die Meshes innerhalb von `NoteLeft` sollten sich fast IMMER an der Position `(0,0,0)` befinden, es sei denn, du hast sie absichtlich angepasst. :::

![Zeige das Mesh neben TemplateNoteSize](~@images/models/notes/62.png)

Sobald du `NoteLeft` in die Nähe der `TemplateNoteSize` verschoben hast, wähle das Skalierungswerkzeug oben links auf dem Bildschirm.

![Auswahl des Skaling-Werkzeuges](~@images/models/notes/63.png)

Wenn das GameObject innerhalb von `NoteLeft` ausgewählt ist, klicke und ziehe es auf das graue Quadrat. Bewege die Maus, bis deine Note ungefähr die gleiche Größe hat wie die `TemplateNoteSize`.

![Zeige wie man das Skalierungswerkzeug verwendet](~@images/models/notes/60.png)

::: warning WARNUNG Stelle sicher, dass du den Maßstab der Objekte INNERHALB von `NoteLeft` anpasst. `NoteLeft` hat immer einen Zwangsmaßstab von eins. Wenn du also einen anderen Maßstab als `(1,1,1)` wählst, wird dein Modell im Spiel anders aussehen! :::

![Zeigt das korrekt skalierte Mesh neben TemplateNoteSize](~@images/models/notes/66.png)

Wie du sehen kannst, ist die Skala, die für mein Netz funktioniert, etwa `(0.65,0.65,0.65)`. Dieser Wert wird wahrscheinlich unterschiedlich sein je nachdem, welches Netz du verwendest. Wenn das Mesh nicht genau die gleiche Größe hat wie die `TemplateNoteSize`, nicht zu sehr beunruhigen lassen, denn es muss nicht exakt sein. Denke daran, dass eine etwas zu große Note im Allgemeinen besser ist als eine etwas zu kleine Note.

::: warning WARNUNG Achte darauf, dass deine Noten in die richtige Richtung zeigen. Achte auf die Richtung aller anderen Noten in der Szene und stelle sicher, dass deine Meshes in die gleiche Richtung zeigen. **DENKE DARAN**: Das `NoteLeft` GameObject sollte immer eine Rotation von `(0,0,0)` haben. Wenn du deine Note drehen musst, drehe nicht `NoteLeft`, sondern drehe die darin enthaltenen Meshes! :::

## Materialien Hinzufügen
Nachdem das Mesh nun richtig skaliert ist, können wir ihm ein Material hinzufügen. Klicken Sie im Projektfenster mit der rechten Maustaste auf `Materialien` und dann auf `Erstellen> Material`. Da dies das Material für das Mesh meiner `LeftNote` sein wird, werde ich es `LeftMaterial` nennen.

![Neues Material erstellen](~@images/models/notes/17.png)

Nun, da wir LeftMaterial haben, müssen wir wählen, welche Shader wir dafür verwenden wollen. Wenn man einen der Standard-Shader von Unity verwendet, werden sie im Spiel nicht richtig angezeigt, also müssen wir einen der `BeatSaber` Shader verwenden.

![Einstellung des Shaders für das neue Material](~@images/models/notes/18.png)

Für mein LeftMaterial werde ich `Unlit Glow` verwenden. Es kann jedoch sein, dass du je nach Mesh einen anderen Shader verwenden möchtest. Hier sind die wichtigsten Unterschiede zwischen den Shadern:

* Lit glow ist beleuchtet und hat Schatten. Du kannst die Richtung, aus der das Licht kommt, und die Stärke des Lichts ändern
* Metallic macht das Material etwas dunkler und ermöglicht es dir, eine metallische Reflexion hinzuzufügen
* Unlit glow ist lit glow ähnlich, hat aber keine Lichteffekte.
* Unlit glow cutout dither ist dasselbe wie unlit glow, ermöglicht es dir aber, Transparenz zu deinem Material hinzuzufügen.

Alle vier Shader erlauben auch die Verwendung von Texturen, obwohl Metallic die Textur für die Reflexion verwendet, anstatt sie direkt anzuwenden.

Sobald du deinen Shader ausgewählt hast, wähle eine Farbe für dein linkes Material. Da dies der der linke Block ist, werde ich eine rötliche Farbe wählen.

![Die Farbe des Materials auswählen](~@images/models/notes/19.png)

Jetzt, da die Farbe festgelegt ist, gehen zurück zu deinem Mesh und lege es als Material fest.

![Auswählen des Material auf dem Mesh](~@images/models/notes/20.png)

![Auswählen des Material auf dem Mesh](~@images/models/notes/21.png)

Deine Note sollte jetzt ein Material haben, das im Spiel richtig angezeigt wird. Jetzt müssen wir eine rechte Note erstellen und das Gleiche wiederholen. Klicke mit der rechten Maustaste auf `NoteLeft` und `Dupliziere` sie. Benenne das Duplikat in `NoteRight` um.

![Duplizieren der linken Note](~@images/models/notes/67.png)

![Anzeige der Hierarchie der Note, mit NoteLeft und NoteRight](~@images/models/notes/68.png)

Führe nun die obigen Schritte erneut aus, um ein zweites Material zu erstellen. Achte darauf, denselben Shader zu verwenden, wenn du möchtest, dass die Noten zwischen den Farben konsistent aussehen. Für mein zweites Material werde ich es RightMaterial nennen und ihm eine blaue Farbe geben.

![Farbe von RightMaterial auswählen](~@images/models/notes/25.png)

Jetzt, wo du das zweite Material hast, wende es auf das Mesh der `NoteRight` an.

![Klicke auf das Mesh der rechten Note](~@images/models/notes/69.png)

![Auswählen des richtigen Notenmaterials auf dem richtigen Noten Mesh](~@images/models/notes/27.png)

![Auswählen des richtigen Notenmaterials auf dem richtigen Noten Mesh](~@images/models/notes/28.png)

Du hast nun zwei Noten, die beide richtig texturiert sind und im Spiel angezeigt werden.

## Exportieren deiner Noten

Nun, da unsere Meshes und Materialien richtig eingestellt sind, können wir zum `NoteDescriptor` zurückkehren und die Einstellungen ändern. Gehe zum Haupt-GameObject deiner Note und sehe dir den `NoteDescriptor` im Eigenschaften-Fenster an.

![Anzeigen des NoteDescriptor](~@images/models/notes/29.png)

Setze den `Note Name` auf den Namen, den deine Note im Spiel haben soll. Ich werde meine auf "Triangle Note" einstellen. Zusätzlich, setze den `Author Name` auf den Namen, den du als Autor angeben möchtest. Ich werde meinen auf "Bobbie" einstellen.

![Anzeigen des NoteDescriptor](~@images/models/notes/30.png)

::: warning WARNUNG
Obwohl es technisch nicht erforderlich ist, wird dringend empfohlen, ein Symbol zu deinen Noten hinzuzufügen, damit
sie in der Benutzeroberfläche leichter zu erkennen sind.
:::

Importiere das Bild, das du für dein Symbol verwenden willst, indem du auf `Neues Asset importieren` klickst. Ich werde ein von mir erstelltes Dreieckssymbol verwenden.

![Importieren eines neuen Assets](~@images/models/notes/31.png)

Wenn dein Bild transparent ist, aktiviere `Alpha ist transparent` und klicke auf "Anwenden".

![Prüfen ob Alpha transparent ist](~@images/models/notes/32.png)

![Klicken anwenden](~@images/models/notes/33.png)

Gehe nun zurück zum `NoteDescriptor` und wähle das Bild aus, das du gerade importiert hast.

![Auswahl der Textur](~@images/models/notes/34.png)

![Auswahl der Textur](~@images/models/notes/35.png)

Jetzt haben wir noch drei Optionen: `Disable Base Note Arrows`, `Uses Note Color` und `Note Color Strength`. Da mein Modell keine benutzerdefinierten Pfeile hat, lasse ich `Disable Base Note Arrows` unmarkiert, damit wir die Standardpfeile behalten. Ich werde `Uses Note Color` vorerst auch nicht ankreuzen, was bedeutet, dass wir auch `Note Color Strength` nicht zu ändern brauchen.

Wenn du `Uses Note Color` aktivierst- und ich empfehle dir dringend, dies zu tun - lies dir unbedingt den Abschnitt über die korrekte Unterstützung benutzerdefinierter Farben! :::

![Anzeigen von NoteDescriptor](~@images/models/notes/36.png)

Nun, da unsere `NoteDescriptor` Optionen vollständig eingestellt sind, können wir unsere Note mit dem `Note Exporter` exportieren. Um zum `Note Exporter` zu gelangen, suche die Registerkarte auf der linken Seite deines Bildschirms, in der Nähe der Registerkarte `Hierarchy`.

![Klicken "Note Exportieren"](~@images/models/notes/70.png)

![Anzeige der Note im Note-Exporter](~@images/models/notes/38.png)

Deine Note sollte am Anfang des `Note Exporter` stehen. Wenn du dir sicher bist, dass alle deine `NoteDescriptor` Einstellungen korrekt sind, klicke im `Note Exporter` auf die Schaltfläche Exportieren unter deiner Note. Stelle sicher, dass du es in deinen `Beat Saber/CustomNotes` Ordner exportierst, damit du es im Spiel testen kannst.

::: warning WARNUNG
Wenn du eine Notiz erneut exportieren willst, musst du die alte Version löschen. Der Note Exporter exportiert keine Note, wenn sich im selben Ordner bereits eine Notemit demselben Namen befindet.
:::

![Exportiere Note](~@images/models/notes/39.png)

![Exportiere Note](~@images/models/notes/40.png)

Jetzt, wo deine Noten exportiert sind, kannst du Beat Saber starten und sehen, wie sie im Spiel aussehen. Klicke in Beat Saber auf `Mods` und dann `Custom Notes`. Wenn du alles richtig gemacht hast, solltest du deine Noten in der Liste sehen.

![Zeige Note-Vorschau ingame](~@images/models/notes/41.png)

Wähle deine Noten aus und versuche, ein Lied zu spielen.

![Zeige Note Ingame](~@images/models/notes/42.png)

### Mit FPFC eine Vorschau Noten im Spiel anzeigen, ohne das Headset aufzusetzen
First Person Flying Controller (FPFC) ist ein Startparameter, der sowohl von Steam- als auch von Oculus-Nutzern verwendet werden kann. FPFC öffnet eine Instanz von Beat Saber auf deinem Desktop und erlaubt dir, es mit der Tastatur und Maus zu steuern.

While a map is playing, pressing:

* `P` **P**auses the map
* `M` Returns to **m**enu if paused
* `R` **R**estarts the map if paused
* `C` Unpauses and **c**ontinues playing

You will need the SiraUtil mod in order move the camera while a map is playing. Without it, the camera is fixed in the floor at an undesirable angle. Install SiraUtil from Mod Assistant and run Beat Saber to create a config json file. SiraUtil also adds additional useful features such as camera FOV, sensitivity, and rebindable pause and exit controls. Edit the `SiraUtil.json` file in your `UserData` folder to tweak settings.

**For Steam Users:**

Open the game properties and add `fpfc` to the Steam launch options in the General tab. ![Fpfc launch options](~@images/mapping/fpfc.png)

**For Oculus Users:**

1. Klicke mit der rechten Maustaste auf Beat Saber.exe und erstelle eine Verknüpfung.
2. Bearbeite das Ziel, um "fpfc" am Ende hinzuzufügen. Zum Beispiel: `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber.exe" fpfc`

After installing the mods and adding the launch parameter you can then now move around and pause in a map. The default toggle key to switch between headset and mouse/keyboard control is <kbd>G</kbd>.

:::warning NOTE

* If you go back into vr and the game doesn't load in the headset either:
  * Press the <kbd>G</kbd> key until the headset displays the game  
    **==OR==**
  * Quit the game, remove the launch option, and relaunch the game.

* If the mod doesn't seem to be working, make sure the in-game Smooth Camera setting is disabled. :::

If everything looks good ingame, you should be finished! Make sure to try playing with your notes with your headset on at least once before releasing them.

## Custom Colors
This section is assuming you already have a custom note fully set up and simply want to add support for custom colors, which is highly recommended because it will almost always enhance the user experience.

CustomColor support works by tinting the notes to the current player-set color. If your material has a texture, lighter colors will be tinted more, whilst darker colors will be tinted less.

Go ahead and create a new material in the `Materials` folder. With CustomColor support, generally you're going to be using the same material for both the left and right note, so I'm going to name my material `NoteMaterial`.

![Creating a new material](~@images/models/notes/43.png)

Now select the shader you want to use for your note. If you're not sure which shader you want to use, refer back to the `Adding Materials` section of this guide. For my note, I'm going to use `Unlit Glow`.

![Selecting shader](~@images/models/notes/44.png)

Now apply this material to both your NoteLeft mesh and your NoteRight mesh. Make sure to apply it to BOTH!

![Clicking TriangleMesh](~@images/models/notes/71.png)

![Selecting Material](~@images/models/notes/46.png)

![Material auswählen](~@images/models/notes/47.png)

Now that you're done applying the material to all of your note's meshes, go back to the `NoteMaterial` in the inspector. To double check that your notes look good when using CustomColors, try messing around with the `Color` property; this is what property will be changed when the notes are tinted.

![Changing color of material](~@images/models/notes/48.png)

![Farbe des Materials ändern](~@images/models/notes/49.png)

![Farbe des Materials ändern](~@images/models/notes/50.png)

Once you've confirmed that the notes change color when you change the material's `Color` property, go to your note's main GameObject and go to the `NoteDescriptor`. Enable `Uses Note Color` and feel free to mess around with `Note Color Strength`. When Note Color Strength is at 1, it will tint the color with 100% strength. The lower you go from one, the more subtle it will be. For the purposes of this tutorial, I will be leaving `Note Color Strength` at one.

![Enabling uses note color](~@images/models/notes/51.png)

Your note should now be compatible with Custom Colors! Go ahead and re-export it. If you need a refresher, read the section on Exporting up above.

### Custom Colors bei bestimmten Spielobjekten deaktivieren

In some cases, you may want CustomColors to not affect a certain mesh. For example, if you have a part of your model that needs to stay the same color, such as an arrow needing to be white. There is a simple solution to this problem.

In this example, I have two meshes inside of my `LeftNote` object. I want the `TriangleMesh` to be affected by custom colors, but not `SmallerTriangleMesh`.

![Double mesh example](~@images/models/notes/52.png)

![Double mesh hierarchy](~@images/models/notes/53.png)

All you have to do is go into the GameObjects that you do not want to be affected by custom colors and add a `Disable Note Color On GameObject` component. Any GameObject with this component will retain how it looks and not be affected by custom colors.

::: warning WARNING
Remember to apply these changes to all of the notes in your CustomNote!
:::

![Adding a disable note color on gameobject component](~@images/models/notes/54.png)
