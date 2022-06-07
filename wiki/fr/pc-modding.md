---
sidebar: auto
---

# Modding sur PC

## Préface

:::danger AVIS DE NON-RESPONSABILITÉ En choisissant d'utiliser des mods, vous comprenez et acceptez que :

* Vous pouvez rencontrer des problèmes qui n'existent pas dans le jeu de base. 99.9% des bugs, plantages et ralentissements sont dus aux mods.
* Les mods sont susceptibles de ne plus fonctionner à cause des mises à jour et c'est normal - soyez patient et respectueux lorsque cela se produit, parce que les moddeurs sont bénévoles et ont une vie.
* Beat Games ne cherche pas volontairement à casser les mods. Ils souhaitent améliorer la base du jeu et parfois cela casse les mods, mais ce n'est pas dans leur objectif de tuer les mods.

N'attaquez pas les développeurs pour des problèmes relatifs aux mods, et inversement - les moddeurs et les développeurs sont deux groupes distincts. Ne sois pas idiot, d'accord ? :::

:::warning FAITES ATTENTION EN INSTALLANT DES MODS Beat Saber ne vous demandera **JAMAIS** de l'exécuter en tant qu'administrateur.

Si vous avez installé un mod et vous voyez la fenêtre de contrôle de compte d'utilisateur, **N'ACCEPTEZ PAS** et signalez ce mod. Ce que vous avez installé est un mod malveillant !

L'unique situation autorisée est l'activation ou la désactivation de la fonction OneClick™ de Mod Assistant. Les permissions administrateur sont requises pour enregistrer les liens OneClick™ avec Mod Assistant.

Si vous n'êtes pas sûr que ce que vous avez installé est un malware ou non, ***veuillez demander dans notre serveur Discord*** (en anglais). :::

Beat Saber supporte les chansons personnalisées de façon native, donc vous n'avez pas besoin de mods si c'est tout ce que vous cherchez ! Cela dit, il est judicieux d'installer `SongCore` puisque ce mod étend les fonctionnalités de base afin de raccourcir les temps de chargement et de fournir une base pour d'autres mods tels que le téléchargeur en jeu, les classements personnalisés, les playlists, etc.

::: warning This guide is for PC-modding on Windows.  
If you have a Quest, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux page](./linux-modding.md) or [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

If you run into problems at any point, please head to the [support page](./support/) and see if you can identify what went wrong before asking in the Discord server. Avec un peu de chance, la réponse que vous cherchez est déjà sur cette page !

::: warning J'ai suivi un tutoriel vidéo sur Youtube, mais ça coince/ne marche pas. Pourquoi ? Ici, nous recommandons **fortement** d'évviter les tutoriels vidéos pour modder le jeu. Nous remarquons souvent que ces vidéos sont obsolètes ou fournissent des informations incomplètes, erronées voire complètement fausses.

Vous devriez à la place suive les guides écrits ici sur le wiki, ou demander de l'aide dans le [Discord BSMG](https://discord.gg/beatsabermods) (anglophone). :::

## Installateurs

### Mod Assistant
> **CECI EST L'INSTALLATEUR DE MOD ACTUELLEMENT RECOMMANDÉ.**

__**Lancez le jeu au moins une fois**** avant d'essayer de modder votre jeu ! Ceci est valable aussi après une réinstallation.

Un installateur de mod Beat Saber simple, similaire à l'ancien Mod Manager, mais avec des fonctionnalités additionnelles telles que la suppression de mods et la vérification de version. Téléchargez-le sur [le GitHub d'Assistant](https://github.com/Assistant/ModAssistant/releases/latest).

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Comment avoir plus de chansons
::: tip
Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before
good mapping practices were established. Try downloading songs released between late 2019 and now to get the best
custom levels experience.
:::

::: warning It is a good idea to backup your `CustomLevels` folder periodically as there is a small chance it will be reset if the game updates!

This folder is located in your game install: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### Téléchargeur en jeu
The `BeatSaver Downloader` mod allows you to download maps in-game using the `MORE SONGS` menu button on the `MODS` menu screen. This pulls maps directly from [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) is the master repository of custom songs made by the community. Many other tools and sites enhance the experience of downloading custom songs, but this site is where they are stored. To install songs downloaded from the site, unzip them into a folder and place it into `Beat Saber/Beat Saber_Data/CustomLevels`. You can also use the in-game downloader mod, or Mod Assistant's OneClick™ Install feature.

To enable and use Mod Assistant's OneClick™ Install see the picture below: ![Mod Assistant](~@images/beginners-guide/modassistant-oneclick.png)

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) is a site that tries to help make finding fantastic maps to play easier. It does this by categorizing the thousands of songs on BeatSaver and lets you sort by a song's genre and many other attribute tags. It also has a full social feature where players can review songs and comment on them. One of the most used features is the "Curator Recommended" feature where a team plays through most songs released each day and recommends the ones that stand out, letting you [automatically download these in-game](https://bsaber.com/beatsync/).

