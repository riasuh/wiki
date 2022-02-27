# 常见问题

## 我刚安装了游戏，该从哪儿看起？
来看看我们的[入门指南](/beginners-guide.md)！

## 如何导入自定义歌曲？
> 社区上传的歌曲都在 [BeatSaver](https://beatsaver.com)。 其他一些工具或者网站也提供了自定义歌曲的下载，但是这个网站是他们的数据来源。

如果你是从 BeatSaver 手动下载的歌曲包，请将它们解压成文件夹，放到 `Beat Saber/Beat Saber_Data/CustomLevels` 里。 游戏原生支持从这里读取自定义歌曲。

### BeastSaber
[Beast Saber](https://www.bsaber.com) 是另一个自定义歌曲网站，旨在管理和审核 BeatSaver 上所有歌曲。 您可以下载歌曲列表、关注作者、使用高级搜索等等。

### 歌曲管理工具

The following can be used to help you manage custom songs or playlists.

* [BeatList](https://github.com/ranmd9a/beatlist/releases/latest) is a desktop app to manage custom songs and playlists, maintained by **ranmd9a**.
* [BeaterList](https://syltaris.github.io/beaterlist) is a browser based service by **zexurge** to manage playlists.

## 如何安装歌曲列表？

### PC
您首先需要安装 [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod。

接下来：

* Use the `Install Playlist` tool in the Options tab of Mod Assistant.
* Place the playlist file into `Beat Saber/Playlists`, select the playlist title header in-game, then hit download all songs.

您应该在自定义歌曲的封面旁边看到歌曲列表。 模组还支持管理游戏中的歌曲列表。

### Quest
您可以使用 [Playlist editor Pro](https://beatsaberquest.com/bmbf/my-tools/playlist-editor-pro/) 来管理您 Quest 上的歌曲列表。 Note that a custom level can only appear once in-game due to a limitation with BMBF.

:::warning Quest 用户请注意 重新加载你的自定义歌曲文件夹后，会重置所有的歌曲列表顺序。 :::

## 如何制作自己的自定义歌曲？
查看 [地图](/mapping/)！

## 如何加载非 Mod Assistant 的 PC 模组？
见初学者指南中的 [这一节](/pc-modding.md#manual-installation)。

## Does multiplayer have crossplay?
Officially, multiplayer is limited to playing with other people in the store version (Oculus/Steam) you purchased. Additionally, modifying the game on Quest disables official multiplayer.

The BeatTogether mod is the current solution for cross-platform play between the modded game versions. Join their [Discord server](https://discord.com/invite/gezGrFG4tz) and check the `#install-instructions` channel for more information.

## 游戏更新导致Mod全部失效？
每次游戏更新时，旧版的 Mod *（很可能）*也需要更新。 To make sure your install will not break when the game runs on a new update for the first time, everything in the `Plugins` folder is automatically moved into a new folder called `Old 1.xx.x Plugins`. **Leave those plugins/mods in there!**

To get mods back, simply **run the installer again.**  
The BeatMods repository only includes mods that have been confirmed to work on the latest version of the game!

If you're confused by any of this, visit [Beginners Guide](/beginners-guide.md).

## Beat Saber 是如何计算得分的？ 全球排名是如何排名的？
我们在 [控制和技巧](/grips-and-tricks.md) 页面上详细介绍了评分和排名系统。

## 我的菜单是空白的，什么都没有？
如果游戏界面是空的，那么你的存档很可能被破坏了。

要修复这个问题，请到： `%AppData%\..\LocalLow\Hyperbolic Magnistism`

删除或重命名 Beat Saber 文件夹。 当重新进入游戏时，它会重新创建存档并加载主菜单。
