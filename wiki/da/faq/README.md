# Ofte Stillede Spørgsmål

## Jeg har lige fået spillet. Hvordan kommer jeg i gang?
Check out our [beginner's guide](/beginners-guide.md)!

## Hvordan får jeg flere baner?
> [BeatSaver](https://beatsaver.com) er hovedarkivet for brugerskabte baner fra fællesskabet. Mange andre værktøjer og websteder forbedrer oplevelsen af at downloade brugerskabte baner, men dette er stedet, hvor de er opbevaret.

Hvis du henter baner manuelt fra BeatSaver, så udpak dem i en mappe og placér filerne i `Beat Saber/Beat Saber_Data/CustomLevels`. Dette er den mappe, som spillet indbygget læser brugerskabte baner fra.

### BeastSaber
[Beast Saber](https://www.bsaber.com) is a review site that aims to curate all of the songs on BeatSaver. You can also download playlists, follow mappers, find songs using advanced sorting methods and more.

### Sangstyringsværktøjer

There are no working song management apps available at this time.

## Hvordan installere jeg playlister?

### PC
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* Use the `Install Playlist` tool in the Options tab of Mod Assistant.
* Place the playlist file into `Beat Saber/Playlists`, select the playlist title header in-game, then hit download all songs.

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

### Quest
You can use [Playlist Editor Pro](https://beatsaberquest.com/bmbf/my-tools/playlist-editor-pro/) to manage the playlists on your Quest. Note that a custom level can only appear once in-game due to a limitation with BMBF.

:::warning WARNING for Quest Users Reloading your Custom Songs Folder resets all playlist organization. :::

## How do I make my own custom levels?
See [mapping](/mapping/)!

## How do I load PC mods that aren't in Mod Assistant?
See [this section](/pc-modding.md#manual-installation) in the beginners guide.

## Does multiplayer have crossplay?
Officially, multiplayer is limited to playing with other people in the store version (Oculus/Steam) you purchased. Additionally, modifying the game on Quest disables official multiplayer.

The BeatTogether mod is the current solution for cross-platform play between the modded game versions. Join their [Discord server](https://discord.com/invite/gezGrFG4tz) and check the `#install-instructions` channel for more information.

## My game updated and now none of my mods are working
Each time the game updates it is possible *(and very likely)* that your existing mods will stop working and need to be updated. To make sure your install will not break when the game runs on a new update for the first time, everything in the `Plugins` folder is automatically moved into a new folder called `Old 1.xx.x Plugins`. **Leave those plugins/mods in there!**

To get mods back, simply **run the installer again.**  
The BeatMods repository only includes mods that have been confirmed to work on the latest version of the game!

If you're confused by any of this, visit [Beginners Guide](/beginners-guide.md).

## How does the scoring system work in Beat Saber? How does global ranking work?
We have sections on the [grips and tricks](/grips-and-tricks.md) page dedicated to the scoring and ranking systems, check them out!

## My menus are blank and I have nothing to click on
If the main window in your game is blank, your save file likely got corrupted.

To fix it, navigate to: `%AppData%\..\LocalLow\Hyperbolic Magnetism`

Delete or rename the Beat Saber folder to something else. When you re-enter the game, it'll recreate the save file and should load the main menu properly.
