---
sidebar: auto
---

# PC端Mod

## 前言

::: danger 免责声明 在使用 Mod 前，你必须知道:

* 您可能会遇到在原版游戏中不存在的问题。 99.9%的bug、崩溃和卡顿是由 Mod 造成的。
* Mod 可能会因游戏更新而无法使用，这很正常。发生这种情况时，你应该耐心等待并尊重用爱发电的Mod作者们。
* 游戏开发商Beat Games没有故意阻止使用Mod。 开发商更新游戏会对游戏代码作出改动，这有时会让Mod无法使用，但并不是有意阻止玩家使用Mod。

不要因为 Mod 相关的问题而攻击游戏开发者，因为 Mod 作者和游戏开发者是两个独立的团体。 心胸大度一点。 :::

:::warning 安装时注意 节奏光剑 **从不** 要求您使用管理员权限运行。

如果您已经下载并安装了 Mod 并且看到获取用户权限控制的提示， **不要** 点击接受，然后反馈举报。 因为您安装的是恶意 Mod！

请只在激活/禁用 Mod Assistant 中的 OneClick™一键安装 功能时同意使用管理员权限。 程序在关联 OneClick™一键安装 链接时需要管理员权限。

如果你不确定你是否安装了恶意Mod，***请向我们的Discord社区求助***。 :::

节奏光剑原生支持自定义歌曲，如果你只是想要这个功能的话并不需要安装Mod！ 安装 `SongCore (歌曲核心)` Mod是不错的选择，因为这个 Mod 不仅为原生游戏增加了一些额外功能并降低了加载时间，还作为游戏内下载 (in-game downloader)，自定义排行榜 (custom leaderboards)，歌曲列表 (playlists) 等 Mod 的依赖项。

