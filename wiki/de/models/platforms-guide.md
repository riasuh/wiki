---
sidebar: auto
prev: ./avatars-guide.md
next: ./notes-guide.md
description: Emmas Leitfaden zur Erstellung von Custom Platforms!
---

# Custom Platforms Guide
_Emmas Leitfaden zur Erstellung von Custom Platforms._

## Projekt
Open the current [Custom Platforms Project](https://github.com/affederaffe/CustomPlatformsUnityProject/releases/) with [Unity 2018.1.6f1](https://download.unity3d.com/download_unity/57cc34175ccf/Windows64EditorInstaller/UnitySetup64-2018.1.6f1.exe).

## Erste Schritte
![Custom Platform Skript](~@images/models/platforms/CustomPlatformScript.png)

Erstelle ein `Leeres Spielobjekt`, indem du mit der rechten Maustaste in das Hierarchiefenster klickst und `"Leeres Objekt erstellen"` auswählst. Stelle sicher, dass seine Position im Inspektor auf den Ursprung (0,0,0) gesetzt wird. Suche im Inspektor nach dem Skript `Custom Platforms` und wende es auf dieses GameObject an. Alles, was sich in diesem Objekt befindet, wird exportiert, wenn die Schaltfläche im `Custom Platforms` Skript gedrückt wird. Im Skript gibt es auch Optionen zum Exportieren. Diese deaktivieren Teile der Originalplattform (Für den Fall, dass du etwas teilweise ersetzen möchtest).

## Modelle hinzufügen
![Objekte](~@images/models/platforms/Objects.png)

Drag all models you want in your Platform into the GameObject created in the second step and position them to your liking. Stelle für die Materialien der Modelle sicher, dass Beat Saber kompatible Shader verwendest oder die, die du im Projekt findest, `_dark_replace` und `_glow_replace` im Namen haben. Dies sind benutzerdefinierte Materialien, die sich wie die Beat Saber Materialien verhalten, d. h. auf die Röhrenleuchten und den Nebel reagieren.

### Track Rings
Das `Track Rings ` Skript macht Track Rings wie man sie im Spiel sieht. Um dies zu erreichen, nimmt das Skript ein Prefab. Currently I haven't been able to figure out how to use a prefab in it, so I used a gameObject, that is part of the platform hierarchy, that I later moved off to `y = -1000`. For the ring-preview to show correctly, move this gameObject to (0,0,0) and adjust your settings and before importing move it off to somewhere offscreen.

Die Aktivierung des Rotationseffekts bewirkt, dass sich die Ringe um das angegebene Ereignis drehen, abhängig von den angegebenen Variablen. (Ich habe mit den noch nicht herumgespielt, also experimentiere am besten).

Das Aktivieren des Stufeneffekts ändert die Ringabstände, wenn das angegebene Ereignis zwischen 2 Variablen aufgerufen wird.

![Track Rings Skript](~@images/models/platforms/TrackRingsScript.png)

### Röhren Licht
![Röhren Licht](~@images/models/platforms/TubeLightScript.png)

Dieses Skript aktiviert blinkende Lichter. Putting this on an empty gameObject changes the background and adds a bit of color to that space, according to the light ID's. When there's also a mesh renderer on it, it'll change the meshes color according to the light ID's. When using this no color adding is needed, so I change the size on the script to 0.

### Song Events
![Song Event Handler](~@images/models/platforms/SongEventHandler.png)

The event manager is the most useful script. With it you can trigger an action on any beat saber event (even unused ones). Um ein Event hinzuzufügen, drücke die Taste `+` unterhalb von `Auslöser ()`. Drag in the object you want to manipulate into the box that just got created. Press the dropdown menu to the right and choose what that object should do, by first selecting what component, then what action. Make sure that you only use 1 event Handler per gameObject, as only 1 will work per gameObject.

### Spectogram
![Spectogram](~@images/models/platforms/Spectogram.png)

The spectrogram script works like the track rings script and also requires a prefab or gameObject. This will get stretched and shrunk according to the sound of the game and the variables provided. (Haven't played with this either).

## Exportieren

![Saving](~@images/models/platforms/Save.png)

Export the platform trough the script that you previously added to the gameObject to the location of your choosing. Preferably the game's directory `Beat Saber/CustomPlatforms`.

::: tip NOTE **Once you've got your new platform working**, [upload them to ModelSaber](https://modelsaber.com) if you want to share them with the world. :::

![Cat](~@images/models/platforms/Cat.png)
