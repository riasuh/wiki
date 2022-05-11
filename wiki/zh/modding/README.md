# 制作 Mod

## 注入 Mod
节奏光剑原生 _**不支持**_ Mod。

所以，大多数在Mod安装器中的Mod依赖于 [BSIPA (节奏光剑幻象插件架构 Beat Saber Illusion Plugin Architecture) ](https://github.com/nike4613/BeatSaber-IPA-Reloaded/)来将插件注入游戏，同时也提供了一些对Mod作者有用的工具。

对于那些想要使用 [BepInEx](https://github.com/BepInEx/BepInEx) 的人来说，Bepis 制作了一个 BSIPA 插件加载器，可以在 [这里](https://github.com/BepInEx/BepInEx.BSIPA.Loader) 查看。 对于使用 BepInEx 插件 API 开发节奏光剑插件的开发者，在他们的 [文档页](https://bepinex.github.io/bepinex_docs/v5.0/articles/dev_guide/plugin_tutorial/index.html) 上有一个通用指南，但是其他的部分你得自己解决了。

## 项目设置
如果你对制作节奏光剑 Mod有兴趣的话，但是没有模板或者Visual Studio 模板设置的话，可以 [跟着入门指南来设置好你的项目](./intro.md)。

### 准备好了？
看看 [下面的链接](#other-links) 获取 Unity 和其他相关工具的文档。 如果你有任何问题，最好在 [BSMG Discord](https://discord.gg/beatsabermods) 的 `#pc-mod-dev` 频道问问。

## 启动参数
好用的启动参数可以帮助你制作/调试 Mod更加简单。

<!-- markdownlint-disable MD013 -->
| 参数&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | 描述                                                                                                                        |
| -------------------------------------------------------------------------------------- |:------------------------------------------------------------------------------------------------------------------------- |
| `--verbose`                                                                            | 启用IPA的日志输出窗口。 这会显示Mod使用的调试控制台。                                                                                            |
| `fpfc`                                                                                 | “第一人称无需控制器 (First Person Flying Controller)”<br /><br />这允许你可以使用 WASD 键和鼠标在游戏中调整视角和控制。 这让你测试更加的方便，因为你不需要带着头显！ |
| `-vrmode oculus`                                                                       | 如果你是用Steam运行节奏光剑，这可以让你可以在Oculus 头显上运行游戏。                                                                                  |
<!-- markdownlint-enable MD013 -->

## 其他链接

* [BeatMods](https://beatmods.com)
* [BeatMods 审核准则](https://docs.google.com/document/d/15RBVesZdS-U94AvesJ2DJqcnAtgh9E2PZOcbjrQle5Y/edit?usp=sharing)
* [Unity 脚本 API](https://docs.unity3d.com/ScriptReference/index.html)
* [dnSpy](https://github.com/0xd4d/dnSpy)
* [Harmony](https://github.com/pardeike/Harmony)
* [Beat Saber IPA](https://bsmg.github.io/BeatSaber-IPA-Reloaded/)
