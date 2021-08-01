---
sidebar: auto
---

# Modding en PC

## Prólogo

::: danger Descargo de responsabilidad al elegir usar mods, entiendes que:

* Puede que experimentes problemas que no existen en el juego base. El 99,9% de los errores, fallos y lag se deben a mods.
* Los Mods son subceptibles de romperse por actualizaciones y eso es normal - sed pacientes y respetuosos cuando esto suceda, ya que los modders son voluntarios con vidas reales.
* Beat Games no trata de romper los mods a proposito. Quieren trabajar en la base de código y a veces esto rompe los mods, pero no están decididos a matar los mods.

No ataques a los desarrolladores por problemas relacionados con mods, y viceversa - los modders y los desarrolladores son dos grupos separados. Simplemente no seas un cretino ok? :::

:::warning MANTENTE SEGURO CUANDO INSTALES MODS Beat Saber **NUNCA** te pedirá que lo ejecutes como Administrador.

Si has descargado e instalado un mod y te aparece el panel de control de cuentas de usuario, **NO** hagas clic en aceptar, y por favor informa de esto. ¡Lo que has instalado es un mod malicioso!

Si no estás seguro de si algo que has instalado es software malicioso o no, *** por favor pregunta a alguien en nuestro discord***. :::

Beat Saber soporta de forma nativa canciones personalizadas, así que si eso es todo lo que buscas, ¡no necesitas más mods! Sin embargo es una buena idea instalar `SongCore`, puesto que este mod amplía la funcionalidad base del juego para mejorar los tiempos de carga y provee funcionalidad para otros mods como el descargador dentro del juego, clasificaciones personalizadas, listas de reproducción, etc.

