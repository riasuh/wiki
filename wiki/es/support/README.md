---
sidebar: auto
---

# Soporte

## Índice

0. [Actualizaciones](#_0-updates)
1. [¿No hay mods?](#_1-no-mods)
2. [Problemas de juego después de la modificación](#_2-game-issues-post-modding)
3. [Preguntas comunes](#_3-common-questions)
4. [Solución de problemas varios](#_4-miscellaneous-troubleshooting)
5. [¿Aún tienes problemas?](#_5-still-having-issues)

## 0. Actualizaciones
Después de una actualización, el canal de discord de BSMG `#modding-announcements` debería tener la información más actualizada sobre el estado de los mods. A continuación se ofrecen instrucciones más detalladas del procedimiento más habitual.

### Una actualización ha roto mis mods
**Ejecuta el juego una vez** en la nueva actualización. A continuación, vuelve a instalar tus mods utilizando un instalador listado en la [guía de principiantes](/beginners-guide), como Mod Assistant.

## 1. ¿No hay mods?

### Preguntas diversas

#### 1.1 No aparecen mods en una copia nueva del juego
En primer lugar, asegúrate de que lo siguiente es correcto:

* **Has ejecutado el juego una vez antes de instalar los mods**. BSIPA elimina todos los mods en la primera ejecución de una nueva actualización para evitar que se carguen los mods antiguos que no funcionen en una nueva versión. Vuelve a instalar los mods si este es el caso.
* Steam/Oculus está lanzando Beat Saber desde la **misma instalación** en la que están los mods. *por ejemplo, los mods están en la unidad D pero steam se lanza desde la unidad C.* Establece la ubicación de instalación correcta en tu instalador elegido.
* Si has instalado mods manualmente, asegúrate de que has incluido todos los archivos de la descarga y los has colocado en las carpetas correctas así como sus dependencias.

#### 1.2 Tenía mods instalados en una versión anterior, pero no se carga nada después de una actualización
Si los detalles del apartado 1.1 son correctos, prueba las soluciones siguientes, en orden descendente.

##### Solución 1

* Actualiza BSIPA a la última versión (en Mod Assistant o manualmente)
* Ve a tu carpeta de Beat Saber
* Ejecuta `IPA.exe`

##### Solución 2 (Sólo Steam)

* [Verifica tus archivos del juego](#verify-game-files-for-steam)
* Actualiza BSIPA a la última versión
* Ve a tu carpeta de Beat Saber
* Ejecuta `IPA.exe`

##### Solución 3

* Ve a tu carpeta de Beat Saber
* Haz una copia de seguridad de la carpeta `UserData` (opcional)
* Borra UserData

::: warning ¡Esto restablecerá todos los ajustes del mod! :::

##### Solución 4

* Realiza una [instalación limpia](#clean-installation)

#### 1.2 Mod Assistant no parece instalar ningún mod
Los instaladores descargan los mods en `Beat Saber/IPA/Pending`, BSIPA mueve estos archivos a la carpeta raíz cuando se lanza el juego. Si la carpeta Plugins del juego sigue vacía después de esto, ejecuta de nuevo `IPA.exe` y asegúrate de que nada impide su ejecución, por ejemplo que se ejecute, `algún antivirus, permisos de administrador, etc.`

## 2. Problemas del juego después de la modificación

### El juego no arranca

#### 2.1 Error GetThreadContext falló
Si aparece una ventana que dice `GetThreadContext Failed` y/o escuchas un sonido de error de Windows, es posible que tengas un software en tu PC que rompe los mods de Beat Saber. Muchos programas antitrampas de terceros como ESEA y FaceIt impiden que BSIPA aplique mods a Beat Saber, incluso cuando no se ejecutan. Algunos programas antivirus también muestran un comportamiento similar.

Para resolver este problema:

1. Desinstala el sofware antitrampas.
2. Reinicia tu PC.
3. Comprueba si todavía existen restos del software en las carpetas dentro de `AppData`.
4. Ejecuta el juego. Si los problemas persisten entonces prueba lo siguiente: `Nota adicional: El problema puede seguir persistiendo por falta de permisos o excepciones, cualquier programa que pueda
bloquear BSIPA, o programas marcados como sospechosos pueden hacer que este problema persista`. Steam: [Verifica los archivos de juego de Steam](#verify-game-files-for-steam) Oculus: Realiza una [Instalación limpia](#clean-installation)

Esto debería solucionar el problema.

#### 2.2 Congelado al iniciar
Si el juego se congela en la pantalla de Salud y Seguridad, o ves un avatar en forma de T sin poder controlar el juego, [verifica tus archivos](#verify-game-files-for-steam) si tienes el juego en Steam, o reinstala el juego en Oculus Home. Consulta [Instalación limpia](#clean-installation)

Esto parece ocurrir cuando se actualiza Beat Saber y se tienen mods instalados previamente, pero no a los usuarios con instalaciones limpias del juego.

### Problemas en la tasa de fotogramas

#### 2.3 El juego se para de forma insufrible después de instalar mods
Si el juego se retrasa tanto que apenas puedes pulsar el botón `Continuar` en la pantalla de Salud & Seguridad, entonces verifica los archivos si tienes el juego en Steam, o reinstala el juego en Oculus Home. Haz lo mismo si no se inicia en absoluto y no muestra ningún mensaje de error al intentar iniciar el juego.

Si eso no ha solucionado el problema, entonces revisa la sección [2.4 Mejorar la tasa de fotogramas](#_2-4-improving-framerate)

#### 2.4 Mejorar la tasa de fotogramas
Si [2.3](#2-3-the-game-stutters-unbearably-after-installing-mods) no ha mejorado tus FPS, entonces tu PC podría simplemente estar combatiendo el estrés causado por los mods. Aquí hay algunas cosas que puedes hacer para mejorar la tasa de fotogramas, sin ningún orden en particular:

* Comprueba si NVIDIA GEFORCE EXPERIENCE ha configurado la escala de renderizado para Beat Saber más allá del valor predeterminado de 1,0. Es posible que lo haya ajustado a un número superior a 1,4 o 1,8, lo que aumenta considerablemente la carga de la GPU.
* Usa una avatar personalizado menos complejo.
* Los sables personalizados **Plasma Katanas** tienen toneladas de eventos personalizados y son conocidos por introducir lag si fallas.
* Camera2 y CameraPlus pueden ser muy exigentes, especialmente si tienes varias cámaras o aumentas el ángulo de visión.
* Desactiva la Escala de renderización, el Anti-Aliasing, el modo espejo, la niebla, etc. en los ajustes del juego base.
* Para los jugadores de Oculus Rift (CV1): considera el uso de 2 sensores en lugar de 3+.
* Reduce tu número total de mods y canciones.
* Realiza una [instalación limpia](#clean-installation) de los archivos del juego.
* La baja tasa de fotogramas también puede ser causada por algo que va mal dentro de su carpeta de datos de la aplicación, consulta [Borrar la carpeta de Beatsaber dentro de AppData](#deleting-your-save-in-appdata)
* Desactiva contadores de Counters+ como el contador de puntuación y la velocidad de balanceo, ya que pueden consumir bastante.
* HTTPStatus y DataPuller pueden causar picos de lag. Prueba sin este mod para ver si los picos de lag desaparecen.

La realidad virtual requiere de un uso intensivo de la CPU, especialmente si se añaden mods. Si tienes problemas para ejecutar el juego con los mods que deseas, considera actualizar tu hardware. Ten en cuenta que Beat Saber no utiliza mucho la GPU ya que visualmente es un juego bastante sencillo.

## 3. Preguntas habituales

### Varias

#### 3.1 Menú en blanco, sin botones
Si tu ventana principal del juego está en blanco, es probable que tu archivo de guardado se haya corrompido. Para solucionar esto, consulta [Borrar la carpeta de Beatsaber dentro de AppData](#deleting-your-save-in-appdata)

::: warning Esto borrará tus resultados locales y las estadísticas. :::

#### 3.2 ¿Cómo se utiliza el mod `x`?
Si utilizas Mod Assistant, haz clic en el mod y pulsa el botón "Información del mod". [BeatMods](http://beatmods.com) tiene un botón de "Más información" en cada mod también.

#### 3.3 Problemas con la vibración
Gameplay Modifiers Plus tenía un interruptor para activar/desactivar la vibración del mando. Si lo has desactivado y luego has eliminado el mod, tendrás que modificar manualmente el archivo de datos de guardado en el que se escribe. Abre `%appdata%\..\LocalLow\Hyperbolic Magnetism\Beat Saber\settings.cfg` y establece `controllersRumbleEnabled` a `true`.

Si esta no es la causa de tus problemas de vibración y lo siguiente es cierto con respecto a tus controles táctiles:

* los controladores táctiles son minúsculos
* no hay vibración al golpear varios bloques
* hay un ligero retraso al tocar los sables entre sí
* estás usando los controladores táctiles de Oculus

Entonces es muy probable que Beat Saber esté sobrecargando el controlador USB de tu placa base. Oculus devora el ancho de banda de tu controlador USB y la mayoría de las placas base vienen con un controlador muy barato. Beat Saber lo fuerza más que cualquier otro juego, esto es por lo que otros juegos y menús pueden estar bien. No hay una solución clara, así que prueba lo siguiente:

* Intercambia los cables USB del HMD y del sensor en diferentes puertos
* Desconecta dispositivos USB innecesarios
* Compra un concentrador USB de tipo PCI-Express
* Utiliza `-vrmode oculus` si utilizas SteamVR para saltártelo y utilizar el SDK de Oculus en su lugar

### Avatares personalizados

#### 3.4 Avatares personalizados que no se muestran en el juego
Haz clic en el botón **Inicio** del teclado con el juego enfocado para alternar la visibilidad en el auricular.

#### 3.5 Mis avatares no funcionan
Asegúrate de que tu mod de avatares personalizados está instalado correctamente y actualizado, también asegúrate de que sus dependencias están también. Puede que tengas un avatar corrupto/roto, tener un avatar roto puede romper todos tus avatares al igual que las canciones y los sables.

### Canciones personalizadas

#### 3.6 Faltan mis canciones
Asegúrate de que tus canciones están en tu carpeta `CustomLevels`, ubicada en `Beat Saber/Beat Saber_Data/`. De aquí es de donde el juego lee de forma nativa las canciones personalizadas.

**No** coloques las canciones en la antigua carpeta `Beat Saber/CustomSongs`. Esta ubicación está obsoleta ya que el formato de las canciones ha cambiado. Si tienes mapas en el formato antiguo (archivos `.json` y `.ogg` en lugar de `.dat` y `.egg`), déjalos en la antigua carpeta `Beat Saber/CustomSongs`. Tendrás que volver a descargarlos desde BeatSaver.

También puede convertirlos manualmente utilizando [Song Converter](https://github.com/lolPants/songe-converter), sin embargo, no obtendrás ninguna ayuda con este método y tendrás que compilar el programa tu mismo.

#### 3.7 Botón Play en gris
Haz clic en el botón azul brillante con el signo de interrogación (?) en la esquina superior derecha. Esto debería decirte qué mods son necesarios para y la canción, cuales te faltan y cuales deberías instalar. Si sigue sin funcionar, prueba a reinstalar el mod necesario. De lo contrario, intenta una [Instalación-limpia](#clean-installation).

#### 3.8 Los detalles del mapa se quedan cargando infinitamente
Si esto sólo ocurre en determinados mapas, es posible que te falten mods necesarios o que esos archivos de canciones estén rotos. Si le pasa a todos tus mapas, borra tu carpeta `Plugins` y vuelve a instalar unos nuevos.

### CameraPlus

#### 3.9 No funciona CameraPlus/Pasada la pantalla de Salud
Asegúrate de que la configuración "Smooth Camera" del juego está desactivada en los ajustes del juego. Si no funciona, prueba a reinstalarlo y sus también dependencias asociadas.

#### 3.10 Mi vista de escritorio sólo ocupa una pequeña parte de la pantalla
El visor de CameraPlus no está llenando tu pantalla. Arrastra la esquina para que se ajuste a la pantalla, o haz clic con el botón derecho del ratón en la ventana y hacer clic en "Ajustar a la pantalla".

### BeatSaver Downloader

#### 3.11 Botón More Songs en BeatSaver Downloader
**El botón More Songs se encuentra en el menú principal a la izquierda bajo el texto de Mods.** Si el botón More Songs está está en gris, asegúrate de que todas tus canciones se han cargado primero, como se ve en la barra de progreso arcoiris en el menú principal. Si tu menú de Mods no aparece ahí, entonces asegúrate de que tus mods y dependencias funcionan y están instalados correctamente, consulta la sección [¿No hay mods?](#_1-no-mods).

#### 3.12 No aparece nada en el menú More Songs
Las causas probables de que BeatSaver Downloader no funcione son:

1. Asegúrate de que todas tus canciones se han cargado antes, o de lo contrario el botón de More Songs aparecerá en gris.
2. Tu antivirus o cortafuegos está bloqueando el acceso a BeatSaver.
3. Has alcanzado el límite de intentos de Beatsaver y tendrás que esperar antes de volver a intentarlo.

### Códigos de error multijugador
A continuación, una lista de los códigos de error conocidos, lo que significan y lo que puedes hacer para solucionarlos.

<!-- Disable line length rule because of table -->
<!-- markdownlint-disable MD013 -->
| Código&nbsp; | Descripción                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
|:------------ |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| CFR-1        | Se ha producido un error desconocido. Intenta reiniciar el juego.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| CFR-2        | La conexión multijugador fue cancelada.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| CFR-3        | No se puede acceder al servidor. Puede haber un problema con tu conexión a Internet o con los servidores de retransmisión de Beat Saber. Comprueba que no estás sin red y que tu cortafuegos permite a Beat Saber conectarse a Internet. <details><summary>**Antecedentes**</summary>El multijugador de Beat Saber es peer-to-peer donde te conectas directamente con cada jugador en la sala. Cuando esto no es posible, Beat Saber inicia un servidor "relevo" para enviar los datos. Este error significa que ambos métodos han fallado.</details> &nbsp; Esto también puede ser causado por el uso de emojis o caracteres especiales en tu nombre de usuario. |
| CFR-4        | El servidor ya existe.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| CFR-5        | El servidor no existe. Es posible que la sala a la que te estabas conectando se haya cerrado cuando te estabas uniendo.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| CFR-6        | El servidor está lleno. Elige otra sala.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| CFR-7        | Estás en una versión del juego no soportada por los servidores.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| CFR-8        | La contraseña de la sala es incorrecta. Comprueba que estás introduciendo la contraseña correcta.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| CFR-9        | Los servidores de matchmaking que gestiona Beat Games, que llevan el control de las salas públicas y privadas abiertas, están desconectados. Prueba de nuevo más tarde.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| CFR-10       | Tu clave de sesión de Steam u Oculus no es válida. Si juegas en Quest y has modificado tu juego, consulta esta [respuesta del FAQ](/faq/README.md#does-multiplayer-have-crossplay) para solucionar esto. De lo contrario, estás usando una copia pirata del juego la cual no es compatible.                                                                                                                                                                                                                                                                                                                                                             |
| CFR-11       | Tu conexión a internet está desconectada.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
<!-- markdownlint-enable MD013 -->

## 4. Solución de problemas varios

### Comprender los registros
Si estás en Steam puedes ir a
> Beat Saber > Properties > General > Add `--verbose` al campo de opciones de inicio

Si estás en Oculus, tendrás que hacer clic con el botón derecho en Beat Saber.exe y crear un acceso directo. Edita el destino añadiendo "--verbose" al final de este. Por ejemplo, `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber.exe" --verbose`

Después de añadir verbose a tu juego debería mostrarse cualquier error relacionado con tus avatares, sables y canciones

* Esto puede no mostrarse el 100% de las veces para los avatares y sables, y puede que tengas que quitar todos tus avatares/sables y probar uno por uno para ver cual rompe el juego.

Estos mensajes también se registran en `Beat Saber/Logs`.

Puedes encontrar una lista de excepciones comunes [aquí](./exceptions.md).

### Verifica los archivos del juego en Steam
Para verificar la integridad de los archivos del juego sigue estos pasos:

1. Asegúrate de que SteamVR está cerrado ya que de lo contrario no te dejará verificar tus juegos.
2. Ve a tu librería de Steam y encuentra Beat Saber
3. Haz clic derecho en Beat Saber y haz clic en Propiedades
4. Ve a la pestaña "Archivos locales" en las propiedades
5. Selecciona la opción "Verificar la integridad de los archivos del juego".
6. Deja que termine de verificar y descargar los archivos que faltan y ya debería estar listo.

Aquí hay una [guía en vídeo](https://www.youtube.com/watch?v=EBFfT4-ZiIc) aunque está en la antigua interfaz de usuario de Steam, los pasos siguen siendo los mismos.

### Instalación limpia

1. (Opcional) Haz una copia de seguridad de los contenidos personalizados descargados haciendo una copia de las siguientes carpetas:

* `Beat Saber\Beat Saber_Data\CustomLevels`
* `Beat Saber\CustomSabers`
* `Beat Saber\CustomPlatforms`
* `Beat Saber\CustomNotes`
* `Beat Saber\CustomAvatars`

2. **Borra TODA la carpeta de Beat Saber.** Esto es diferente a desinstalar el juego en Steam, ya que hacer esto no eliminará los archivos que no venían con el juego.

> Steam: ``\steamapps\common\Beat Saber\`
  Oculus:``\hyperbolic-magnetism-beat-saber\`

3. Reinstala el juego a través de Steam o la tienda Oculus
4. **Antes de realizar las modificaciones, lanza el juego una vez**
5. Ejecuta Mod Assistant, instala tus mods, e inicia el juego.

(Opcional) Si quieres ir un paso más allá, consulta: [Borrar la carpeta de Beatsaber dentro de AppData](#deleting-your-save-in-appdata)

### Borrar tus datos guardados en AppData
Esto borrará tus puntuaciones y datos locales, pero no tus estadísticas de tu tabla de clasificación personalizada/ScoreSaber. Puedes encontrar la carpeta en
> `%appdata%/../locallow/hyperbolic magnetism/beat saber`

Copia y pega todo lo que hay dentro de la barra de arriba y pégalo en tu barra de direcciones en el explorador de archivos y bórralo.

También puedes llegar a esta carpeta mostrando los elementos ocultos y navegando a tu
> Users > "USER" > AppData > LocalLow > Hyperbolic Magnetism > beat saber

<YouTube url='https://youtu.be/ONxJcD3Ir3Q' />

::: warning Al eliminar esta carpeta en Appdata también se eliminarán las puntuaciones locales y las estadísticas. :::

#### Medidas desesperadas
::: warning Desactivar tu antivirus implica riesgos de seguridad, asegúrate de saber lo que estás haciendo (es decir, no descargues ni abras archivos sospechosos mientras esté desactivado) y no olvides volver a activarlo en cuanto termines estos pasos. :::

* Asegúrate de que tu usuario actual **es un administrador**
* **Apaga** tu antivirus (durante el proceso al menos)
* Asegúrate de que tienes permiso para crear carpetas y editar archivos dentro de la unidad de disco/tu PC, (por lo que he oído una actualización de windows recientemente causó problemas a la gente)
* Asegúrate de que tus controladores están actualizados
* Comprueba que el problema no se encuentra en los auriculares, ni en el sistema operativo, ni en el hardware/software
* Comprueba tu conexión a internet, y que no haya nada que bloquee lo relacionado con el modding de BeatSaber y Steam, etc.

## 5. ¿Aún tienes problemas?
¡Si esta página no cubre lo básico, no dudes en hacer una pregunta en el discord! Para aumentar las posibilidades de que tus preguntas sean respondidas, ten en cuenta lo siguiente:

* Utiliza los canales correctos por favor, `#pc-help` para soporte de mods en PC y `#quest-help` para soporte de mods en Quest. Utiliza `#pc-3d-modeling` y `#quest-3d-modeling` para preguntas sobre **hacer tus propios avatares, plataformas, notas o sables**, y `#mapping-discussion` para preguntas sobre **hacer mapas.**
* Sé educado y respetuoso
* Describe tu problema en detalle. "No funcionó" es tan descriptivo como decirle a tu médico que no te sientes bien. ¿Qué es lo que no funciona y qué has probado? ¿Hay algún mensaje que aparezca en la pantalla? ¿Toda tu pantalla se ha vuelto de color púrpura brillante?

::: tip NOTA Aquellos con el rol de `Soporte` son voluntarios que pueden elegir ayudar en su tiempo libre. El rol de soporte es un reconocimiento a los conocimientos y al esfuerzo que han realizado, pero eso no significa necesariamente que estarán cerca para ayudar sólo porque están en línea. :::

Reconocimientos a Saber-Chan por su arduo trabajo en esta página.
