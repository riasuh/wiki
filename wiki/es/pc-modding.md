---
sidebar: auto
---

# Mods en PC

## Prólogo

::: danger Descargo de responsabilidad Al elegir usar mods, entiendes que:

* Puede que experimentes problemas que no existen en el juego base. El 99,9% de los errores, fallos y lag se deben a mods.
* Los Mods están sujetos a romperse por actualizaciones y eso es normal - sed pacientes y respetuosos cuando esto suceda, ya que los modders son voluntarios con vidas reales.
* Beat Games no trata de romper los mods a proposito. Quieren trabajar en la base de código y a veces esto rompe los mods, pero no están decididos a matar los mods.

No atacar a los desarrolladores por problemas relacionados con mods, y viceversa - los modders y los desarrolladores son dos grupos separados. Simplemente no seas un cretino ok? :::

:::warning STAY SAFE WHEN INSTALLING MODS Beat Saber will **NEVER** ask you to run it as Administrator.

If you've downloaded and installed a mod and you get the User Account Control prompt, **DO NOT** click accept, and please report this. What you installed is a malicious mod!

If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

Beat Saber natively supports custom songs, so if that's all you're looking for, you don't require more mods! It's a wise idea to install `SongCore` though, as this mod expands upon the base game functionality to improve loading times and provide functionality for other mods like the in-game downloader, custom leaderboards, playlists, etc.

::: warning This guide is for PC-modding on Windows.  
If you have a Quest, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux page](/modding/linux.md) or [QBeat](https://github.com/geefr/beatsaber-linux-goodies/blob/master/README.md) :::

If you run into problems at any point, please head to the [support page](./support) and see if you can identify what went wrong before asking in the Discord server. Chances are, your answer is on that page!

::: warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** suggest against using video tutorials for modding. Often, we find they are outdated or contain a incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Instaladores

### Asistente de mods
> **ESTE ES ACTUALMENTE EL INSTALADOR RECOMENDADO.**

__**Run the game at least once**** before trying to mod the game! This applies to reinstalling your game too.

A simple Beat Saber Mod Installer similar to the mod manager, but with additional features such as mod removal and version checking! Get it on [Assistant's GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Cómo obtener más canciones
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

::: warning It is a good idea to backup your `CustomLevels` folder periodically as there is a small chance it will be reset if the game updates!

This folder is located in your game install: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### Descargador en el juego
The `BeatSaver Downloader` mod allows you to download maps in-game using the `MORE SONGS` menu button on the `MODS` menu screen. This pulls maps directly from [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) is the master repository of custom songs made by the community. Many other tools and sites enhance the experience of downloading custom songs, but this site is where they are stored. To install songs downloaded from the site, unzip them into a folder and place it into `Beat Saber/Beat Saber_Data/CustomLevels`. You can also use the in-game downloader mod, or Mod Assistant's OneClick™ Install feature.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) is a site that tries to help make finding fantastic maps to play easier. It does this by categorizing the thousands of songs on beatsaver and lets you sort by a song's genre and many other attribute tags. It also has a full social feature where players can review songs and comment on them. One of the most used features is the "Curator Recommended" feature where a team plays through most songs released each day and recommends the ones that stand out, letting you [automatically download these in-game](https://bsaber.com/beatsync/).

### Herramientas de administración de canciones

There are no working song management apps available at this time.

### Listas De Reproducción
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* Use the `Install Playlist` tool in the Options tab of Mod Assistant.
* Place the playlist file into `Beat Saber/Playlists`, select it in-game, then hit download all songs.

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

## Carpeta de instalación
_Where is Beat Saber installed?_

### Ubicación Predeterminada
|        |                                                                                             |
| ------ | ------------------------------------------------------------------------------------------- |
| Steam  | `C:\Archivos de programa (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Archivos de programa\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Otras Ubicaciones
**If you have moved your install folder to a different drive, it might be in the location below.** Replace the drive letter `F` with the drive your game is installed on.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Instalación manual
A mod installer is the recommended way to install mods. See the section [above](#installers). If you have patched the game and just need to install mods that are not available in the installer, skip to step 4.

::: warning STAY SAFE WHEN INSTALLING MODS Modding your game with unverified mods such as mods found in the `#pc-mods` channel comes with risks, including the possibility for malicious software that acts like a regular mod.

Beat Saber will **NEVER** ask you to run it as Administrator.

If you've downloaded and installed a mod and you get the User Account Control prompt, **DO NOT** click accept, and please report this. If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

**Run the game at least once** before trying to mod the game! This applies to reinstalling your game too.

### Instala BSIPA

1. Descarga [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Ve a tu [carpeta de instalación.](#install-folder) y extrae el contenido de BSPIA en ella. ![Directorio Limpio](~@images/beginners-guide/directory-clean.png "Directorio Limpio") ![Directorio lpa](~@images/beginners-guide/directory-ipa.png "Directorio Ipa")
3. Haga doble clic en IPA.exe para parchear el juego. Cualquier mod en la carpeta `Plugins` ahora se cargará al iniciar el juego. Si hay errores, probablemente no seguiste el paso 2 correctamente. ![Directorio Parcheado](~@images/beginners-guide/directory-patched.png "Directorio Parcheado")

### Instalar mods

4. Descarga el(los) mod(s) que deseas instalar, ya sea desde GitHub, en el [Discord BSMG](https://discord.com/invite/beatsabermods) el canal `#pc-mods`,  [BeatMods](https://beatmods.com/#/mods) u otras fuentes. **Asegúrate de descargar las dependencias requeridas por el mod.** ![Directorio Plugins](~@images/beginners-guide/directory-plugins.png "Directorio Plugins")
5. Algunos mods tienen instrucciones de instalación, algunos no. Generalmente puedes simplemente arrastrar y soltar el contenido zip en tu carpeta de instalación de Beat Saber, y los archivos deberían ir a las carpetas correspondientes.

## Cómo desinstalar mods
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## A dónde ir a partir de aquí

* [Grips and Tricks](./grips-and-tricks.md)
* [Making Beatmaps](/mapping/)
* [Custom Sabers](/models/custom-sabers.md)
* [Custom Avatars](/models/custom-avatars.md)
* [Custom Platforms](/models/custom-platforms.md)
* [Play Customs in Multiplayer](https://discord.com/invite/gezGrFG4tz)
* [Making Mods](/modding/)

## ¿Tienes alguna pregunta?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
