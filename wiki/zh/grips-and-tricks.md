---
sidebar: auto
---

# 握法和技巧
_一些整理过的资源可以帮您更好的击打方块。_

## 提升排名教程
由 TeknozFR 写的一篇非常好的教程帮助你获得PP分。 [排名和打分教程](./ranking-guide)

## 计分
观看这个由 [Cube Community YT](https://www.youtube.com/channel/UCdG9zS8jVcQIKl7plwWXUkg) 制作的视频了解计分系统是如何工作的。

<YouTube url='https://www.youtube.com/watch?v=rVbXCGddspA' />

另外，这张由游戏开发者提供的图片显示了[击打区域](https://twitter.com/Split82/status/979365834324889600)。

![方块击打区](~@images/mapping/hitbox-from-split.jpg)

## 排名
*全球排名是如何排名的？ 什么是PP (performance points)分？ 括号里的分数代表了什么？ 为什么我的PP分这么低？*

您可以在 [ScoreSaber](https://scoresaber.com/global) 搜索名字来查看全球排名和PP分。 您的 ScoreSaber 账户是关联到你的 Steam / Oculus 用户名的。

1. 排名曲是有一个PP分的 (PP = performance points 表现分)。 你完成排名曲所获得的PP分由准确度决定。 一首排名曲的PP分值是由我们的Panda God (Umbranox) 所开发的一套保密算法决定的。
2. 为了防止技术高的玩家刷分，简单的曲子的PP分较低。会有一条曲线根据游玩情况生成。 这条曲线的公式是 `0.965^(x-1)`，其中 `x` 代表了该分数在你的游玩情况中的位置。 例如，如果你所有曲目中获得的最佳记录是 260PP分，你将会获得 260PP分，也就是 原PP分(raw PP) 中的 100% (权重)。 如果你第二好的成绩的 原PP分 为247，那么根据曲线，你将会获得 238分的加权PP分。 下面你的表格可以展示系统如何计算的：

| 原PP   | 加权PP                    |
| ----- | ----------------------- |
| 260pp | **260pp** (100% 的原PP)   |
| 247pp | **238pp** (96.5% 的原PP)  |
| 246pp | **229pp** (93.1% 的原PP)  |
| 244pp | **219pp**  (89.9% 的原PP) |

3. 为了获得更高的排名，这里有几个工具可以让你找到适合你技术水平的评分曲。 首先，一个比较好的办法是，你可以到自己的 [ScoreSaber](https://scoresaber.com/global) 个人资料里看看你有段时间没玩过的歌曲。有哪些是可以打得更好的，然后你最好的分数大概是什么样的。 [ScoreSaberEnhanced](https://github.com/Splamy/ScoreSaberEnhanced#readme) 或者 [ScoreSaber Country Leaderboard](https://github.com/motzel/ScoreSaberCountryLeaderboard#readme) 浏览器插件可以给你的个人资料上增加些额外功能。 [BaliBilo's ScoreSaber 网站](https://scoresaber.balibalo.xyz/peepee) 和 [Beat Savior](https://www.beatsavior.io/) 是两个外部网站，它们可以帮助你找到谱面来提升并追踪你的表现。

你可以在 [排名和打分指南](./ranking-guide.md) 里找到更多信息。

*这一小结改编自 Tek 写在 Beat Saber Canadian discord 中的内容。*

::: tip 排名歌曲由 [ScoreSaber Discord](https://discord.gg/WpuDMwU) 审核。 你可以关注服务器看看有什么新变动！ :::

## 握法
Cube Community 制作了一些视频，展示了一些适用于 Oculus Touch 控制器 (CV1) 和 Vive 控制器 的比较热门的握法。

### HTC Vive 控制器
<YouTube url='https://www.youtube.com/watch?v=G7x_wb7RrgU' />

![Vive 握法指南](~@images/grips-and-tricks/vive-grips-guide.jpg)

### Oculus Rift
<YouTube url='https://www.youtube.com/watch?v=XFt90q69aEA' />

![Oculus 握法指南](~@images/grips-and-tricks/oculus-grips-guide.jpg)

### Oculus Rift S 和 Quest
暂时还没有适用于 Rift S 和 Quest 控制器的视频，但是你可以看看下面的一些示例！ ![Oculus Rift S/Quest 指南](~@images/grips-and-tricks/touch2-grips.jpg)

### Valve Index 控制器
暂时还没有适用于 Index 控制器的视频，但是你可以在 `#tips-and-grips` 频道里看到一些示例！ [CC Discord](https://discord.gg/dwe8mbC)

### Oculus Quest 2
暂时还没有适用于 Quest 2 控制器的视频，但是你可以看看下面的一些示例！ ![Oculus Quest 2](~@images/grips-and-tricks/touch3-grips.jpg)

看看 Cube Community [Discord服务器](https://discord.gg/dwe8mbC) 中的 `#tips-and-grips` 频道，里面有一些建议和示例。 请记住，每个人的游玩风格和身体情况是不同的。其他人的握法可能并不适合你。 多尝试体验，总会找到适合你的！

## 改进 Vive 控制器追踪
你的身体可能会阻挡 定位器 看见你其中的一个控制器。 这里有一些可能帮助你改进追踪的步骤。

1. 移动到游玩空间的角落里。
2. 旋转你的身体45°，这样你的 定位器 就可以看到你的两个控制器了。
3. 在节奏光剑的设置项里旋转房间使得你在游戏中也是正面向前。

![Vive 追踪帮助](~@images/grips-and-tricks/vive-tracking-help.gif)

这也适用于 Oculus 的传感器。

## Touch 控制器电池断连
你在玩节奏光剑的时候，挥动所使的力可能会让 Touch 控制器中的弹簧压缩导致短时断电。 这个情况发生时，你可以看到你的光剑没法追踪但是还在旋转。 为了减少这种情况的发生，ragesaq 建议在电池舱中加入额外的弹簧来减少电池断链情况的发生，详情请见这个 [Reddit 帖子](https://www.reddit.com/r/oculus/comments/a2h7o4/psa_adding_an_additional_spring_to_the_battery/?st=JR9Q7OEZ&sh=a7a3d091)。

## 也可以考虑
![也可以考虑](~@images/grips-and-tricks/allow-adequate-room-around-you-during-game-play-put-on-27689465.png)
