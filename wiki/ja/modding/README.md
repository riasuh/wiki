- - -
sidebar: auto description: Learn how to create your own mods!
- - -

# Modを作る

ビートセイバーはmodを_**サポートしていません**_。

Development for [PC](#pc-mod-development) and [Quest standalone](#quest-mod-development) are two vastly different workflows.

## PC Mod Development

### Modの導入
ほとんどのModは[BSIPA (Beat Saber Illusion Plugin Architecture)](https://github.com/nike4613/BeatSaber-IPA-Reloaded/)を利用してゲームにModを導入しています。そのほかのツールなどもこのソフトを利用しています。

[BepInEx](https://github.com/BepInEx/BepInEx)のほうが好ましいという方がいれば、BepisがBSIPA用の[ロードソフト](https://github.com/BepInEx/BepInEx.BSIPA.Loader)を作成しています。 ビートセイバーのプラグインをBepInEx plugin APIで開発するさいは、こちらの[ガイド](https://bepinex.github.io/bepinex_docs/v5.0/articles/dev_guide/plugin_tutorial/index.html)を参照してください。

### プロジェクトのセットアップ
ビートセイバーのModの作製に興味があるがVisual Studioなどで使うテンプレートを持っていない場合は[はじめのセットアップ](./pc-mod-dev-intro.md)に従ってください。

#### Ready to go?
Unityやそのほか関連するツールを以下の[リンク](#other-links)を参照してください。 If you have any questions, the best place to ask is in the `#pc-mod-dev` channel on the [BSMG Discord](https://discord.gg/beatsabermods)

### Launch args
Helpful launch arguments that will make modding / debugging easier.

<!-- markdownlint-disable MD013 -->
| Argument&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | Description                                                                                                                                                                                                           |
| -------------------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `--verbose`                                                                                  | Enables the output log window for IPA. This will show the debug console that mods use.                                                                                                                                |
| `fpfc`                                                                                       | "First Person Flying Controller"<br /><br />This allows you to use WASD and the mouse to navigate around the menu in game. This makes testing much easier, because you don't have to put on your headset! |
| `-vrmode oculus`                                                                             | If you are running Beat Saber through Steam, this allows you to play the game on an Oculus headset.                                                                                                                   |
<!-- markdownlint-enable MD013 -->

### Other Links

* [BeatMods](https://beatmods.com)
* [BeatMod承認ガイドライン（英語）](https://docs.google.com/document/d/15RBVesZdS-U94AvesJ2DJqcnAtgh9E2PZOcbjrQle5Y/edit?usp=sharing)
* [Unity Scripting API](https://docs.unity3d.com/ScriptReference/index.html)
* [dnSpy](https://github.com/0xd4d/dnSpy)
* [Harmony](https://github.com/pardeike/Harmony)
* [Beat Saber IPA](https://bsmg.github.io/BeatSaber-IPA-Reloaded/)

## Quest Mod Development

The following guide covers most of the concepts you will need for creating mods for the Quest. This includes but is not limited to:

* Hooking
* Configuration using `config-utils`
* Manual configuration
* User Interfaces using `questui` or `QUC`

Visit the [Quest Mod Development Intro](./quest-mod-dev-intro.md) page for more information on getting started!