::: warning Esta guía es para modificaciones en PC sobre Windows.  
Si tienes un dispositivo Quest, mira la [página Modding en Quest ](/quest-modding.md).  
Si estás en Linux, revisa la[página de Linux](/modding/linux.md) o [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

Si encuentras problemas en cualquier momento, por favor dirígete a la [página de soporte](./support) y mira si puedes identificar lo que salió mal antes de preguntar en el servidor de Discord. ¡Lo más probable es que tu respuesta esté en esa página!

::: warning He visto un video tutorial en YouTube, pero me he quedado atascado/no ha funcionado. ¿Qué sucede? Aquí en BSMG recomendamos **encarecidamente** que no se utilicen tutoriales en vídeo para el modding. A menudo, nos encontramos con que están desfasados o contienen una información incompleta, errónea o directamente incorrecta.

En su lugar, deberías seguir las guías escritas aquí en la wiki o buscar ayuda en [el discord de BSMG](https://discord.gg/beatsabermods). :::

## Instaladores

### Asistente de mods
> **ESTE ES AHORA MISMO EL INSTALADOR RECOMENDADO.**

__**¡Ejecuta el juego al menos una vez**** antes de intentar modificar el juego! Esto también se aplica al reinstalar tu juego.

¡Un simple instalador de Mods de Beat Saber similar al gestor de mods, pero con características adicionales como eliminación de mods y verificación de versiones! Consíguelo en la [página de Github de Assiistant](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Cómo obtener más canciones
::: tip La mayoría de los mapas en los filtros "Top general", "Clasificación", "Descargas" o "Jugadas" se crearon antes de que se establecieran las buenas prácticas de mapeo. Prueba a descargar las canciones publicadas entre finales de 2019 y el día de hoy para obtener la mejor experiencia en niveles personalizados. :::

::: warning ¡Es una buena idea hacer una copia de seguridad de tu carpeta `CustomLevels` periódicamente ya que hay una pequeña posibilidad de que se resetee si el juego se actualiza!

Esta carpeta se encuentra en tu instalación del juego: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### Descargador dentro del juego
El mod `BeatSaver Downloader` te permite descargar mapas dentro del juego usando el botón `MORE SONGS` del menú en la pantalla `MODS` del menú. Este extrae los mapas directamente de [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) es el repositorio principal de canciones personalizadas hechas por la comunidad. Muchas otras herramientas y sitios mejoran la experiencia de descargar canciones personalizadas, pero este sitio es donde se almacenan. Para instalar las canciones descargadas del sitio, descomprímelas en una carpeta y colócalas en `Beat Saber/Beat Saber_Data/CustomLevels`. También puedes utilizar el descargador de mods dentro del juego o la función de instalación OneClick™ de Mod Assistant.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) es un sitio que intenta facilitar la búsqueda de fantásticos mapas para jugar. Para ello, clasifica las miles de canciones de BeatSaver y permite ordenarlas por su género y muchas otras etiquetas de atributos. También tiene una característica social completa en la que los jugadores pueden revisar las canciones y comentarlas. Una de las funciones más utilizadas es la función "Curator Recommended", en la que un equipo reproduce la mayoría de las canciones publicadas cada día y recomienda las que destacan, permitiéndote [descargarlas automáticamente en el juego](https://bsaber.com/beatsync/).

### Herramientas de administración de canciones

En este momento no hay aplicaciones de gestión de canciones que funcionen.

### Listas De Reproducción
Necesitas instalar el mod [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest).

Entonces puedes:

* Utilizar la herramienta `Install Playlist` en la pestaña Options de Mod Assistant.
* Colocar el archivo de la lista de reproducción en `Beat Saber/Playlists`, selecciónarlo en el juego y luego pulsar descargar todas las canciones.

Deberías ver la lista de reproducción junto al álbum de niveles personalizados en el juego. El mod también admite la gestión de listas de reproducción en el juego.

## Carpeta de instalación
_¿Dónde está instalado Beat Saber?_

### Ubicación Predeterminada
|        |                                                                                             |
| ------ | ------------------------------------------------------------------------------------------- |
| Steam  | `C:\Archivos de programa (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Archivos de programa\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Otras Ubicaciones
**Si has movido tu carpeta de instalación a una unidad diferente, podría estar en la ubicación que se indica a continuación.** Sustituye la letra de la unidad `F` por la unidad en la que está instalado tu juego.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Instalación manual
Un instalador de mods es la forma recomendada de instalar mods. Mira la sección [arriba](#installers). Si has parcheado el juego y sólo necesitas instalar mods que no están disponibles en el instalador, salta al paso 4.

::: warning MANTENTE SEGURO AL INSTALAR MODS Modificar tu juego con mods no verificados, como los que se encuentran en el canal `#pc-mods`, conlleva riesgos, como la posibilidad de que un software malicioso actúe como un mod normal.

Beat Saber **NUNCA** te pedirá que lo ejecutes como Administrador.

Si has descargado e instalado un mod y te aparece el panel de control de cuentas de usuario, **NO** hagas clic en aceptar, y por favor informa de esto. Si no estás seguro de si algo que has instalado es malware o no, ***pregunta a alguien en nuestro discord***. :::

**¡Ejecuta el juego al menos una vez** antes de intentar modificar el juego! Esto también se aplica al reinstalar tu juego.

### Instala BSIPA

1. Descarga [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Ve a tu [carpeta de instalación.](#install-folder) y extrae el contenido de BSPIA en ella. ![Directorio Limpio](~@images/beginners-guide/directory-clean.png "Directorio Limpio") ![Directorio lpa](~@images/beginners-guide/directory-ipa.png "Directorio Ipa")
3. Haz doble clic en IPA.exe para parchear el juego. Cualquier mod en la carpeta `Plugins` ahora se cargará al iniciar el juego. Si hay errores, probablemente no seguiste el paso 2 correctamente. ![Directorio Parcheado](~@images/beginners-guide/directory-patched.png "Directorio Parcheado")

### Instalar mods

4. Descarga el(los) mod(s) que deseas instalar, ya sea desde GitHub, en el el canal `#pc-mods` del [Discord de BSMG](https://discord.com/invite/beatsabermods),  [BeatMods](https://beatmods.com/#/mods) u otras fuentes. **Asegúrate de descargar las dependencias requeridas por el mod.** ![Directorio Plugins](~@images/beginners-guide/directory-plugins.png "Directorio Plugins")
5. Algunos mods tienen instrucciones de instalación, otros no. En general puedes simplemente arrastrar y soltar el contenido zip en tu carpeta de instalación de Beat Saber, y los archivos deberían ir a las carpetas correspondientes.

## Cómo desinstalar mods
O bien eliminas la dll de la carpeta `Plugins`, o haces clic en el botón `Desinstalar` en Mod Assistant.

## A dónde ir a partir de aquí

* [Agarres y trucos](./grips-and-tricks.md)
* [Creando mapas de ritmo](/mapping/)
* [Sables personalizados](/models/custom-sabers.md)
* [Avatares personalizados](/models/custom-avatars.md)
* [Plataformas personalizadas](/models/custom-platforms.md)
* [Jugar canciones personalizas en modo multijugador](https://discord.com/invite/gezGrFG4tz)
* [Creando Mods](/modding/)

## ¿Tienes alguna pregunta?
¡Visita los canales de soporte en el [Discord de BSMG](https://discord.gg/beatsabermods)!
