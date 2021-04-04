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

:::warning I watched this video by Elite Eric or FluffySez, but I got stuck/it didn't work. What gives? We at BSMG **strongly** suggest against using any tutorials by Elite Eric or FluffySez. After reviewing much of their content, they contain a large amount of incomplete, erroneous, or straight up incorrect information. Attempts to reach out to correct these errors has unfortunately not been successful.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Instalación
Currently the only recommended way to install custom songs and mods is BMBF sideloaded with SideQuest using a PC.

If you do not have access to a PC you can use an [Android Phone](#installing-bmbf-with-an-android-phone).

* [BMBF apk](https://bmbf.dev/stable) :::warning Instalar BMBF y modear tu juego deshabilitará el Multijugador Oficial, así como ver y subir puntuaciones en los marcadores del juego base. Si quieres jugar multijugador con mods, necesitas el mod, `Beat Together`, que permite el juego cruzado entre pc y Quest y permite que se usen canciones personalizadas si todas las partes tienen dicha canción. El mod se puede encontrar en el Beat Saber Modding Group en `#quest-mods` o en el sitio [Questboard](https://questmodding.com).

To get leaderboards on custom songs and to be able to get Performance Points (PP) from ranked songs you need the [ScoreSaber](https://new.scoresaber.com/quest) mod. [This link](https://new.scoresaber.com/quest) will take you to the ScoreSaber page to set it up. ScoreSaber does not replace the base game leaderboards, it only adds leaderboards for custom songs.

**Note:** Check the updates channel in the [ScoreSaber discord](https://discord.gg/WpuDMwU) to see if the mod is available for the current game version. :::

### Instalar BMBF con SideQuest
If you haven't already, download and setup [SideQuest](https://sidequestvr.com/#/setup-howto)

Open SideQuest and connect your Quest to your PC.

:::tip If you've previously modded Beat Saber or have scores you want to backup, [Backup your Save Data first!](#backup-save-data-using-sidequest) :::

If you have a modded game you also need to uninstall it by pressing the `UNINSTALL APP` button. You can later restore your save from the same menu, after modding.

Select the `Install APK from folder` button shown below and find the latest BMBF apk you downloaded and click on it, or simply drag the BMBF apk into SideQuest. Either method will install BMBF to your Quest.

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

Once it has been successfully installed, make sure you have the latest version of Beat Saber installed and unmodded.

:::warning Before modding, run Beat Saber once, play a level and immediately fail! :::

After running Beat Saber once, open BMBF from unknown sources as the picture below shows. ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

Follow each step exactly as you're told. Then, you should see [bsaber.com](https://www.bsaber.com). This is where you can download any custom songs available. You can also click on the globe icon in the top right and go to beatsaver to download songs too.

If at any point during the install process, you get the `Restore App` popup just click `Close`. This warning is more directed to pirated versions of the game so if you're just modding there will likely be no consequences for ignoring it.

![RestoreApp](~@images/beginners-guide/restoreapp.png)

Continue to the [Core Mods](#core-mods) step of the installation process.

### Instalando BMBF con un teléfono Android
This is **NOT** the recommended way to install BMBF and should only be used if you do not have access to a PC.

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
:::warning Before modding, run Beat Saber once, play a level and immediately fail! :::

Open bugjaeger on your Phone and connect your Quest. You should get a USB debugging pop-up in your Quest and on your phone. Select allow on both devices and if you prefer, select always allow. Once bugjaeger picks your Quest up, install the BMBF APK by doing following:

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

After you pressed ok, allow file access and select the download APK file which should be labeled `com.weloveoculus.BMBF.apk`. The apk file should now install to your Quest.

#### Configurar Beat Saber
After successfully installing BMBF onto your Quest you should be able to find it in your Quests library under unknown sources.

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

Open it and allow file access after starting it if prompted. Now follow the on-screen instructions carefully. After you finished you should see [BeastSaber](https://bsaber.com).

If at any point during the install process, you get the Restore App popup just click Close. This warning is directed to pirated versions of the game so there will likely be no consequences for ignoring it if you have a legitimate copy.

Now you can continue to the [Core Mods](#core-mods) step of the installation process.

## Administrar datos guardados

### Copia de seguridad de datos usando SideQuest

Open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber.

Navigate to `sdcard/Android/data/com.beatgames.beatsaber/files` using the SideQuest file explorer.

Save the files: `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` into a folder on your PC. Do not lose these, as they contain your scores and other settings!

### Restaurar datos guardados usando SideQuest

To restore your data, open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber. Using the SideQuest file explorer take the 3 files you saved from the [Backup Save Data using SideQuest](#backup-save-data-using-sidequest) steps `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` and put them in the `sdcard/Android/data/com.beatgames.beatsaber/files` folder.

Go back to the menu and press the circular arrows located beside your latest backup. Your scores and settings should now be restored.

## Instalar mods

### Mods esenciales
Before installing any additional mods look in the top right of the BMBF web interface, you should see a red button that says, `Sync to Beat Saber`. Click this and let it finish syncing. Then go to your `mods` tab in BMBF. Make sure that you have the 5 core mods:

* Codegen
* Goodbye bug
* PinkCore
* QuestUI
* Custom Types

:::danger All other mods will not work if these core mods are not listed and enabled.

If one of the core mods does not enable, delete that mod and click `Sync to Beat Saber` again to redownload it. Double check to see if it has been downloaded and enabled. If it still doesn't work, or mods are appear to be enabled, but not working in-game see [Core Mods don't work](#core-mods-don-t-work) for troubleshooting steps. :::

### Dentro de tus Quest
:::warning Not all mods are available on QuestBoard!  
If a mod is not seen in here, you should follow the [Using Your PC](#using-your-pc) method instead. :::

Open BMBF in your Quest and go to the `Browser` tab, there you should see a globe icon similar to what's shown below. Click it, then click the `QuestBoard` button.

![globequestboard](~@images/beginners-guide/globequestboard.png)

You should be greeted with the [QuestBoard](https://www.questmodding.com/) website below. Next, select the `DOWNLOAD MODS` tab.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Scroll down with your thumbsticks. You can now select any mod from the list, seen below, and download it by hitting the download button next to it. Some downloads may redirect you to a website or GitHub page. If so, follow the instructions onscreen, or select the latest `.zip` in the Releases list, respectively.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Usando tu PC
You can find and download other Quest mods from the [BSMG Discord](https://discord.com/invite/beatsabermods) in the `#quest-mods` channel.

:::warning Make sure your Quest and PC are on the same network and that you are using http and not https! :::

Open BMBF in your Quest and go to the `Tools` tab, there you should see a web address and a version number similar to what's shown below.

![ip](~@images/beginners-guide/ip.png)

On your PC, open your browser and type the address into the search bar.

You should be greeted with this screen below.

If this doesn't work [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Now just drag any Quest compatible mods into the upload box and sync. If the mod was originally made for an older version, then it won't automatically enable. To enable an old mod, go to the `Mods` tab and enable it from there.

## Instalar canciones
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

### Dentro de tus Quest
There are 2 sources to getting custom maps inside your Quest using the browser window.

* Si estás buscando mapas y listas de reproducción supervisadas, visita [BeastSaber](https://bsaber.com/)
* Si no te gusta la interfaz de usuario de BeastSaber también puedes probar [BeatSaver](https://beatsaver.com/)

Both have a OneClick™ button that easily installs that song onto your Quest. You can switch between these websites using the globe icon in the top right of the browser window.

An easy way to download different kinds of songs is to use `Syncsaber` you can access it by going into BMBF on your quest and clicking the tab called `Syncsaber`. Here you can download songs with a click of a button, you can choose from different "settings". For example you can download the top 20 songs in [Beatsaver's](https://beatsaver.com/) "hot" section or the 50 hardest ranked songs.

Another method is using the `Bookmark` feature on [Beastsaber](https://bsaber.com/). After creating an account you can click a little bookmark icon on a song and if you later delete all your songs from the Quest you can redownload the ones that are bookmarked with OneClick™.

### Usando tu PC
If you are unable to install songs inside your Quest, you can install maps using your computer similar to installing mods.

1. Visita [BeastSaber](https://bsaber.com/) o [BeatSaver](https://beatsaver.com/) en tu ordenador
2. Descarga el zip
3. Sigue los pasos de [Instalación de mods usando tu PC](#using-your-pc) hasta la pantalla de subir archivos.
4. Arrastra y suelta el mapa zip y debería estar instalado!

If the web interface doesn't load [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

:::tip You can also download playlists in the same way. You can find various playlists on [Beastsaber](https://bsaber.com/category/playlists/) or various community discords. You can also make your own using [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) or [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

If you want to test a map you have created see the [Testing on a Quest](/mapping/#testing-on-a-quest) Section in the Mapping Wiki section for steps on packing it up for testing! :::

## Instalando modelos
Join the [Qosmetics Community](https://discord.gg/qosmetics) to change how your menu title, sabers, bloqs or walls look in-game!

## Enlaces útiles

* [Comunidad Qosmetics](https://discord.gg/qosmetics) - Servidor dedicado a hacer y usar sables, bloques y paredes para Quest.
* [Guías de creación de Qosmetics](https://github.com/RedBrumbler/Qosmetics/wiki) - Guías para crear tus propios sables, bloques y muros personalizados para las Quest.
* [Sitio web de Questboard](https://questmodding.com) - ¡Un lugar para obtener noticias e información relacionadas con Beat Saber junto con las últimas versiones de Mods!
* [Questboard discord server](https://discord.gg/P7sUKVnP) - A quest community to hangout and talk about Beat Saber related stuff, you can also get a role to get notified when a new mod gets released!
* [Arreglando audio desincronizado](https://bsaber.com/quest-out-of-sync/)
* [Sable de puntuación](https://new.scoresaber.com/quest) - Marcadores de clasificación para canciones personalizadas.

## Resolución de problemas
:::warning I watched this video by Elite Eric or FluffySez, but I got stuck/it didn't work. What gives? We at BSMG **strongly** suggest against using any tutorials by Elite Eric or FluffySez. After reviewing much of their content, they contain a large amount of incomplete, erroneous, or straight up incorrect information. Attempts to reach out to correct these errors has unfortunately not been successful.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

### Añadir mods de beatmods.com o modelos de modelsaber.com no funciona
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model zip use the [BMBF Web Interface](#using-your-pc) to install it.

### Error al hacer Sideloading con BMBF
When sideloading BMBF you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Los mods esenciales no funcionan

If you are having problems with core mods, please verify that you are not trying to use any outdated mods. Any mod made for a previous game version is considered outdated. Once you have removed them:

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
If your BMBF Web Interface is not loading, be sure that you're typing the IP from the tools tab into your browser on your computer that's on the same network. Make sure that:

1. 1) Tu IP no es `127.0.0.1`, si eso aparece prueba a reiniciar tu visor y/o router.
2. BMBF está abierto en los auriculares
3. Hay `http://` al principio del enlace, no `https://`
4. Tienes `:50000` al final de tu enlace
5. Tu PC y Quest están en la misma red wifi
6. Tu IP no ha cambiado ya que cambia de vez en cuando

If none of these work, restart your Quest and go through the list again.

---

### BMBF no carga la configuración después de unos minutos
This is likely due to using BMBF on a game version it was not built for. Such as using BMBF for Beat Saber version `1.13.0` when the version of the game installed on the headset is `1.12.2`.  
If the game version matches what the BMBF release page says its built for, try restarting your headset. If it still does not work use the [BMBF Web Interface](#using-your-pc) and click `Quick Fix` in the Tools tab.

### Beat Saber esta en negro cuando lo lanzo
Open the library on your Quest. Click the three dots next to Beat Saber and then click `Permissions`. In the menu that pops up, enable storage permissions and try launching the game again.

---

### ¡Mis Sables y Mods no se activan/funcionan!
This is most likely due to having an outdated BMBF App, grab the latest [BMBF Release](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* Si se supone que tu mod es compatible con tu versión de BMBF, asegúrese de que no hay ninguna carpeta que separa el contenido del archivo .zip.
* Si tu nivel no se carga entonces intenta instalar extensiones de mapeo desde #quest-mods. También puede requerir las extensiones de mod Noodle que aún no están en las Quest.
* Si tu BMBF está en la última versión y los mods no están habilitados en el juego, desinstala Beat Saber con el botón de desinstalar BS en la pestaña BMBF Tools y despues reinstalar y remodear.
* En casos muy muy muy raros, BMBF no tiene permisos de archivo para copiar mods en la ubicación correcta. Compruebe en SideQuest para asegurarse de que BMBF tiene permisos de archivo.

---

### Beat Saber esta crasheando
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### Sólo veo una pantalla blanca cuando abro BMBF
If you only see a white screen when you open BMBF from unknown sources, restart your quest and then it should be fixed

### ¡Mi Beat Saber tiene 3 puntos cuando lo inicio!
If your Beat Saber is getting 3 dots when launching make sure that:

1. Has lanzado y jugado una canción antes de modificar el juego
2. No estás usando una versión pirata del juego
3. Asegúrate de estar usando la última versión de BMBF
