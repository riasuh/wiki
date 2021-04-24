---
sidebar: auto
---

# Quest Modding

## Vorwort

* Diese Anleitung ist sowohl für die Quest 1 als auch Quest 2.
* Niemand wurde bisher wegen Moddings gebannt.

::: danger DISCLAIMER Solltest Du Mods verwenden, sollte dir bewusst sein:

* Dass du möglicherweise Probleme bekommst, die im normalen Spiel nicht existieren. 99,9% aller Fehler, Abstürzen und Verzögerungen entstehen aufgrund von Mods.
* Mods werden durch Updates oft unbrauchbar und das ist normal - Bitte sei geduldig und respektvoll wenn dies passiert. Modder sind Freiwillige mit einem richtigen Leben.
* Beat Games versucht nicht mit Absicht, Mods kaputt zu machen. Sie versuchen an der Code-Grundlage zu arbeiten, welches Mods manchmal unbrauchbar macht. Dies geschieht aber nicht mit Absicht.

Bitte greife die Entwickler im Bezug mit Problemen bei Mods nicht an. Modder und Entwickler sind zwei verschiedene Gruppen. Sei kein Trottel. :::

:::warning Ich habe ein Video Tutorial angeschaut, aber es hägt/hat nicht funktioniert. Was bedeutet das? Wir, die BSMG raten **strikt** von Video Tutorials für's Modding ab. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Installation
Currently the only recommended way to install custom songs and mods is BMBF sideloaded with SideQuest using a PC.

