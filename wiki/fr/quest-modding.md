---
sidebar: auto
---

# Modding sur Quest

## Préface

* Ce guide concerne à la fois le Quest 1 et le Quest 2.
* Personne n'a encore été banni pour avoir moddé.

:::danger AVIS DE NON-RESPONSABILITÉ En choisissant d'utiliser des mods, vous comprenez et acceptez que :

* Vous pouvez rencontrer des problèmes qui n'existent pas dans le jeu de base. 99,9 % des bugs, des plantages et des ralentissements sont dus aux mods.
* Les mods sont susceptibles de ne plus fonctionner après une mise à jour et c'est normal - soyez patient et respectueux lorsque cela se produit, parce que les moddeurs sont bénévoles et ont une vie.
* Beat Games ne cherche pas volontairement à casser les mods. Ils souhaitent améliorer la base du jeu et parfois cela casse les mods, mais ce n'est pas dans leur objectif de tuer les mods.

N'attaquez pas les développeurs pour des problèmes relatifs aux mods, et inversement - les moddeurs et les développeurs sont deux groupes distincts. Ne sois pas idiot, d'accord ? :::

:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. Pourquoi ? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

À la place, vous devriez suivre les guides écrits ici sur le wiki ou chercher de l'aide dans le [Discord BSMG](https://discord.gg/beatsabermods) (anglophone). :::

## Installation
Actuellement, le seul moyen recommandé pour installer les mods et chansons personnalisées sont via BMBF, installé avec SideQuest depuis un PC.

Si vous n'avez pas accès à un ordinateur, vous pouvez utiliser [un téléphone Android](#installer-bmbf-avec-un-telephone-android).

