---
sidebar: auto
---

# PC Modding

## Vorwort

::: danger BITTE BEACHTE Wenn du Mods verwendest, verstehst du das:

* Du möglicherweise Probleme bekommst, die im normalen Spiel nicht existieren. 99,9% aller Fehler, Abstürzen und Verzögerungen passieren aufgrund von Mods.
* Mods werden durch Updates oft unbrauchbar und das ist normal - Bitte sei geduldig und respektvoll wenn dies passiert. Modder sind Freiwillige mit einem richtigen Leben.
* Beat Games versucht nicht mit Absicht Mods kaputt zu machen. Sie versuchen an der Code-Grundlage zu arbeiten welches manchmal Mods unbrauchbar macht. Dies geschieht aber nicht mit Absicht.

Bitte greife die Entwickler im Bezug mit Problemen bei Mods nicht an. Modder und Entwickler sind zwei verschiedene Gruppen. Sei einfach kein Trottel, ok? :::

Beat Saber unterstützt von Grund auf Custom Songs. Wenn du also nur danach suchst, brauchst du nicht mehr Mods! Es ist aber eine kluge Idee, `SongCore` zu installieren. Diese Mod erweitert die Basisspiel-Funktion, um die Ladezeiten zu verbessern und Funktionen für andere Mods wie den In-Game Downloader, Ranglisten, Playlisten, usw. bereitzustellen.

::: warning Dieser Guide ist für PC Modding in Windows.  
Wenn du eine Quest hast, schau bitte auf der [Quest Modding Seite](/de/quest-modding.md).  
Wenn du auf Linux bist schaue bitte auf die [Linux Seite](/de/modding/linux.md) oder [Qbeat](https://github.com/geefr/beatsaber-linux-goodies/blob/master/README.md) :::

Wenn du an irgendeinem Punkt Probleme haben solltest, gehe einfach zur [Support Seite](./support) und schaue nach ob du herausfinden kannst was falsch lief, bevor du im Discord Server nachfragst. Es besteht die Möglichkeit, das die Antwort auf deine Frage dort bereits existiert!

::: warning Ich habe mir ein Tutorial von Elite Eric angeschaut aber komme nicht weiter. Wie kommts? BSMG rät **stark** davon ab, jegliche Beat Saber Tutorials von Elite Eric zu verweden. Nach Überprüfung seiner Videos haben wir festgestellt, dass sie viele unvollständige, fehlerhafte oder geradezu falsche Informationen enthalten. Versuche, auf ihn zuzugehen, um diese Fehler zu korrigieren wurden leider mit schweigen und neuen (immer noch falschen) Tutorials erfüllt.

Stattdessen solltest du den schriftlichen Anleitungen hier im Wiki folgen oder Hilfe im [BSMG Discord](https://discord.gg/beatsabermods) suchen. :::

## Installationsprogramme

### Mod Assistant
> **DIES IST AKTUELL DER EMPFOHLENE MOD INSTALLER.**

__**Starte das Spiel mindestens einmal**** bevor du versuchst Mods zu installieren! Dies trifft auch zu wenn du dein Spiel neu installierst.

Ein einfacher Beat Saber Mod Installer, ähnlich dem Mod Manager aber mit zusätzlichen Funktionen wie Deinstallation von Mods und Versionskontrolle! Hol es auf [Assistant's GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Wie bekomme ich mehr Songs
::: tip Die meisten Maps in den Sortierfiltern "Top All", "Rating", "Downloads" oder "Plays" wurden erstellt, bevor gute Mapping-Praktiken etabliert wurden. Versuche Songs herunterzuladen, die zwischen Ende 2019 und jetzt veröffentlicht wurden, um die beste benutzerdefinierten Levels zu erleben. :::

::: warning It is a good idea to backup your `CustomLevels` folder periodically as there is a small chance it will be reset if the game updates!

This folder is located in your game install: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### InGame Downloader
The `BeatSaver Downloader` mod allows you to download maps in-game using the `MORE SONGS` menu button on the `MODS` menu screen. This pulls maps directly from [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) is the master repository of custom songs made by the community. Many other tools and sites enhance the experience of downloading custom songs, but this site is where they are stored. To install songs downloaded from the site, unzip them into a folder and place it into `Beat Saber/Beat Saber_Data/CustomLevels`. You can also use the in-game downloader mod, or Mod Assistant's OneClick™ Install feature.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) is a site that tries to help make finding fantastic maps to play easier. It does this by categorizing the thousands of songs on beatsaver and lets you sort by a song's genre and many other attribute tags. It also has a full social feature where players can review songs and comment on them. One of the most used features is the "Curator Recommended" feature where a team plays through most songs released each day and recommends the ones that stand out, letting you [automatically download these in-game](https://bsaber.com/beatsync/).

### Song Management Apps

There are no working song management apps available at this time.

### Playlists
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* Das `Install Playlist` Tool in den Optionen des Mod Assistant verwenden.
* Platziere die Playlist-Datei in `Beat Saber/Playlists` und wähle diese im Spiel aus. Klicke dann auf Download.

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

## Installationspfad
_Where is Beat Saber installed?_

### Standard Installations-Ordner
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Andere Installationspfade
**If you have moved your install folder to a different drive, it might be in the location below.** Replace the drive letter `F` with the drive your game is installed on.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Manuelle Installation
A mod installer is the recommended way to install mods. See the section [above](#installers). If you have patched the game and just need to install mods that are not available in the installer, skip to step 4.

**Run the game at least once** before trying to mod the game! This applies to reinstalling your game too.

### BSIPA installieren

1. Lade [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases) herunter.
2. Begib dich zu deinem [Installationsordner.](#installationspfad) und entpacke den Inhalt des Archivs in diesen Ordner. ![Directory Clean](~@images/beginners-guide/directory-clean.png "Directory Clean") ![Directory Ipa](~@images/beginners-guide/directory-ipa.png "Directory Ipa")
3. Doppelklicke auf IPA.exe um das Spiel zu patchen. Alle Mods im Ordner `Plugins` werden ab sofort geladen, wenn das Spiel gestartet wird. Sollte es Fehler geben, hast du etwas in Schritt 2 nicht richtig gemacht. ![Directory Patched](~@images/beginners-guide/directory-patched.png "Directory Patched")

### Mods installieren

4. Lade die Mod(s) herunter die du installieren möchtest. Sei es von GitHub, dem [BSMG Discord](https://discord.com/invite/beatsabermods) `#pc-mods` Kanal, [BeatMods](https://beatmods.com/#/mods) oder anderen Quellen. **Stell sicher, dass du alle Dependncies herunterlädst, die vom Mod benötigt werden.** ![Directory Plugins](~@images/beginners-guide/directory-plugins.png "Directory Plugins")
5. Einige Mods haben Installationsanweisungen, andere nicht. In der Regel kann man einfach die ZIP-Datei im Beat Saber Installationsordner ziehen und entpacken. Die Dateien werden dann in die entsprechenden Ordner entpackt.

## Wie man Mods deinstalliert
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## Hilfe von der Community

* [Griffe und Tricks](./grips-and-tricks.md)
* [Erstelle Beatmaps](/de/mapping/)
* [Custom Sabers](/de/models/custom-sabers.md)
* [Custom Avatars](/de/models/custom-avatars.md)
* [Custom Platforms](/de/models/custom-platforms.md)
* [Play Customs in Multiplayer](https://discord.com/invite/gezGrFG4tz)
* [Mods erstellen](/de/modding/)

## Hast Du Fragen?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