If you do not have access to a PC you can use an [Android Phone](#installing-bmbf-with-an-android-phone).

* [BMBF Apk](https://bmbf.dev/stable) :::warning Wenn du BMBF installierst und du das Spiel modifizierst, wird der offizielle Multiplayer sowie das Anzeigen und Hochladen von Spielständen in den Basis-Spiel-Ranglisten deaktiviert. Wenn du den modifizierten Multiplayer spielen möchtest, benötigst du den Mod `Beat Together`, die Cross-Play zwischen Pc und Quest erlaubt und die Verwendung von Custom Songs, wenn beide Parteien den Song besitzen. Den Mod findest du in der Beat Saber Modding Group in `#quest-mods` oder auf der [Questboard](https://questmodding.com) Seite.

To get leaderboards on custom songs and to be able to get Performance Points (PP) from ranked songs you need the [ScoreSaber](https://new.scoresaber.com/quest) mod. [This link](https://new.scoresaber.com/quest) will take you to the ScoreSaber page to set it up. ScoreSaber does not replace the base game leaderboards, it only adds leaderboards for custom songs.

**Note:** Check the updates channel in the [ScoreSaber discord](https://discord.gg/WpuDMwU) to see if the mod is available for the current game version. :::

### BMBF mit SideQuest installieren
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

### BMBF mit einem Android Telefon installieren
This is **NOT** the recommended way to install BMBF and should only be used if you do not have access to a PC.

* [Anforderungen](#requirements)
* [Telefon einrichten](#setup-your-phone)
* [BMBF mit deinem Telefon installieren](#installing-bmbf-with-your-phone)
* [Beat Saber einrichten](#setup-beat-saber)

#### Anforderungen

* Ein Android-Telefon oder Android-Tablet (iPhones oder iPads werden nicht unterstützt)
* Eine **bezahlte** Version von Beat Saber im Oculus Quest Store
* Ein Kabel um deine Quest mit deinem Telefon zu verbinden (wenn dein Telefon über USB C geladen wird, sollte das Ladegerät, das mit deiner Quest mitgeliefert wurde, funktionieren).

#### Telefon einrichten

1. Lade die [bugjaeger-App aus dem Google Play Store](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US) herunter
2. Lade die neueste [BMBF APK von bmbf.dev/stable](https://bmbf.dev/stable) herunter.
3. Folge [dieser schriftlichen Anleitung](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ) zum Aktivieren des Entwicklermodus auf Deiner Quest zu aktivieren.
4. Entwicklermodus auf Deinem Telefon aktivieren
    1. Gehe in deine Android Einstellungen
    2. Scrolle zu "Über Telefon" und öffne es
    3. Tippe auf "Software Informationen"
    4. Tippe auf das Feld "Build number", bis der Entwicklermodus aktiviert ist. Dies sollte etwa 7 Tippe erfordern.
5. USB-Debugging auf Deinem Telefon aktivieren
    1. Zurück zu Einstellungen
    2. Tippe auf "Entwickleroptionen"
    3. USB-Debugging aktivieren

#### BMBF mit Deinem Telefon installieren
:::warning Before modding, run Beat Saber once, play a level and immediately fail! :::

Open bugjaeger on your Phone and connect your Quest. You should get a USB debugging pop-up in your Quest and on your phone. Select allow on both devices and if you prefer, select always allow. Once bugjaeger picks your Quest up, install the BMBF APK by doing following:

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

After you pressed ok, allow file access and select the download APK file which should be labeled `com.weloveoculus.BMBF.apk`. The apk file should now install to your Quest.

#### Beat Saber einrichten
After successfully installing BMBF onto your Quest you should be able to find it in your Quests library under unknown sources.

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

Open it and allow file access after starting it if prompted. Now follow the on-screen instructions carefully. After you finished you should see [BeastSaber](https://bsaber.com).

If at any point during the install process, you get the Restore App popup just click Close. This warning is directed to pirated versions of the game so there will likely be no consequences for ignoring it if you have a legitimate copy.

Now you can continue to the [Core Mods](#core-mods) step of the installation process.

## Speicherdaten verwalten

### Sichere Speicherdaten mit SideQuest

Open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber.

Navigate to `sdcard/Android/data/com.beatgames.beatsaber/files` using the SideQuest file explorer.

Save the files: `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` into a folder on your PC. Do not lose these, as they contain your scores and other settings!

### Sichere Speicherdaten mit SideQuest

To restore your data, open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber. Using the SideQuest file explorer take the 3 files you saved from the [Backup Save Data using SideQuest](#backup-save-data-using-sidequest) steps `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` and put them in the `sdcard/Android/data/com.beatgames.beatsaber/files` folder.

Go back to the menu and press the circular arrows located beside your latest backup. Your scores and settings should now be restored.

## Mods installieren

### Kern-Mods
Before installing any additional mods look in the top right of the BMBF web interface, you should see a red button that says, `Sync to Beat Saber`. Click this and let it finish syncing. Then go to your `mods` tab in BMBF. Make sure that you have the 5 core mods:

* Codegen
* Goodbye Bug
* PinkCore
* QuestUI
* Custom Types

:::danger All other mods will not work if these core mods are not listed and enabled.

If one of the core mods does not enable, delete that mod and click `Sync to Beat Saber` again to redownload it. Double check to see if it has been downloaded and enabled. If it still doesn't work, or mods are appear to be enabled, but not working in-game see [Core Mods don't work](#core-mods-don-t-work) for troubleshooting steps. :::

### In deiner Quest
:::warning Not all mods are available on QuestBoard!  
If a mod is not seen in here, you should follow the [Using Your PC](#using-your-pc) method instead. :::

Open BMBF in your Quest and go to the `Browser` tab, there you should see a globe icon similar to what's shown below. Click it, then click the `QuestBoard` button.

![globequestboard](~@images/beginners-guide/globequestboard.png)

You should be greeted with the [QuestBoard](https://www.questmodding.com/) website below. Next, select the `DOWNLOAD MODS` tab.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Scroll down with your thumbsticks. You can now select any mod from the list, seen below, and download it by hitting the download button next to it. Some downloads may redirect you to a website or GitHub page. If so, follow the instructions onscreen, or select the latest `.zip` in the Releases list, respectively.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Von deinem PC
You can find and download other Quest mods from the [BSMG Discord](https://discord.com/invite/beatsabermods) in the `#quest-mods` channel.

:::warning Make sure your Quest and PC are on the same network and that you are using http and not https! :::

Open BMBF in your Quest and go to the `Tools` tab, there you should see a web address and a version number similar to what's shown below.

![ip](~@images/beginners-guide/ip.png)

On your PC, open your browser and type the address into the search bar.

You should be greeted with this screen below.

If this doesn't work [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Now just drag any Quest compatible mods into the upload box and sync. If the mod was originally made for an older version, then it won't automatically enable. To enable an old mod, go to the `Mods` tab and enable it from there.

## Songs installieren
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

### In deiner Quest
There are 2 sources to getting custom maps inside your Quest using the browser window.

* Wenn du nach kuratierten Songs und Playlists suchst besuche [BeastSaber](https://bsaber.com/)
* Wenn du die Benutzeroberfläche von BeastSaber nicht magst kannst du [BeatSaver](https://beatsaver.com/) ausprobieren

Both have a OneClick™ button that easily installs that song onto your Quest. You can switch between these websites using the globe icon in the top right of the browser window.

An easy way to download different kinds of songs is to use `Syncsaber` you can access it by going into BMBF on your quest and clicking the tab called `Syncsaber`. Here you can download songs with a click of a button, you can choose from different "settings". For example you can download the top 20 songs in [Beatsaver's](https://beatsaver.com/) "hot" section or the 50 hardest ranked songs.

Another method is using the `Bookmark` feature on [Beastsaber](https://bsaber.com/). After creating an account you can click a little bookmark icon on a song and if you later delete all your songs from the Quest you can redownload the ones that are bookmarked with OneClick™.

### Von deinem PC
If you are unable to install songs inside your Quest, you can install maps using your computer similar to installing mods.

1. Öffne [BeastSaber](https://bsaber.com/) oder [BeatSaver](https://beatsaver.com/) auf deinem Computer
2. Lade die Zip herunter
3. Folge den [Installation von Mods mit Ihrem PC](#deinen-pc-benutzen) Schritte bis zum Upload Datei Bildschirm.
4. Ziehe die Song Zip in das Upload Feld und er sollte installiert werden!

If the web interface doesn't load [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

:::tip You can also download playlists in the same way. You can find various playlists on [Beastsaber](https://bsaber.com/category/playlists/) or various community discords. You can also make your own using [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) or [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

If you want to test a map you have created see the [Testing on a Quest](/mapping/#testing-on-a-quest) Section in the Mapping Wiki section for steps on packing it up for testing! :::

## Modelle installieren
Join the [Qosmetics Community](https://discord.gg/qosmetics) to change how your menu title, sabers, bloqs or walls look in-game!

## Nützliche Links

* [Qosmetics Community](https://discord.gg/qosmetics) - Ein Server spezialisiert auf das Machen und Nutzen von Sabern, Noten und Wänden für die Quest.
* [Qosmetics Creation Guides](https://github.com/RedBrumbler/Qosmetics/wiki) - Anleitungen zum Erstellen von eigenen Sabern, Noten und Wänden für die Quest.
* [Questboard website](https://questmodding.com) - Ein Ort um die neuesten Informationen und Nachrichten zum Thema Beat Saber und die neuesten Mod Versionen!
* [Questboard Discord Server](https://discord.gg/P7sUKVnP) - Eine Quest-Community zum chillen und reden über Beat Saber und ähnliches. Du kannst auch eine Rolle bekommen um benachrichtigt zu werden, wenn eine neue Mod veröffentlicht wird!
* [Beheben von Audiosynchronisationsfehlern](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - Ranglisten für eigene Songs im Spiel

## Problembehandlung
:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

### Das Hinzufügen von Mods von beatmods.com oder Modellen von modelsaber.com funktioniert nicht
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model zip use the [BMBF Web Interface](#using-your-pc) to install it.

### Sideloading von BMBF ist fehlgeschlagen
When sideloading BMBF you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Kern-Mods funktionieren nicht

If you are having problems with core mods, please verify that you are not trying to use any outdated mods. Any mod made for a previous game version is considered outdated. Once you have removed them:

1. Gehe zu `Tools`
2. Klicke auf `Exit BMBF`
3. Öffne BMBG erneut
4. Gehe nochmal zu `Tools`
5. Klicke auf `Quick Fix`
6. Gehe zum `Browser` Abschnitt der BMBF App.
7. Klicke auf das kleine Globus-Symbol in der oberen rechten Ecke
8. Klicke auf `QuestBoard`
9. Klicke auf `Download Mods`
10. Scrolle nach unten und klicke auf `Download All Core Mods`
11. Klicke dann auf `Sync to Beat Saber`

---

### Das BMBF Web Interface lädt nicht
If your BMBF Web Interface is not loading, be sure that you're typing the IP from the tools tab into your browser on your computer that's on the same network. Make sure that:

1. Deine IP nicht `127.0.0.1` ist. Wenn dies angezeigt wird, starte deine Quest und/oder Router neu.
2. BMBF im Headset geöffnet ist
3. Das `http://` am Anfang des Links steht, nicht `https://`
4. Du hast `:50000` am Ende des Links
5. Dein PC und deine Quest befinden sich im selben WLAN Netzwerk
6. Deine IP ist immer noch die gleiche, da sie sich von Zeit zu Zeit ändern kann

If none of these work, restart your Quest and go through the list again.

---

### BMBF lädt die Konfiguration nicht nach ein paar Minuten
This is likely due to using BMBF on a game version it was not built for. Such as using BMBF for Beat Saber version `1.13.0` when the version of the game installed on the headset is `1.12.2`.  
If the game version matches what the BMBF release page says its built for, try restarting your headset. If it still does not work use the [BMBF Web Interface](#using-your-pc) and click `Quick Fix` in the Tools tab.

### Beat Saber ist schwarz, wenn ich es starte
Open the library on your Quest. Click the three dots next to Beat Saber and then click `Permissions`. In the menu that pops up, enable storage permissions and try launching the game again.

---

### Meine Mods und Saber funktionieren/aktivieren sich nicht
This is most likely due to having an outdated BMBF App, grab the latest [BMBF Release](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* Wenn deine Mod mit deiner Version kompatibel ist, dann stelle sicher, dass es keinen Order gibt der den Inhalt der Zip separiert.
* Wenn ein Level nicht lädt, versuche die Mapping Extensions von #quest-mods zu installieren. Es kann auch die Mod Noodle Extensions benötigen, die noch nicht auf Quest verfügbar ist.
* Wenn BMBF auf der neuesten Version ist und Mods im Spiel nicht aktiviert werden, deinstalliere Beat Saber mit der Schaltfläche "BS Deinstallieren" im Abschnitt Tools, installiere das Spiel neu und führe Mods erneut aus.
* In sehr sehr seltenen Fällen hat BMBF keine Dateirechte, um Mods an den richtigen Ort zu kopieren. Überprüfe in SideQuest ob BMBF über alle Dateirechte verfügt.

---

### Beat Saber stürzt ab
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### Ich sehe nur einen weißen Bildschirm, wenn ich BMBF öffne
If you only see a white screen when you open BMBF from unknown sources, restart your quest and then it should be fixed

### Mein Spiel zeigt mir den Ladebildschirm in Dauerschleife
If your Beat Saber is getting 3 dots when launching make sure that:

1. Du hast einen Song gestartet und gespielt, bevor du das Spiel modifiziert hast
2. Du verwendest keine raubkopierte Version des Spiels
3. Stelle sicher, dass du die neueste Version von BMBF verwendest