::: warning 该指南只针对Windows上的PC端Mod。  
如果你有Quest设备，请见 [Quest 端 Mod 页](/quest-modding.md)。  
如果你使用Linux系统，请见 [Linux 页](/modding/linux.md) 或[Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

如果你在任何时候遇到困难，在Discord社区提问前可以试试在 [支持页](./support) 看看是否可以自行解决一些问题， 很有可能你遇到的问题就在那页里！

::: warning 我在YouTube上看了教程视频，但是还是没法运行。 这些视频教了您什么？ 我们 BSMG **非常** 反对使用 Mod 视频教程。 我们经常发现过时的，不完整的，误导性的或者不正确的信息。

相反，你应该参考我们在Wiki上的指南或者在 [BSMG Discord 社区](https://discord.gg/beatsabermods) 中寻求帮助。 :::

## 安装器

### Mod Assistant
> **这是目前最推荐的 Mod 安装器**

在安装 Mod 之前，__**至少运行一次游戏****。 当你在重装游戏时也需要这么做。

这是一个操作简单的节奏光剑 Mod 安装器。它类似于 Mod 管理器，但是有例如移除 Mod 或者版本检查等额外功能！ 前往 [Assistant 的 GitHub](https://github.com/Assistant/ModAssistant/releases/latest) 下载

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## 如何获取更多歌曲
::: tip
在"热门 (Top All)"，"评分 (Rating)"，"下载量 (Downloads)" 或 "游玩数 (Plays)" 排序中出现的很多谱面都是在优秀制谱共识建立之前发布的。 尝试下载2019后半年至今的自定义关卡以获得最好的体验。
:::

::: warning 建议您定期备份 `CustomLevels` 文件夹，因为游戏更新时会有较小的可能会清空文件夹！

该文件夹位于您的游戏安装目录: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### 游戏内下载
`BeatSaver 下载器 (BeatSaver Downloader)` Mod 可以让你在游戏中的`MODS`面板中使用 `更多歌曲 (MORE SONGS)` 按钮下载歌曲。 它会直接从 [BeatSaver](https://beatsaver.com) 下载歌曲

### Beatsaver
[BeatSaver](https://beatsaver.com) 是玩家社区建立的自定义歌曲主仓库。 很多其他的工具或者网站提供了更多下载自定义歌曲的功能，但是这个网站就是这些歌曲存储的地方。 从网站上下载的歌曲需要解压缩到 `Beat Saber/Beat Saber_Data/CustomLevels`文件夹。 你也可以使用游戏内下载 Mod或者 Mod Assistant 的 OneClick™一键安装 功能。

下图展示了如何开启并使用 Mod Assistant 中的 OneClick™ 一键安装功能： ![Mod Assistant](~@images/beginners-guide/modassistant-oneclick.png)

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) 是一个旨在帮助玩家更容易找到并游玩优质谱面的网站。 它分类了 BeatSaver 上成千上万的谱面，并让你可以根据歌曲的流派和其他标签来挑选歌曲。 它还提供了完整的社交功能，让玩家可以查看以及评论。 其中一个最常用的功能是“小编推荐”，团队每天会游玩最新发布的歌曲并且会推荐其中最好的，让你可以在 [游戏中自动下载](https://bsaber.com/beatsync/)。

### 歌曲管理工具

现在暂时还没有可用的歌曲管理工具。

### 歌曲列表
你需要安装 [歌曲列表管理器 (PlaylistManager)](https://github.com/rithik-b/PlaylistManager/releases/latest) Mod。

然后你可以：

* 在 Mod Assistant 中找到 "设置 Options" 标签页，勾选 `安装歌曲列表 (Install Playlist)`。
* 或者手动将歌曲列表文件放入 `Beat Saber/Playlists `中，然后在游戏里选择播歌曲列表，点击下载所有歌曲。

你应该可以在游戏内的自定义歌曲专辑旁看到播放列表图标。 这个 Mod 也支持在游戏中管理播放列表。

## 安装目录
_节奏光剑安装在哪里？_

### 默认位置
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### 其他位置
**如果你把安装目录移动到其他盘，安装位置可能在下面的地方。** 将盘符 `F` 改为你游戏安装的位置。
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## 手动安装
Mod 安装器是安装 Mod 的推荐方式。 建议查看 [上面](#installers) 的部分。 如果你已经给游戏打了补丁并且想要安装在安装器中没有的 Mod的话，请跳至第 4 步。

::: warning 安装 Mod 时要注意 安装未认证的 Mod，例如在 `#pc-mods` 频道中发布的Mod，可能会有风险。其中可能还会有伪装成正常Mod的恶意软件。

节奏光剑 **从不** 要求您使用管理员权限运行。

如果您已经下载并安装了 Mod 并且看到获取用户权限控制的提示， **不要** 点击接受，然后反馈举报。 如果你不确定你是否安装了恶意Mod，***请向我们的Discord社区求助***。 :::

在安装 Mod 之前，**至少运行一次游戏**。 当你在重装游戏时也需要这么做。

### 安装 BSIPA

1. 下载 [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases)。
2. 解压文件到你的 [安装目录](#install-folder) 。 ![清空的目录](~@images/beginners-guide/directory-clean.png "清空的目录") ![Ipa 目录](~@images/beginners-guide/directory-ipa.png "Ipa 目录")
3. 双击 IPA.exe 来给游戏打补丁。 所有 `Plugins` 文件夹中的 Mod 将会在游戏启动时加载。 如果发生错误，你可能没有正确的执行第 2 步。 ![打补丁的目录](~@images/beginners-guide/directory-patched.png "打补丁的目录")

### 安装 Mod

4. 下载你想要安装的 Mod，不论是从GitHub，[BSMG Discord](https://discord.com/invite/beatsabermods) 里的 `#pc-mods` 频道，[BeatMods](https://beatmods.com/#/mods) 或者其他来源。 **请确保该 Mod 所需的所有依赖项也一并安装。** ![插件目录](~@images/beginners-guide/directory-plugins.png "插件目录")
5. 一些 Mod 会有安装说明，一些则没有。 一般来说，你可以直接把压缩文件里的文件拖到节奏光剑的安装目录，这些文件应该会放入对应文件夹。

## 降级游戏

去 [BSMG](https://www.discord.gg/beatsabermods) 服务器中的 `#modding-notifications` 频道 查看最新版本是否可以安装 Mod。 如果不能安装 Mod的话，你可以按照下列的教程降级游戏至可以安装 Mod 的游戏版本。

根据你游戏所在平台去下面这些链接里查看教程。

* [Oculus 商店](https://computerelite.github.io/tools/Oculus/OculusDowngraderGuide.html)
* 对于Steam平台来说你有几个方法可以降级游戏。 以下两个方法是 [BSLG](https://discord.gg/MrwMx5e) 提供支持的。
  * [BS传统启动器 (BSLegacyLauncher)](https://www.youtube.com/watch?v=qjNU5aENHRU)
  * [传统安装器 (LegacyInstaller)](https://github.com/Goobwabber/LegacyInstaller#readme)

## 如何卸载 Mod
你可以从 `Plugins` 文件夹中删除 dll 文件，或者在 Mod Assistant 中点击 `卸载 (Uninstall)` 按钮。

## 接下来你还可以看看

* [握法和技巧](./grips-and-tricks.md)
* [如何制作谱面](/mapping/)
* [自定义光剑](/models/custom-sabers.md)
* [自定义虚拟形象](/models/custom-avatars.md)
* [自定义场景](/models/custom-platforms.md)
* [多人游玩自定义歌曲](https://discord.com/invite/gezGrFG4tz)
* [制作 Mod](/modding/)

## 还有其他问题吗？
访问 [BSMG Discord 支持频道](https://discord.gg/beatsabermods)！
