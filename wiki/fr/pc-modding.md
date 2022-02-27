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

The only approved case is when activating/deactivating OneClick™ Install in Mod Assistant. Administrator access is required to register the program with your computer to handle OneClick™ Install links.

If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

Beat Saber natively supports custom songs, so if that's all you're looking for, you don't require more mods! It's a wise idea to install `SongCore` though, as this mod expands upon the base game functionality to improve loading times and provide functionality for other mods like the in-game downloader, custom leaderboards, playlists, etc.

::: warning This guide is for PC-modding on Windows.  
If you have a Quest, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux page](/modding/linux.md) or [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

If you run into problems at any point, please head to the [support page](./support) and see if you can identify what went wrong before asking in the Discord server. Chances are, your answer is on that page!

::: warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** suggest against using video tutorials for modding. Often, we find they are outdated or contain a incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Installateurs

### Mod Assistant
> **CECI EST L'INSTALLATEUR DE MOD ACTUELLEMENT RECOMMANDÉ.**

__**Run the game at least once**** before trying to mod the game! This applies to reinstalling your game too.

A simple Beat Saber Mod Installer similar to the mod manager, but with additional features such as mod removal and version checking! Get it on [Assistant's GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Comment avoir plus de chansons
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

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

## Comment désinstaller les mods
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## Où se rendre d'ici

* [Prises et Astuces](./grips-and-tricks.md)
* [Créer ses propres niveaux](/fr/mapping/)
* [Sabres personnalisés](/fr/models/custom-sabers.md)
* [Avatars personnalisés](/fr/models/custom-avatars.md)
* [Plateformes personnalisées](/fr/models/custom-platforms.md)
* [Jouer des chansons personnalisées en multijoueur](https://discord.com/invite/gezGrFG4tz)
* [Créer ses propres mods](/fr/modding/)

## Des questions ?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