### Applications de gestion des chansons

There are no working song management apps available at this time.

### Playlists
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* Utiliser l'outil `Installer une playlist` dans l'onglet Options de Mod Assistant.
* Placer le fichier de playlist dans `Beat Saber/Playlists` et sélectionnez la en jeu, puis appuyez sur le bouton *Download*.

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

## Dossier d'installation
_Where is Beat Saber installed?_

### Emplacement par défaut
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Autre emplacement
**If you have moved your install folder to a different drive, it might be in the location below.** Replace the drive letter `F` with the drive your game is installed on.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Installation manuelle
A mod installer is the recommended way to install mods. See the section [above](#installers). If you have patched the game and just need to install mods that are not available in the installer, skip to step 4.

::: warning STAY SAFE WHEN INSTALLING MODS Modding your game with unverified mods such as mods found in the `#pc-mods` channel comes with risks, including the possibility for malicious software that acts like a regular mod.

Beat Saber will **NEVER** ask you to run it as Administrator.

If you've downloaded and installed a mod and you get the User Account Control prompt, **DO NOT** click accept, and please report this. If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

**Run the game at least once** before trying to mod the game! This applies to reinstalling your game too.

### Installer BSIPA

1. Téléchargez [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Rendez vous dans [le dossier d'installation](#dossier-d-installation) et extrayez-y le contenu de BSIPA. ![Répertoire propre](~@images/beginners-guide/directory-clean.png "Répertoire propre") ![Répertoire avec IPA](~@images/beginners-guide/directory-ipa.png "Répertoire avec IPA")
3. Double-cliquez sur `IPA.exe` pour patcher le jeu. Chaque mod présent dans le dossier `Plugins` sera désormais chargé au lancement du jeu. En cas d'erreur, assurez-vous d'avoir bien suivi l'étape 2. ![Répertoire patché](~@images/beginners-guide/directory-patched.png "Répertoire patché")

### Installer les mods

4. Téléchargez le(s) mod(s) que vous souhaitez installer, que ce soit depuis GitHub, le salon `#pc-mods` du [Discord BSMG](https://discord.com/invite/beatsabermods), [BeatMods](https://beatmods.com/#/mods) ou d'autres sources. **Assurez-vous de télécharger toutes les dépendances requises pour chaque mod.** ![Répertoire Plugins](~@images/beginners-guide/directory-plugins.png "Répertoire Plugins")
5. Certains mods ont des instructions d'installation précises, certains non. Généralement, il suffit de glisser-déposer le contenu du zip dans le dossier d'installation du jeu, et les fichiers doivent aller dans les dossiers correspondants.

## Downgrading

Check `#modding-announcements` in [BSMG](https://www.discord.gg/beatsabermods) to see if the latest version is moddable. If it is not, you can follow these tutorials to downgrade to a moddable version.

Click on these links corresponding to where you own the game to see the tutorials.

* [Oculus Store](https://computerelite.github.io/tools/Oculus/OculusDowngraderGuide.html)
* For Steam you have a few options to be able to downgrade. These two are supported by [BSLG](https://discord.gg/MrwMx5e).
  * [BSLegacyLauncher](https://www.youtube.com/watch?v=qjNU5aENHRU)
  * [LegacyInstaller](https://github.com/Goobwabber/LegacyInstaller#readme)

## How to uninstall mods
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## Where to go from here

* [Grips and Tricks](./grips-and-tricks.md)
* [Making Beatmaps](/mapping/)
* [Custom Sabers](/models/custom-sabers.md)
* [Custom Avatars](/models/custom-avatars.md)
* [Custom Platforms](/models/custom-platforms.md)
* [Play Customs in Multiplayer](https://discord.com/invite/gezGrFG4tz)
* [Making Mods](/modding/)

## Have questions?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
