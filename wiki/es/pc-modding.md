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

Beat Saber soporta nativamente canciones personalizadas, así que si es todo lo que estás buscando, no necesitas más mods! Sin embargo, es una buena idea instalar `SongCore`, ya que este mod se expande sobre la funcionalidad base del juego para mejorar los tiempos de carga y proporcionar funcionalidad para otros mods como las descargas desde el juego, marcadores personalizados, listas de reproducción, etc.

::: warning Esta guía es para modear PC en Windows.  
Si tienes unas Quest, consulta la [página de Modding de Quest](/quest-modding.md).  
Si estás en Linux, mira la página [de Linux](/modding/linux.md) o [QBeat](https://github.com/geefr/beatsaber-linux-goodies/blob/master/README.md) :::

Si encuentras problemas en cualquier momento, por favor dirígete a la [página de soporte](./support) y mira si puedes identificar lo que salió mal antes de preguntar en el servidor de Discord. ¡Es posible que tu respuesta esté en esa página!

::: warning He visto este video de Elite Eric, pero me he quedado atascado/no funcionó. ¿Qué proporciona? En BSMG **sugerimos encarecidamente** no usar ningún tutorial de Elite Eric. Después de revisar gran parte de su contenido, contienen una gran cantidad de información incompleta, errónea o directamente incorrecta. Desgraciadamente, los intentos de contactar con el para corregir estos errores se han encontrado con silencio y nuevos (también incorrectos) tutoriales.

En su lugar, deberías seguir las guías escritas aquí en la wiki o buscar ayuda en [el discord de BSMG](https://discord.gg/beatsabermods). :::

## Instaladores

### Asistente de mods
> **ESTE ES ACTUALMENTE EL INSTALADOR RECOMENDADO.**

__**¡Ejecuta el juego al menos una vez**** antes de intentar moddear el juego! Esto también se aplica a la reinstalación de tu juego.

Un simple instalador de Mods de Beat Saber similar al gestor de mods, pero con características adicionales como eliminación de mod y verificación de versiones! Consíguelo en [Asistente de GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Cómo obtener más canciones
::: tip La mayoría de los mapas en los filtros "Top general", "Clasificación", "Descargas" o "Jugadas" se crearon antes de que se establecieran las buenas prácticas de mapeo. Intenta descargar canciones publicadas entre finales de 2019 y ahora para obtener la mejor experiencia de niveles personalizados. :::

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
