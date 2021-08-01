---
sidebar: auto
---

# Mods en Quest

## Prólogo

* Esta guía es tanto para las Quest 1 como para las Quest 2.
* Todavía no se ha baneado a nadie por moddear.

::: danger Descargo de responsabilidad Al elegir usar mods, entiendes que:

* Puede que experimentes problemas que no existen en el juego base. El 99,9% de los errores, fallos y lag se deben a mods.
* Los Mods están sujetos a romperse por actualizaciones y eso es normal - sed pacientes y respetuosos cuando esto suceda, ya que los modders son voluntarios con vidas reales.
* Beat Games no trata de romper los mods a proposito. Quieren trabajar en la base de código y a veces esto rompe los mods, pero no están decididos a matar los mods.

No atacar a los desarrolladores por problemas relacionados con mods, y viceversa - los modders y los desarrolladores son dos grupos separados. Simplemente no seas un cretino ok? :::

:::warning He visto un video tutorial en YouTube, pero me he quedado atascado/no ha funcionado. ¿Qué sucede? Aquí en BSMG recomendamos **encarecidamente** que no se utilicen tutoriales en vídeo para el modding. A menudo, nos encontramos con que están desfasados o contienen una información incompleta, errónea o directamente incorrecta.

En su lugar, debes seguir las guías escritas aquí en la wiki o buscar ayuda en el [Discord de BSMG ](https://discord.gg/beatsabermods). :::

## Instalación
Actualmente la única forma recomendada para instalar canciones personalizadas y mods es BMBF cargándolo con SideQuest usando un PC.

Si no tienes acceso a un PC puedes utilizar un [teléfono Android](#installing-bmbf-with-an-android-phone).

* [BMBF apk](https://bmbf.dev/stable) :::warning Instalar BMBF y modear tu juego deshabilitará el Multijugador Oficial, así como ver y subir puntuaciones en los marcadores del juego base. Si quieres jugar multijugador con mods, necesitas el mod, `Beat Together`, que permite el juego cruzado entre pc y Quest y permite que se usen canciones personalizadas si todas las partes tienen dicha canción. El mod se puede encontrar en el Beat Saber Modding Group en `#quest-mods` o en el sitio [Questboard](https://questmodding.com).

Para tener tablas de clasificación en las canciones personalizadas y poder obtener Puntos de Actuación (PA) de las canciones clasificatorias necesitas el mod [ScoreSaber](https://new.scoresaber.com/quest). [Este enlace](https://new.scoresaber.com/quest) te llevará a la página de ScoreSaber para configurarlo. ScoreSaber no sustituye las tablas de clasificación del juego base, sólo añade tablas de clasificación para las canciones personalizadas.

**Nota:** Comprueba el canal de actualizaciones en el [discord de ScoreSaber](https://discord.gg/WpuDMwU) para ver si el mod está disponible para la actual versión del juego. :::

### Instalar BMBF con SideQuest
Si aún no lo has hecho, descarga e instala [SideQuest](https://sidequestvr.com/#/setup-howto)

Abre SideQuest y conecta tu Quest a tu PC.

:::tip Si has modificado Beat Saber previamente o tienes puntuaciones que quieres conservar, [¡Haz primero una copia de seguridad de tus datos guardados!](#backup-save-data-using-sidequest). :::

Si tienes un juego modificado también tienes que desinstalarlo pulsando el botón `UNINSTALL APP`. Más tarde, puedes restaurar tus datos guardados desde el mismo menú, después de la modificación.

Selecciona el botón `Install APK from folder` que se muestra a continuación y busca el último apk de BMBF que has descargado y haz clic en él, o simplemente arrastra el apk de BMBF a SideQuest. Cualquiera de los dos métodos instalará BMBF en tu dispositivo Quest.

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

Una vez que se haya instalado con éxito, asegúrate de que tienes la última versión de Beat Saber instalada y sin modificar.

:::warning Antes de hacer las modificaciones, ejecuta Beat Saber una vez, juega un nivel y ¡fracasa inmediatamente!

Actualmente, la modificación no funciona si se utiliza la función experimental de multiusuario. Tendrás que eliminar temporalmente todas las cuentas secundarias antes de modificar el juego. Podrás volver a añadirlas más tarde cuando hayas instalado los mods que desees. :::

Después de ejecutar Beat Saber una vez, abre BMBF desde fuentes desconocidas como muestra la imagen de abajo. ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

Una vez abierto, sigue cada paso en BMBF exactamente como se te indica para modificar tu juego. Una vez completado, deberías ver[Bsaber.com](https://www.bsaber.com) dentro de la aplicación BMBF. Aquí es donde puedes descargar cualquier canción personalizada disponible. También puedes hacer clic en el icono del globo terráqueo de la parte superior derecha e ir también a BeatSaver para descargar canciones.

Si en algún momento del proceso de instalación aparece la ventana emergente `Restore App`, simplemente haz clic en `Close`. Esta advertencia se dirige más bien a las versiones piratas del juego, por lo que si sólo estás haciendo modding probablemente no habrá consecuencias por ignorarla.

![RestoreApp](~@images/beginners-guide/restoreapp.png)

Continúa con el paso [Mods esenciales](#core-mods) del proceso de instalación.

### Instalando BMBF con un teléfono Android
Esta **NO** es la forma recomendada de instalar BMBF y sólo debe utilizarse si no se tiene acceso a un PC.

* [Requisitos](#requirements)
* [Configura tu teléfono](#setup-your-phone)
* [Instalando BMBF con tu teléfono](#installing-bmbf-with-your-phone)
* [Configurar Beat Saber](#setup-beat-saber)

#### Requisitos

* Un teléfono Android o una tableta Android (iPhones ni iPads están soportados)
* Una versión **pagada** de Beat Saber en la Tienda de Oculus Quest
* Un cable para conectar tus Quest a tu teléfono (Si tu teléfono carga por USB C el cargador que se incluyó en tus Quest debería funcionar)

#### Configura tu teléfono

1. Descarga la aplicación [Bugjaeger en la tienda Google Play](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)
2. Descarga el APK más reciente de [ BMBF desde bmbf.dev/stable](https://bmbf.dev/stable)
3. Sigue [esta guía escrita](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ) para activar el modo de desarrollador en tus Quest.
4. Activar el modo de desarrollador en tu teléfono
    1. Ir a la configuración de Android
    2. Desplázate hasta "Acerca del teléfono" y ábrelo
    3. Pulsa "Información del software"
    4. Toca el campo "Número de construcción" hasta que diga el modo de desarrollador habilitado. Esto debería tomar unos 7 toques.
5. Habilita la depuración USB en tu teléfono
    1. Volver a la configuración
    2. Pulsa "Opciones de desarrollador"
    3. Activar depuración USB

#### Instalando BMBF con tu teléfono
:::warning Antes de modificar, ejecuta Beat Saber una vez, juega un nivel y ¡falla inmediatamente! :::

Abre Bugjaeger en tu teléfono y conecta tu Quest. Debería aparecer una ventana emergente de depuración USB en tu Quest y en tu teléfono. Selecciona permitir en ambos dispositivos y si lo prefieres selecciona permitir siempre. Una vez que Bugjaeger seleccione tu Quest, instala el APK de BMBF haciendo lo siguiente:

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

Después de pulsar ok, permite el acceso al archivo y selecciona el archivo APK a descargar que debe estar etiquetado como `com.weloveoculus.BMBF.apk`. El archivo apk debería instalarse ahora en tu Quest.

#### Configurar Beat Saber
Después de instalar con éxito BMBF en tu Quest, deberías poder encontrarlo en tu biblioteca de Quests bajo fuentes desconocidas.

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

Ábrelo y permite el acceso a los archivos después de iniciarlo si te lo pide. Ahora sigue cuidadosamente las instrucciones en pantalla. Después de terminar deberías ver [BeastSaber](https://bsaber.com).

Si en algún momento del proceso de instalación aparece la ventana emergente `Restore App`, simplemente haz clic en `Close`. Esta advertencia está dirigida a las versiones piratas del juego, por lo que probablemente no habrá consecuencias por ignorarla si tienes una copia legítima.

Ahora puedes continuar con el paso [Core Mods](#core-mods) del proceso de instalación.

## Administrar datos guardados

### Copia de seguridad de datos de guardado usando SideQuest

Abre SideQuest y conecta tu Quest a tu PC. Ve a `My Apps` situado en la barra superior de la ventana y busca Beat Saber.

Navega hasta `sdcard/Android/data/com.beatgames.beatsaber/files` utilizando el explorador de archivos de SideQuest.

Guarda los archivos: `AvatarData.dat`, `PlayerData.dat` y `settings.cfg` en una carpeta de tu PC. ¡No los pierdas, ya que contienen contienen tus puntuaciones y otros ajustes!

### Restaurar datos guardados usando SideQuest

Para restaurar tus datos, abre SideQuest y conecta tu Quest a tu PC. Ve a `My Apps` situado en la barra superior de la ventana y busca Beat Saber. Usando el explorador de archivos de SideQuest toma los 3 archivos que guardaste en los pasos para [realizar copias de seguridad de datos de guardado usando SideQuest](#backup-save-data-using-sidequest) `AvatarData.dat`, `PlayerData.dat` y `settings.cfg` y ponlos en el directorio `sdcard/Android/data/com.beatgames.beatsaber/files`.

Vuelve al menú y pulsa las flechas circulares situadas junto a tu última copia de seguridad. Tus puntuaciones y ajustes deberían estar restaurados.

## Instalar mods

### Mods esenciales
Antes de instalar cualquier mod adicional mira en la parte superior derecha de la interfaz web de BMBF, deberías ver un botón rojo que dice, `Sync to Beat Saber`. Púlsalo y deja que termine de sincronizarse. A continuación, ve a tu pestaña `mods` en BMBF. Asegúrate de que tienes los 5 mods principales:

* Codegen
* Goodbye Bug
* PinkCore
* QuestUI
* Custom Types

:::danger Todos los demás mods no funcionarán si estos mods principales no están listados y activados.

Si uno de los mods principales no se activa, borra ese mod y haz clic en `Sync to Beat Saber` de nuevo para volver a descargarlo. Comprueba de nuevo si se ha descargado y activado. Si sigue sin funcionar, o los mods parecen estar activados, pero no funcionan en el juego mira [Core Mods don't work](#core-mods-don-t-work) para ver los pasos para solucionar los problemas. :::

### Dentro de tus Quest
:::warning No todos los mods están disponibles en QuestBoard  
Si no ves un mod ahí, debes seguir el método [Usando tu PC](#using-your-pc) en su lugar. :::

Abre BMBF en tu Quest y ve a la pestaña `Browser`, allí deberías ver un icono de un globo terráqueo similar al que se muestra a continuación. Ha< clic en él y, a continuación, en el botón `QuestBoard`.

![globequestboard](~@images/beginners-guide/globequestboard.png)

Debería aparecer el sitio web [QuestBoard](https://www.questmodding.com/) debajo. A continuación, selecciona la pestaña `DOWNLOAD MODS`.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Desplázate hacia abajo con los sticks. Ahora puedes seleccionar cualquier mod de la lista, que se ve a continuación, y descargarlo pulsando el botón botón de descarga junto a él. Algunas descargas pueden redirigirte a un sitio web o a una página de GitHub. Si es así, sigue las instrucciones en pantalla, o selecciona el último `.zip` en la lista de versiones, respectivamente.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Usando tu PC
Puedes encontrar y descargar otros mods para Quest desde el [Discord de BSMG](https://discord.com/invite/beatsabermods) en el canal `#quest-mods`.

:::warning ¡Asegúrate de que tu Quest y tu PC están en la misma red y que estás utilizando http y no https! :::

Abre BMBF en tu Quest y ve a la pestaña `Tools`, allí deberías ver una dirección web y un número de versión similar al que se muestra a continuación.

![ip](~@images/beginners-guide/ip.png)

En tu PC, abre tu navegador y escribe la dirección en la barra de búsqueda.

Debería aparecer la siguiente pantalla debajo.

Si esto no funciona [haz clic aquí](#bmbf-web-interface-not-loading) para ver algunos pasos para la resolución de problemas.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Ahora sólo tienes que arrastrar cualquier mod compatible con Quest a la caja de subida de archivos y sincronizar. Si el mod fue originalmente creado para una versión anterior, entonces no se activará automáticamente. Para activar un mod antiguo, ve a la pestaña `Mods` y habilítalo desde allí.

## Instalar canciones
::: tip La mayoría de los mapas en los filtros de ordenación "Top All", "Rating", "Downloads" o "Plays" fueron creados antes de que se establecieran las buenas prácticas de mapeo. Prueba a descargar las canciones publicadas entre finales de 2019 y el día de hoy para obtener la mejor experiencia en niveles personalizados. :::

### Dentro de tus Quest
Hay dos fuentes para obtener mapas personalizados dentro de tu Quest utilizando la ventana del navegador.

* Si estás buscando mapas y listas de reproducción supervisadas, visita [BeastSaber](https://bsaber.com/)
* Si no te gusta la interfaz de usuario de BeastSaber también puedes probar [BeatSaver](https://beatsaver.com/)

Ambos tienen un botón de un sólo clic que instala fácilmente esa canción en tu Quest. Puedes pasar de un sitio web a otro utilizando el icono del globo terráqueo situado en la parte superior derecha de la ventana del navegador.

Una forma fácil de descargar diferentes tipos de canciones es utilizar `Syncsaber` al que puedes acceder entrando en BMBF en tu Quest y haciendo clic en la pestaña llamada `Syncsaber`. Aquí puedes descargar canciones con el clic de un botón, puedes elegir entre diferentes "ajustes". Por ejemplo, puedes descargar las 20 mejores canciones de la sección "hot" de [BeatSaver](https://beatsaver.com/) o las 50 canciones mejor clasificadas.

Otro método es el uso de la función `Bookmark` en [BeastSaber](https://bsaber.com/). Después de crear una cuenta, puedes hacer clic en un pequeño icono de marcador en una canción y si más tarde borras todas tus canciones del Quest puedes volver a descargar las que están marcadas con OneClick™.

### Usando tu PC
Si no puedes instalar canciones dentro de tu Quest, puedes instalar mapas usando tu ordenador de forma similar a la instalación de mods.

1. Visita [BeastSaber](https://bsaber.com/) o [BeatSaver](https://beatsaver.com/) en tu ordenador
2. Descarga el zip
3. Sigue los pasos de [Instalación de mods usando tu PC](#using-your-pc) hasta la pantalla de subir archivos.
4. ¡Arrastra y suelta dentro el zip del mapa y debería ser instalado!

Si la interfaz web no se carga [haz clic aquí](#bmbf-web-interface-not-loading) para ver algunos pasos para la resolución de problemas.

:::tip También puedes descargar listas de reproducción de la misma manera. Puedes encontrar varias listas de reproducción en [BeastSaber](https://bsaber.com/category/playlists/) o en varios discords de la comunidad. También puedes crear la tuya propia utilizando [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) o [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

¡Si quieres probar un mapa que has creado, consulta la sección [Testeo en Quest](/mapping/#testing-on-a-quest) en la Wiki de mapeo para conocer los pasos para empaquetarlo y probarlo! :::

## Instalando modelos
¡Únete a la [Comunidad Qosmetics](https://discord.gg/qosmetics) para cambiar el aspecto del título de tu menú, los sables, los bloques o los muros en el juego!

## Enlaces útiles

* [Comunidad Qosmetics](https://discord.gg/qosmetics) - Servidor dedicado a hacer y usar sables, bloques y paredes para Quest.
* [Guías de creación de Qosmetics](https://github.com/RedBrumbler/Qosmetics/wiki) - Guías para crear tus propios sables, bloques y muros personalizados para las Quest.
* [Sitio web de QuestBoard](https://questmodding.com) - Un lugar para obtener noticias e información relacionada con Beat Saber junto con los últimos lanzamientos de los mods.
* [Servidor de Discord de QuestBoard](https://discord.gg/P7sUKVnP) - Una comunidad de Quest para pasar el rato y hablar de cosas relacionadas con Beat Saber, también puedes obtener un rol para ser notificado cuando un nuevo mod sea publicado.
* [Arreglando audio desincronizado](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - Tablas de clasificación para canciones personalizadas

## Resolución de problemas
:::warning He visto un video tutorial en YouTube, pero me he quedado atascado/no ha funcionado. ¿Qué sucede? Aquí en BSMG desaconsejamos **encarecidamente** el uso de cualquier video tutorial para realizar el modding. A menudo, nos encontramos con que están anticuados o contienen información incompleta, errónea o directamente incorrecta.

En su lugar, debes seguir las guías escritas aquí en la wiki o buscar ayuda en el [Discord de BSMG](https://discord.gg/beatsabermods). :::

### Añadir mods de beatmods.com o modelos de modelsaber.com no funciona
La razón por la que añadir mods de [BeatMods](https://beatmods.com/) o modelos de [ModelSaber](https://modelsaber.com/) no funciona es porque esos mods y modelos son sólo para PC.

Consigue mods compatibles con Quest en [QuestBoard](https://www.questmodding.com/) o `#quest-mods` en el discord de Beat Saber Modding Group, con sables, bloques y muros compatibles con las Quest en la [comunidad Qosmetics](https://discord.gg/qosmetics). Una vez que tengas tu mod o modelo zip utiliza la [interfaz web de BMBF](#using-your-pc) para instalarlo.

### Error al hacer Sideloading con BMBF
Al cargar BMBF se obtiene el error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: El paquete com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

Deberás desinstalar la versión de BMBF en tu Quest. Puedes hacer esto desde el menú `My Apps` de SideQuest.

### Los mods esenciales no funcionan

Si tienes problemas con los mods esenciales, comprueba que no estás intentando utilizar ningún mod obsoleto. Cualquier mod hecho para una versión anterior del juego se considera obsoleto. Una vez que los hayas eliminado:

1. Ve a `Herramientas`
2. Haz clic en `salir de BMBF`
3. Abre de nuevo BMBF
4. Ve a `Herramientas` de nuevo
5. Haz clic en `reparación rápida`
6. Ve a la sección `Navegador` de la aplicación BMBF.
7. Haz clic en el icono de globo pequeño en la esquina superior derecha
8. Haz clic en `QuestBoard`
9. Haga clic en `descargar Mods`
10. Desplázate hacia abajo y haz clic en `Descargar todos los Mods esenciales`
11. Haz clic en `Sincronizar con Beat Saber`

---

### Interfaz web de BMBF no cargada
Si tu Interfaz Web de BMBF no se carga, asegúrate de que estás escribiendo la IP desde la pestaña de herramientas en tu ordenador que está en la misma red. Asegúrate de:

1. 1) Tu IP no es `127.0.0.1`, si eso aparece prueba a reiniciar tu visor y/o router.
2. BMBF está abierto en los auriculares
3. Hay `http://` al principio del enlace, no `https://`
4. Tienes `:50000` al final de tu enlace
5. Tu PC y Quest están en la misma red wifi
6. Tu IP no ha cambiado ya que cambia de vez en cuando

Si nada de esto funciona, reinicia tu Quest y repasa la lista de nuevo.

---

### BMBF no carga la configuración después de unos minutos
Es probable que esto se deba a la utilización de BMBF en una versión del juego para la que no fue creado. Como por ejemplo usar BMBF para la versión de Beat Saber `1.13.0` cuando la versión del juego instalada en los cascos es `1.12.2`.  
Si la versión del juego coincide con la que dice la página de lanzamientos de BMBF, intenta reiniciar tus cascos. Si todavía no no funciona, utiliza la [Interfaz Web de BMBF](#using-your-pc) y haz clic en `Quick Fix` en la pestaña Tools.

### Beat Saber esta en negro cuando lo lanzo
Abre la biblioteca en tu Quest. Haz clic en los tres puntos junto a Beat Saber y luego haz clic en `Permissions`. En el menú que aparece, activa los permisos de almacenamiento e intenta lanzar el juego de nuevo.

---

### ¡Mis Sables y Mods no se activan/funcionan!
Lo más probable es que esto se deba a que tienes una aplicación BMBF anticuada, obtén la última [versión de BMBF](https://bmbf.dev/stable). Si la versión de BMBF para tu Beat Saber no está ahí, por favor espera un tiempo para que los unicornios actualicen BMBF.

* Si se supone que tu mod es compatible con tu versión de BMBF, asegúrese de que no hay ninguna carpeta que separa el contenido del archivo .zip.
* Si tu nivel no se carga entonces intenta instalar extensiones de mapeo desde #quest-mods. También puede requerir las extensiones de mod Noodle que aún no están en las Quest.
* Si tu BMBF está en la última versión y los mods no están habilitados en el juego, desinstala Beat Saber con el botón de desinstalar BS en la pestaña BMBF Tools y despues reinstalar y remodear.
* En casos muy muy muy raros, BMBF no tiene permisos de archivo para copiar mods en la ubicación correcta. Compruebe en SideQuest para asegurarse de que BMBF tiene permisos de archivo.

---

### Beat Saber esta crasheando
Si tu juego se bloquea al hacer algo, desactiva tus mods uno por uno, ejecutando tu juego cada vez para ver si el problema se soluciona antes de pedir ayuda en un canal de soporte.

### Sólo veo una pantalla blanca cuando abro BMBF
Si sólo ves una pantalla blanca cuando abres BMBF desde fuentes desconocidas, reinicia tu Quest y entonces debería solucionarse

### ¡Mi Beat Saber tiene 3 puntos cuando lo inicio!
Si tu Beat Saber muestra 3 puntos al lanzarlo asegúrate de que:

1. Has lanzado y jugado una canción antes de modificar el juego
2. No estás usando una versión pirata del juego
3. Asegúrate de estar usando la última versión de BMBF
