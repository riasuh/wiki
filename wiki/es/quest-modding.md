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

## Instalación
Actualmente la única forma recomendada de instalar canciones y mods personalizados es BMBF sideloaded con SideQuest usando un PC.

Si no tienes acceso a un PC puedes utilizar un [teléfono Android](#installing-bmbf-with-an-android-phone).

* [BMBF apk](https://bmbf.dev/stable) :::warning Instalar BMBF y modear tu juego deshabilitará el Multijugador Oficial, así como ver y subir puntuaciones en los marcadores del juego base. Si quieres jugar multijugador con mods, necesitas el mod, `Beat Together`, que permite el juego cruzado entre pc y Quest y permite que se usen canciones personalizadas si todas las partes tienen dicha canción. El mod se puede encontrar en el Beat Saber Modding Group en `#quest-mods` o en el sitio [Questboard](https://questmodding.com).

Para obtener tablas de clasificación en canciones personalizadas y para poder obtener puntos de rendimiento (PP) de canciones clasificadas, necesitas el mod [ScoreSaber](https://new.scoresaber.com/quest). [Este enlace](https://new.scoresaber.com/quest) te lleva a la página ScoreSaber para configurarlo. Scoresaber no reemplaza las tablas de clasificación del juego base, sólo añade tablas de clasificación para canciones personalizadas. **Nota:** Scoresaber aún no ha sido actualizado para Beat saber 1.13.2. :::

### Instalar BMBF con SideQuest
Si aún no lo has hecho, descarga y configura [SideQuest](https://sidequestvr.com/#/setup-howto)

Abre SideQuest y conecta tus Quest a tu PC.

:::tip Si has modificado anteriormente Beat Saber o tienes puntuaciones que quieres respaldar, [¡Copia tus datos guardados primero!](#backup-save-data-using-sidequest) :::

Si tienes un juego modeado también necesitas desinstalarlo pulsando el botón `DESINSTALAR APLICACIÓN`. Más adelante puedes restaurar tus datos guardados desde el mismo menú, después de la modificación.

Selecciona el botón `Instalar APK de la carpeta` que se muestra a continuación y encuentra la última apk BMBF que descargaste y haz clic en ella o simplemente arrastra el apk BMBF a SideQuest. Cualquiera de los dos métodos instalará BMBF en tus Quest.

![Installar Apk](~@images/beginners-guide/apkfromfolder.png)

Una vez que se haya instalado con éxito, asegúrate de que tienes la última versión de Beat Saber instalada y sin modificar.

:::warning Antes de modificar, ejecuta Beat Saber una vez, juega un nivel y ¡falla inmediatamente! :::

Después de ejecutar Beat Saber una vez, abre BMBF de fuentes desconocidas como muestra la imagen de abajo. ![Fuente desconocida](~@images/beginners-guide/quest_home-menu.jpg)

Sigue cada paso exactamente como se ha dicho. Entonces, deberías ver [bsaber.com](https://www.bsaber.com). Aquí es donde puedes descargar cualquier canción personalizada disponible. También puedes hacer clic en el icono del globo en la parte superior derecha e ir a beatsaver para descargar canciones.

Si en algún momento durante el proceso de instalación, obtienes la ventana emergente `Restaurar aplicación` solo haz clic en `Cerrar`. Esta advertencia está más dirigida a las versiones pirateadas del juego, así que si solo estás modeandolo probablemente no habrá consecuencias por ignorarlo.

![Restaurar App](~@images/beginners-guide/restoreapp.png)

Continúa al paso [Mods esenciales](#core-mods) del proceso de instalación.

### Instalando BMBF con un teléfono Android
Esta **NO** es la forma recomendada de instalar BMBF y solo debe ser usada si no tienes acceso a un PC.

* [Requisitos](#requirements)
* [Configura tu teléfono](#setup-your-phone)
* [Instalando BMBF con tu teléfono](#installing-bmbf-with-your-phone)
* [Configurar Beat Saber](#setup-beat-saber)

#### Requisitos

* Un teléfono Android o Tablet Android (no se admiten teléfonos IPhones o IPAds)
* Una versión **pagada** de Beat Saber en la Tienda de Oculus Quest
* Un cable para conectar tus Quest a tu teléfono (Si tu teléfono carga por USB C el cargador que se incluyó en tus Quest debería funcionar)

#### Configura tu teléfono

1. Descarga la aplicación [bugjaeger desde la tienda Google Play](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)
2. Descarga el más reciente [APK BMBF desde bmbf.dev/stable](https://bmbf.dev/stable)
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

Abre bugjaeger en tu teléfono y conecta tus Quest. Deberías tener un emergente de depuración USB en tus Quest y en tu teléfono. Selecciona permitir en ambos dispositivos y si lo prefieres, seleccione siempre permitir. Una vez que el bugjaeger escoja tus Quest, instala el APK de BMBF haciendo lo siguiente:

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

Después de haber presionado ok, permitir el acceso al archivo y seleccionar el archivo APK de descarga, el cual debe ser etiquetado `com.weloveoculus.BMBF.apk`. El archivo apk ahora debe instalarse en tus Quest.

#### Configurar Beat Saber
Después de instalar con éxito BMBF en tus Quest, deberías poder encontrarlo en tu biblioteca de Quest bajo fuentes desconocidas.

![Menú desconocido](~@images/beginners-guide/quest_home-menu.jpg)

Ábrelo y permite el acceso de archivos después de iniciarlo si se te solicita. Ahora sigue las instrucciones en pantalla con cuidado. Después de que hayas terminado, deberías ver [BeastSaber](https://bsaber.com).

Si en algún momento durante el proceso de instalación, obtienes la ventana emergente Restaurar aplicación solo haz clic en Cerrar. Esta advertencia está dirigida a versiones pirateadas del juego, por lo que probablemente no habrá consecuencias para ignorarla si tienes una copia legítima.

Ahora puedes continuar con el paso [Mods esenciales](#core-mods) del proceso de instalación.

## Administrar datos guardados

### Copia de seguridad de datos usando SideQuest

Abre SideQuest y conecta tus Quest a tu PC. Ve a `Mis aplicaciones` ubicadas en la barra superior de la ventana y encuentra Beat Saber.

Ve a `sdcard/Android/data/com.beatgames.beatsaber/files` usando el explorador de archivos de SideQuest.

Guarda los archivos: `AvatarData.dat`, `PlayerData.dat` y `settings.cfg` en una carpeta en tu PC. ¡No los pierda, ya que contienen tus puntuaciones y otros ajustes!

### Restaurar datos guardados usando SideQuest

Para restaurar tus datos, abre SideQuest y conecta tus Quest a tu PC. Ve a `Mis aplicaciones` ubicadas en la barra superior de la ventana y encuentra Beat Saber. Usando el explorador de archivos de SideQuest toma los 3 archivos que has guardado en los pasos de [Copia de seguridad de datos usando SideQuest](#backup-save-data-using-sidequest) `AvatarData.dat`, `PlayerData.dat` y`settings.cfg` y ponlos en la carpeta `sdcard/Android/data/com.beatgames.beatsaber/files`.

Vuelve al menú y pulsa las flechas circulares ubicadas al lado de tu última copia de seguridad. Tus puntuaciones y ajustes ahora deben ser restaurados.

## Instalar mods

### Mods esenciales
Antes de instalar cualquier mods adicional mira en la parte superior derecha de la interfaz web BMBF, deberías ver un botón rojo que dice, `Sincronizar con Beat Saber`. Haz clic en esto y deja que termine de sincronizar. Luego ve a tu pestaña de `mods` en BMBF. Asegúrate de que tienes los 5 mods esenciales:

* Codegen
* Goodbye bug
* PinkCore
* QuestUI
* Custom Types

:::danger Todos los demás mods no funcionarán si estos mods esenciales no están listados y habilitados.

Si uno de los mods esenciales no se habilita, elimina ese mod y haz clic en `Sincronizar con beat Saber` de nuevo para volver a descargarlo. Asegúrate de que se ha descargado y habilitado. Si todavía no funciona, o los mods parecen estar habilitados, pero sin funcionar en el juego mira [los Mods esenciales no funcionan](#core-mods-don-t-work) para los pasos de solución de problemas. :::

### Dentro de tus Quest
:::warning ¡No todos los mods están disponibles en QuestBoard!  
Si un mod no se ve aquí, deberías seguir el método [usando tu PC](#using-your-pc) en su lugar. :::

Abre BMBF en tus Quest y ve a la pestaña `Navegador`, ahí deberías ver un icono de globo similar a lo que se muestra a continuación. Haz clic en él, luego haz clic en el botón `QuestBoard`.

![globequestboard](~@images/beginners-guide/globequestboard.png)

Deberías ser saludado con el sitio web de [QuestBoard](https://www.questmodding.com/)debajo. A continuación, selecciona la pestaña `DOWNLOAD MODS `.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Desplázate hacia abajo con los sticks. Ahora puedes seleccionar cualquier mod de la lista, vistos a continuación, y descargarlo pulsando el botón de descarga junto a él. Algunas descargas pueden redirigirte a un sitio web o a una página de GitHub. Si es así, sigue las instrucciones en pantalla o selecciona el ultimo `.zip` en la lista de Versiones, respectivamente.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Usando tu PC
Puedes encontrar y descargar otros mods de Quest desde el [BSMG Discord](https://discord.com/invite/beatsabermods) en el canal `#quest-mods`.

:::warning ¡Asegúrate de que tus Quest y PC están en la misma red y de que estás usando http y no https! :::

Abre BMBF en tus Quest y ve a la pestaña `Herramientas`, allí deberías ver una dirección web y un número de versión similar a lo que se muestra a continuación.

![ip](~@images/beginners-guide/ip.png)

En tu PC, abre tu navegador y escribe la dirección en la barra de búsqueda.

Deberías ver una pantalla como la que se muestra a continuación.

Si esto no funciona [haz clic aquí](#bmbf-web-interface-not-loading) para ver algunos pasos de solución de problemas.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Ahora simplemente arrastra cualquier mod compatible con Quest a la caja de subida y sincroniza. Si el mod fue creado originalmente para una versión anterior, entonces no se habilitará automáticamente. Para habilitar un mod antiguo, ve a la pestaña `Mods` y habilítalo desde allí.

## Instalar canciones
::: tip La mayoría de los mapas en los filtros "Top general", "Clasificación", "Descargas" o "Jugadas" se crearon antes de que se establecieran las buenas prácticas de mapeo. Intenta descargar canciones publicadas entre finales de 2019 y ahora para obtener la mejor experiencia de niveles personalizados. :::

### Dentro de tus Quest
Hay dos fuentes para obtener mapas personalizados dentro de tus Quest usando la ventana del navegador.

* Si estás buscando mapas y listas de reproducción supervisadas, visita [BeastSaber](https://bsaber.com/)
* Si no te gusta la interfaz de usuario de BeastSaber también puedes probar [BeatSaver](https://beatsaver.com/)

Ambos tienen un botón OneClickTM que instala fácilmente esa canción en tus Quest. Puedes cambiar entre estos sitios web usando el icono del globo en la parte superior derecha de la ventana del navegador.

Una forma fácil de descargar diferentes tipos de canciones es usar `Syncsaber` puedes acceder ahí yendo a BMBF en tus Quest y haciendo clic en la pestaña `Syncsaber`. Aquí puedes descargar canciones con el clic de un botón, puedes elegir entre diferentes "ajustes". Por ejemplo, puedes descargar las mejores 20 canciones en la sección "[hot](https://beatsaver.com/)" de Beatsaver o las 50 canciones rankeadas más duras.

Otro método es utilizar la función `Marcador` en [Beastsaber](https://bsaber.com/). Después de crear una cuenta, puedes hacer clic en un pequeño icono de marcadores en una canción y si más tarde eliminas todas tus canciones de la Búsqueda puedes volver a descargar las que están marcadas con OneClickTM.

### Usando tu PC
Si no puedes instalar canciones dentro de tu Quest, puedes instalar mapas usando tu ordenador parecido a la instalación de mods.

1. Visita [BeastSaber](https://bsaber.com/) o [BeatSaver](https://beatsaver.com/) en tu ordenador
2. Descarga el zip
3. Sigue los pasos de [Instalación de mods usando tu PC](#using-your-pc) hasta la pantalla de subir archivos.
4. Arrastra y suelta el mapa zip y debería estar instalado!

Si la interfaz web no carga [haz clic aquí](#bmbf-web-interface-not-loading) para ver algunos pasos de solución de problemas.

:::tip También puedes descargar listas de reproducción de la misma manera. Puedes encontrar varias listas de reproducción en [BeastSaber](https://bsaber.com/category/playlists/) o varios discords comunitarios. También puedes hacer el tuyo usando [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) o [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

Si quieres probar un mapa que has creado, ve la sección [Pruebas en unas Quest](/mapping/#testing-on-a-quest) en la sección de Mapeo de la Wiki para ver los pasos sobre empaquetarlo para probar! :::

## Instalando modelos
¡Únete a la comunidad de [Qosmetics](https://discord.gg/qosmetics) para cambiar cómo se ven en el juego el título de tu menú, sables, bloques o paredes!

## Enlaces útiles

* [Comunidad Qosmetics](https://discord.gg/qosmetics) - Servidor dedicado a hacer y usar sables, bloques y paredes para Quest.
* [Guías de creación de Qosmetics](https://github.com/RedBrumbler/Qosmetics/wiki) - Guías para crear tus propios sables, bloques y muros personalizados para las Quest.
* [Sitio web de Questboard](https://questmodding.com) - ¡Un lugar para obtener noticias e información relacionadas con Beat Saber junto con las últimas versiones de Mods!
* [Servidor de Discord de Questboard](https://discord.gg/P7sUKVnP) - Una comunidad de misiones para colgar y hablar sobre cosas relacionadas con Beat Saber , también puedes obtener un rol para ser notificado cuando un nuevo mod sea liberado!
* [Arreglando audio desincronizado](https://bsaber.com/quest-out-of-sync/)
* [Sable de puntuación](https://new.scoresaber.com/quest) - Marcadores de clasificación para canciones personalizadas.

## Resolución de problemas
:::warning He visto este video de Elite Eric, pero me he quedado atascado/no funcionó. ¿Qué proporciona? En BSMG **sugerimos encarecidamente** no usar ningún tutorial de Elite Eric. Después de revisar gran parte de su contenido, contienen una gran cantidad de información incompleta, errónea o directamente incorrecta. Desgraciadamente, los intentos de contactar con el para corregir estos errores se han encontrado con silencio y nuevos (también incorrectos) tutoriales.

En su lugar, deberías seguir las guías escritas aquí en la wiki o buscar ayuda en [el discord de BSMG](https://discord.gg/beatsabermods). :::

### Añadir mods de beatmods.com o modelos de modelsaber.com no funciona
La razón por la que añadir mods de [BeatMods](https://beatmods.com/) o modelos de [ModelSaber](https://modelsaber.com/) no funciona es porque esos mods y sables son sólo para PC.

Obtén Mods compatibles con Quest de [Questboard](https://www.questmodding.com/) o `#quest-mods` en el Grupo de discord de mods de Beat Saber, con sables compatibles con Quest, bloques y muros en la [Comunidad Qosmética](https://discord.gg/qosmetics). Una vez que tenga su mod o modelo zip utilice la [interfaz web BMBF](#using-your-pc) para instalarlo.

### Error al hacer Sideloading con BMBF
Al hacer Sideload con BMBF obtienes el error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Las firmas del paquete com.weloveoculus.BMBF no coinciden con la versión instalada anteriormente; ¡ignorando!`

Necesitarás desinstalar la versión BMBF en tu Quest. Puedes hacerlo desde el menú `Mis Aplicaciones` de SideQuest.

### Los mods esenciales no funcionan

Si estás teniendo problemas con los mods esenciales, por favor verifica que no estás intentando usar ningún mod desactualizado. Cualquier mod hecho para una versión anterior del juego se considera desactualizado. Una vez que los hayas eliminado:

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
Si tu interfaz web BMBF no está cargando, asegúrate de que estás escribiendo la IP de la pestaña de herramientas en el navegador de tu equipo que está en la misma red. Asegúrate de que:

1. 1) Tu IP no es `127.0.0.1`, si eso aparece prueba a reiniciar tu visor y/o router.
2. BMBF está abierto en los auriculares
3. Hay `http://` al principio del enlace, no `https://`
4. Tienes `:50000` al final de tu enlace
5. Tu PC y Quest están en la misma red wifi
6. Tu IP no ha cambiado ya que cambia de vez en cuando

Si ninguno de estos funciona, reinicia tus Quest y vuelve a pasar por la lista.

---

### BMBF no carga la configuración después de unos minutos
Esto se debe probablemente al uso de BMBF en una versión del juego para la que no se diseñó. Como usar BMBF para Beat Saber versión `1.13.0` cuando la versión del juego instalada en el visor sea `1.12.2`.  
Si la versión del juego coincide con la versión para la que la página de lanzamiento de BMBF dice que esta diseñado, intenta reiniciar el visor. Si todavía no funciona, utiliza la [interfaz web BMBF](#using-your-pc) y haz clic en `Corrección rápida` en la pestaña Herramientas.

### Beat Saber esta en negro cuando lo lanzo
Abre la biblioteca en tus Quest. Haz clic en los tres puntos al lado de Beat Saber y luego haz clic en `Permisos`. En el menú que aparece, habilita los permisos de almacenamiento e intenta iniciar el juego de nuevo.

---

### ¡Mis Sables y Mods no se activan/funcionan!
Esto probablemente se deba a tener un cliente BMBF anticuado, coge la última [versión de BMBF](https://bmbf.dev/stable). Si la versión de BMBF para tu Beat Saber no está ahí, por favor espera un tiempo a que los unicornios actualicen BMBF.

* Si se supone que tu mod es compatible con tu versión de BMBF, asegúrese de que no hay ninguna carpeta que separa el contenido del archivo .zip.
* Si tu nivel no se carga entonces intenta instalar extensiones de mapeo desde #quest-mods. También puede requerir las extensiones de mod Noodle que aún no están en las Quest.
* Si tu BMBF está en la última versión y los mods no están habilitados en el juego, desinstala Beat Saber con el botón de desinstalar BS en la pestaña BMBF Tools y despues reinstalar y remodear.
* En casos muy muy muy raros, BMBF no tiene permisos de archivo para copiar mods en la ubicación correcta. Compruebe en SideQuest para asegurarse de que BMBF tiene permisos de archivo.

---

### Beat Saber esta crasheando
Si tu juego está crasheando al hacer algo, desactiva tus mods uno por uno ejecutando tu juego cada vez para ver si el problema está solucionado antes de pedir ayuda en un canal de soporte.

### Sólo veo una pantalla blanca cuando abro BMBF
Si sólo ves una pantalla blanca cuando abres BMBF de fuentes desconocidas, reinicia tus Quest y entonces debería arreglarse

### ¡Mi Beat Saber tiene 3 puntos cuando lo inicio!
Si tu Saber de Beat está obteniendo 3 puntos al lanzar asegúrate que:

1. Has lanzado y jugado una canción antes de modificar el juego
2. No estás usando una versión pirata del juego
3. Asegúrate de estar usando la última versión de BMBF
