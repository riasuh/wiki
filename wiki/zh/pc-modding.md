---
sidebar: auto
---

# PC 平台 Mod

## 前言

::: danger 免责声明 使用 Mod 前，你必须知道:

* 您可能会遇到在原版游戏中不存在的问题。 99.9%的bug、崩溃和延迟是由 mod 造成的。
* Mod 可能会因游戏更新而失效，这是正常的，在发生这种情况时不该抱怨，保持耐心和尊重， 因为 Mod 作者是完全自愿制作的。
* 游戏不是故意试图破坏模组。 游戏依赖于代码库运行，有时会破坏 Mod 的代码逻辑，但是他们不会杀掉 Mod 程序。

不要因为 Mod 相关的问题而骂游戏开发者，其实 Mod 作者和游戏开发者是两个独立的团体。 这样就太没素质了。 :::

:::warning 安装时注意 Beat Saber **从不** 要求你使用管理员权限运行。

如果您已经下载并安装了 Mod 并且看到获取用户权限控制的提示， **不要** 点击接受，然后反馈举报。 因为您安装的是恶意 Mod！

The only approved case is when activating/deactivating OneClick™ Install in Mod Assistant. Administrator access is required to register the program with your computer to handle OneClick™ Install links.

If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

Beat Saber natively supports custom songs, so if that's all you're looking for, you don't require more mods! It's a wise idea to install `SongCore` though, as this mod expands upon the base game functionality to improve loading times and provide functionality for other mods like the in-game downloader, custom leaderboards, playlists, etc.

::: warning This guide is for PC-modding on Windows.  
If you have a Quest, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux page](/modding/linux.md) or [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

If you run into problems at any point, please head to the [support page](./support) and see if you can identify what went wrong before asking in the Discord server. Chances are, your answer is on that page!

::: warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** suggest against using video tutorials for modding. Often, we find they are outdated or contain a incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Mod 安装器

### Mod Assistant
> **这是目前最推荐的 Mod 安装器**

__**Run the game at least once**** before trying to mod the game! This applies to reinstalling your game too.

A simple Beat Saber Mod Installer similar to the mod manager, but with additional features such as mod removal and version checking! Get it on [Assistant's GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## 在哪里下载更多歌曲
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

::: warning It is a good idea to backup your `CustomLevels` folder periodically as there is a small chance it will be reset if the game updates!

This folder is located in your game install: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### 游戏内下载器
The `BeatSaver Downloader` mod allows you to download maps in-game using the `MORE SONGS` menu button on the `MODS` menu screen. This pulls maps directly from [BeatSaver](https://beatsaver.com)

### Beatsaver
[BeatSaver](https://beatsaver.com) is the master repository of custom songs made by the community. Many other tools and sites enhance the experience of downloading custom songs, but this site is where they are stored. To install songs downloaded from the site, unzip them into a folder and place it into `Beat Saber/Beat Saber_Data/CustomLevels`. You can also use the in-game downloader mod, or Mod Assistant's OneClick™ Install feature.

To enable and use Mod Assistant's OneClick™ Install see the picture below: ![Mod Assistant](~@images/beginners-guide/modassistant-oneclick.png)

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) is a site that tries to help make finding fantastic maps to play easier. It does this by categorizing the thousands of songs on BeatSaver and lets you sort by a song's genre and many other attribute tags. It also has a full social feature where players can review songs and comment on them. One of the most used features is the "Curator Recommended" feature where a team plays through most songs released each day and recommends the ones that stand out, letting you [automatically download these in-game](https://bsaber.com/beatsync/).

### 歌曲管理工具

There are no working song management apps available at this time.

### 歌曲列表
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* 点击 `Install Playlist（安装歌曲列表）`。
* 或者手动将歌曲列表文件放入 `Saber/Plists`中，然后在游戏里选择播歌曲列表的标题，点击下载所有歌曲。

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

## 安装目录
_Where is Beat Saber installed?_

### 默认位置
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### 其他位置
**If you have moved your install folder to a different drive, it might be in the location below.** Replace the drive letter `F` with the drive your game is installed on.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## 手动安装
A mod installer is the recommended way to install mods. See the section [above](#installers). If you have patched the game and just need to install mods that are not available in the installer, skip to step 4.

::: warning STAY SAFE WHEN INSTALLING MODS Modding your game with unverified mods such as mods found in the `#pc-mods` channel comes with risks, including the possibility for malicious software that acts like a regular mod.

Beat Saber will **NEVER** ask you to run it as Administrator.

If you've downloaded and installed a mod and you get the User Account Control prompt, **DO NOT** click accept, and please report this. If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

**Run the game at least once** before trying to mod the game! This applies to reinstalling your game too.

### 安装 BSIPA

1. 下载 [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases)。
2. Navigate to your [install folder.](#install-folder) and extract the contents of BSIPA into it. ![Directory Clean](~@images/beginners-guide/directory-clean.png "Directory Clean") ![Directory Ipa](~@images/beginners-guide/directory-ipa.png "Directory Ipa")
3. Double click IPA.exe to patch the game. Any mods in the `Plugins` folder will now be loaded when starting the game. If there are errors, you probably didn't follow step 2 correctly. ![Directory Patched](~@images/beginners-guide/directory-patched.png "Directory Patched")

### Install Mods

4. Download the mod(s) you wish to install, whether it be from GitHub, the [BSMG Discord](https://discord.com/invite/beatsabermods) `#pc-mods` channel,  [BeatMods](https://beatmods.com/#/mods) or other sources. **Make sure to download any dependencies required by the mod.** ![Directory Plugins](~@images/beginners-guide/directory-plugins.png "Directory Plugins")
5. Some mods have installation instructions, some don't. Generally you can just drag and drop the zip contents into your beat saber install folder, and the files should go into the corresponding folders.

## 如何卸载 Mod
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## 接下来

* [Grips and Tricks](./grips-and-tricks.md)
* [制作谱面](/mapping/)
* [自定义光剑](/models/custom-sabers.md)
* [自定义人物模型](/models/custom-avatars.md)
* [自定义平台](/models/custom-platforms.md)
* [在多人游戏中玩自定义歌曲](https://discord.com/invite/gezGrFG4tz)
* [制作 Mod](/modding/)

## 还有其他问题吗？
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