* [APK BMBF](https://bmbf.dev/stable) :::warning ATTENTION Installer BMBF et modifier votre jeu désactive le multijoueur officiel, ainsi que l'affichage et l'envoi de scores dans les classements du jeu de base. Si vous souhaitez jouer en multijoueur en étant moddé, vous aurez besoin du mod `Beat Together` qui permet de jouer en multijoueur avec des joueurs PC et Quest, et permet de jouer des chansons personnalisées si tous les joueurs les ont installées. Le mod peut être trouvé dans `#quest-mods` dans le Discord BSMG, ou bien sur [Questboard](https://questmodding.com).

Pour obtenir les classements sur les chansons personnalisées et gagner des points de performance (PP) sur les chansons classées, vous avez besoin du mod [ScoreSaber](https://new.scoresaber.com/quest). [Ce lien](https://new.scoresaber.com/quest) (en anglais) vous enverra sur la page du site ScoreSaber vous permettant de l'installer. ScoreSaber ne remplace pas les classements du jeu de base, il ne fait qu'ajouter les classements pour les chansons personnalisées.

**Note :** Consultez le salon *#updates* du [serveur Discord ScoreSaber](https://discord.gg/WpuDMwU) pour vérifier si le mod est disponible pour la version actuelle du jeu. :::

### Installer BMBF avec SideQuest
Si ce n'est pas déjà fait, téléchargez et installez [SideQuest](https://sidequestvr.com/#/setup-howto) (en anglais).

Ouvrez SideQuest et connectez votre Quest à votre PC.

:::tip ASTUCE Si vous avez précédemment moddé Beat Saber ou avez des scores à sauvegarder, [sauvegardez vos données d'abord](#sauvegarder-les-donnees-de-sauvegarde-avec-sidequest) ! :::

Si vous avez déjà moddé le jeu, vous devez également le désinstaller en appuyant sur le bouton `UNINSTALL APP`. Vous pourrez restaurer votre sauvegarde depuis le même menu, après le modding.

Cliquez sur le bouton `Install APK from folder` comme indiqué ci-dessous et sélectionnez le fichier APK BMBF que vous avez téléchargé, ou glissez simplement le fichier APK dans la fenêtre de SideQuest. Ces deux méthodes vont installer BMBF sur votre Quest.

![Installation d'APK](~@images/beginners-guide/apkfromfolder.png)

Une fois installé avec succès, assurez-vous que la dernière version de Beat Saber est installée et non moddée.

:::warning Before modding, run Beat Saber once, play a level and immediately fail!

Modding currently does not work if the experimental multi-user feature is in use. You will need to temporarily remove all secondary accounts before modding the game. You can add them back later once you have installed your desired mods. :::

After running Beat Saber once, open BMBF from unknown sources as the picture below shows. ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

Follow each step exactly as you're told. Then, you should see [bsaber.com](https://www.bsaber.com). This is where you can download any custom songs available. You can also click on the globe icon in the top right and go to beatsaver to download songs too.

If at any point during the install process, you get the `Restore App` popup just click `Close`. This warning is more directed to pirated versions of the game so if you're just modding there will likely be no consequences for ignoring it.

![RestoreApp](~@images/beginners-guide/restoreapp.png)

Continue to the [Core Mods](#core-mods) step of the installation process.

### Installer BMBF avec un téléphone Android
This is **NOT** the recommended way to install BMBF and should only be used if you do not have access to a PC.

* [Prérequis](#prerequis)
* [Préparer votre téléphone](#preparer-votre-telephone)
* [Installer BMBF avec votre téléphone](#installer-bmbf-avec-votre-telephone)
* [Préparer Beat Saber](#preparer-beat-saber)

#### Prérequis

* Un téléphone Android ou une tablette Android (les iPhones ou iPads ne sont pas pris en charge)
* Une version **payante** de Beat Saber sur le Store Oculus Quest
* Un câble pour connecter votre Quest à votre téléphone (si votre téléphone dispose d'un port USB C, le chargeur inclus avec votre Quest devrait fonctionner)

#### Préparer votre téléphone

1. Téléchargez l'application [Bugjaeger depuis le Google Play Store](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)
2. Téléchargez l'APK BMBF le plus récent depuis [bmbf.dev/stable](https://bmbf.dev/stable)
3. Suivez [ce guide écrit](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ) (en anglais) pour activer le mode développeur sur votre Quest.
4. Activez le mode développeur sur votre téléphone
    1. Allez dans vos paramètres Android
    2. Faites défiler jusqu'à "À propos du téléphone" et cliquez dessus
    3. Ouvrez "Information sur le logiciel"
    4. Appuyez sur le champ "Numéro de build" jusqu'à ce que le mode développeur soit activé. Cela devrait prendre environ 7 appuis.
5. Activez le débogage USB sur votre téléphone
    1. Retournez dans les paramètres
    2. Appuyez sur "Options pour les développeurs"
    3. Activez le débogage USB

#### Installer BMBF avec votre téléphone
:::warning Before modding, run Beat Saber once, play a level and immediately fail! :::

Open bugjaeger on your Phone and connect your Quest. You should get a USB debugging pop-up in your Quest and on your phone. Select allow on both devices and if you prefer, select always allow. Once bugjaeger picks your Quest up, install the BMBF APK by doing following:

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

After you pressed ok, allow file access and select the download APK file which should be labeled `com.weloveoculus.BMBF.apk`. The apk file should now install to your Quest.

#### Préparer Beat Saber
After successfully installing BMBF onto your Quest you should be able to find it in your Quests library under unknown sources.

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

Open it and allow file access after starting it if prompted. Now follow the on-screen instructions carefully. After you finished you should see [BeastSaber](https://bsaber.com).

If at any point during the install process, you get the Restore App popup just click Close. This warning is directed to pirated versions of the game so there will likely be no consequences for ignoring it if you have a legitimate copy.

Now you can continue to the [Core Mods](#core-mods) step of the installation process.

## Gérer les données de sauvegarde

### Sauvegarder les données de sauvegarde avec SideQuest

Open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber.

Navigate to `sdcard/Android/data/com.beatgames.beatsaber/files` using the SideQuest file explorer.

Save the files: `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` into a folder on your PC. Do not lose these, as they contain your scores and other settings!

### Restaurer les données de sauvegarde avec SideQuest

To restore your data, open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber. Using the SideQuest file explorer take the 3 files you saved from the [Backup Save Data using SideQuest](#backup-save-data-using-sidequest) steps `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` and put them in the `sdcard/Android/data/com.beatgames.beatsaber/files` folder.

Go back to the menu and press the circular arrows located beside your latest backup. Your scores and settings should now be restored.

## Installer les mods

### Mods essentiels
Before installing any additional mods look in the top right of the BMBF web interface, you should see a red button that says, `Sync to Beat Saber`. Click this and let it finish syncing. Then go to your `mods` tab in BMBF. Make sure that you have the 5 core mods:

* Codegen
* Goodbye Bug
* PinkCore
* QuestUI
* Custom Types

:::danger All other mods will not work if these core mods are not listed and enabled.

If one of the core mods does not enable, delete that mod and click `Sync to Beat Saber` again to redownload it. Double check to see if it has been downloaded and enabled. If it still doesn't work, or mods are appear to be enabled, but not working in-game see [Core Mods don't work](#core-mods-don-t-work) for troubleshooting steps. :::

### Depuis votre Quest
:::warning Not all mods are available on QuestBoard!  
If a mod is not seen in here, you should follow the [Using Your PC](#using-your-pc) method instead. :::

Open BMBF in your Quest and go to the `Browser` tab, there you should see a globe icon similar to what's shown below. Click it, then click the `QuestBoard` button.

![globequestboard](~@images/beginners-guide/globequestboard.png)

You should be greeted with the [QuestBoard](https://www.questmodding.com/) website below. Next, select the `DOWNLOAD MODS` tab.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Scroll down with your thumbsticks. You can now select any mod from the list, seen below, and download it by hitting the download button next to it. Some downloads may redirect you to a website or GitHub page. If so, follow the instructions onscreen, or select the latest `.zip` in the Releases list, respectively.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Depuis votre PC
You can find and download other Quest mods from the [BSMG Discord](https://discord.com/invite/beatsabermods) in the `#quest-mods` channel.

:::warning Make sure your Quest and PC are on the same network and that you are using http and not https! :::

Open BMBF in your Quest and go to the `Tools` tab, there you should see a web address and a version number similar to what's shown below.

![ip](~@images/beginners-guide/ip.png)

On your PC, open your browser and type the address into the search bar.

You should be greeted with this screen below.

If this doesn't work [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Now just drag any Quest compatible mods into the upload box and sync. If the mod was originally made for an older version, then it won't automatically enable. To enable an old mod, go to the `Mods` tab and enable it from there.

## Installer des maps
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

### Depuis votre Quest
There are 2 sources to getting custom maps inside your Quest using the browser window.

* Si vous cherchez des maps et des playlists organisées, visitez [BeastSaber](https://bsaber.com/)
* Si vous n'aimez pas l'interface de BeastSaber vous pouvez aussi essayer [BeatSaver](https://beatsaver.com/)

Both have a OneClick™ button that easily installs that song onto your Quest. You can switch between these websites using the globe icon in the top right of the browser window.

An easy way to download different kinds of songs is to use `Syncsaber` you can access it by going into BMBF on your quest and clicking the tab called `Syncsaber`. Here you can download songs with a click of a button, you can choose from different "settings". For example you can download the top 20 songs in [Beatsaver's](https://beatsaver.com/) "hot" section or the 50 hardest ranked songs.

Another method is using the `Bookmark` feature on [Beastsaber](https://bsaber.com/). After creating an account you can click a little bookmark icon on a song and if you later delete all your songs from the Quest you can redownload the ones that are bookmarked with OneClick™.

### Depuis votre PC
If you are unable to install songs inside your Quest, you can install maps using your computer similar to installing mods.

1. Visitez [BeastSaber](https://bsaber.com/) ou [BeatSaver](https://beatsaver.com/) sur votre ordinateur
2. Téléchargez le zip
3. Suivez les instructions d'[installation de mods avec votre PC](#depuis-votre-pc) jusqu'à l'écran d'envoi de fichiers.
4. Glissez et déposez le zip de la map et elle devrait s'installer !

If the web interface doesn't load [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

:::tip You can also download playlists in the same way. You can find various playlists on [Beastsaber](https://bsaber.com/category/playlists/) or various community discords. You can also make your own using [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) or [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

If you want to test a map you have created see the [Testing on a Quest](/mapping/#testing-on-a-quest) Section in the Mapping Wiki section for steps on packing it up for testing! :::

## Installer des modèles
Join the [Qosmetics Community](https://discord.gg/qosmetics) to change how your menu title, sabers, bloqs or walls look in-game!

## Liens utiles

* [Qosmetics Community](https://discord.gg/qosmetics) (en anglais) - un serveur dédié à la création et l'utilisation de sabres, bloqs, et murs pour Quest
* [Guides de création des Qosmetics](https://github.com/RedBrumbler/Qosmetics/wiki) (en anglais) - des guides sur la création de vos propres sabres, bloqs et murs personnalisés sur Quest
* [Site de Questboard](https://questmodding.com) - un site pour obtenir des nouvelles sur Beat Saber ainsi que les derniers mods publiés
* [Serveur Discord Questboard](https://discord.gg/P7sUKVnP) - une communauté Quest pour discuter de choses en lien avec Beat Saber, où vous pouvez également obtenir un rôle pour être notifié des nouveaux mods publiés
* [Corriger les problèmes de synchronisation audio (en anglais)](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - classements en jeu pour les chansons personnalisées

## Dépannage
:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

### Ajouter des mods de beatmods.com ou des modèles de modelsaber.com ne fonctionne pas
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model zip use the [BMBF Web Interface](#using-your-pc) to install it.

### BMBF refuse de s'installer
When sideloading BMBF you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Les mods essentiels ne fonctionnent pas

If you are having problems with core mods, please verify that you are not trying to use any outdated mods. Any mod made for a previous game version is considered outdated. Once you have removed them:

1. Allez dans `Tools`
2. Cliquez `Exit BMBF`
3. Ouvrez à nouveau BMBF
4. Allez à nouveau dans `Tools`
5. Cliquez sur `Quick Fix`
6. Allez dans la section `Browser` de BMBF
7. Cliquez sur l'icône de globe dans le coin supérieur droit
8. Cliquez sur `QuestBoard`
9. Cliquez sur `Download Mods`
10. Défilez et cliquez sur `Download All Core Mods`
11. Cliquez sur `Sync to Beat Saber`

---

### L'interface web BMBF ne charge pas
If your BMBF Web Interface is not loading, be sure that you're typing the IP from the tools tab into your browser on your computer that's on the same network. Make sure that:

1. Votre IP n'est pas `127.0.0.1`, si c'est le cas essayez de redémarrer votre casque et/ou votre routeur.
2. BMBF est ouvert dans votre casque
3. Le lien commence par `http://` et non pas `https://`
4. Vous avez `:50000` à la fin de votre lien
5. Votre PC et votre Quest sont sur le même réseau Wi-Fi
6. Votre IP n'a pas changé, car elle peut changer de temps en temps

If none of these work, restart your Quest and go through the list again.

---

### BMBF ne charge pas la configuration après quelques minutes
This is likely due to using BMBF on a game version it was not built for. Such as using BMBF for Beat Saber version `1.13.0` when the version of the game installed on the headset is `1.12.2`.  
If the game version matches what the BMBF release page says its built for, try restarting your headset. If it still does not work use the [BMBF Web Interface](#using-your-pc) and click `Quick Fix` in the Tools tab.

### Beat Saber est noir quand je le lance
Open the library on your Quest. Click the three dots next to Beat Saber and then click `Permissions`. In the menu that pops up, enable storage permissions and try launching the game again.

---

### Mes sabres et mods ne s'activent pas/ne fonctionnent pas
This is most likely due to having an outdated BMBF App, grab the latest [BMBF Release](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* Si votre mod est normalement compatible avec votre version de BMBF, assurez-vous qu'il n'y a pas de dossier séparant le contenu du fichier `.zip`.
* Si votre niveau ne charge pas, essayez d'installer Mapping Extensions depuis `#quest-mods`. Il peut aussi nécessiter le mod Noodle Extensions qui n'est pas encore disponible sur Quest.
* Si votre BMBF est à jour et les mods ne s'activent pas une fois dans le jeu, désinstallez Beat Saber avec le bouton "Uninstall BS" dans l'onglet Tools de BMBF puis réinstallez et remoddez.
* Dans de très, très rares cas, BMBF n'a pas les permissions de copier les mods au bon endroit. Allez donc vérifier dans SideQuest pour vous assurer que BMBF a les droits requis pour gérer les fichiers.

---

### Beat Saber plante
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### BMBF affiche uniquement un écran blanc
If you only see a white screen when you open BMBF from unknown sources, restart your quest and then it should be fixed

### Beat Saber affiche 3 points au lancement
If your Beat Saber is getting 3 dots when launching make sure that:

1. Vous avez lancé et joué une chanson avant de modifier le jeu
2. Vous n'utilisez pas une version piratée du jeu
3. Vous utilisez la dernière version de BMBF
