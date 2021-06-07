# Modを作る

## Modの導入
translation-done: false

ほとんどのModは[BSIPA (Beat Saber Illusion Plugin Architecture)](https://github.com/nike4613/BeatSaber-IPA-Reloaded/)を利用してゲームにModを導入しています。そのほかのツールなどもこのソフトを利用しています。

[BepInEx](https://github.com/BepInEx/BepInEx)のほうが好ましいという方がいれば、BepisがBSIPA用の[ロードソフト](https://github.com/BepInEx/BepInEx.BSIPA.Loader)を作成しています。 ビートセイバーのプラグインをBepInEx plugin APIで開発するさいは、こちらの[ガイド](https://bepinex.github.io/bepinex_docs/v5.0/articles/dev_guide/plugin_tutorial/index.html)を参照してください。

## プロジェクトのセットアップ
ビートセイバーのModの作製に興味があるがVisual Studioなどで使うテンプレートを持っていない場合は[はじめのセットアップ](./intro.md)に従ってください。

### 準備はいいですか?
Unityやそのほか関連するツールを以下の[リンク](#other-links)を参照してください。 質問があれば [BSMG Discord](https://discord.gg/beatsabermods)の`#pc-mod-dev`チャンネルでお尋ねください。

## 引数の設定
Modの導入とデバッグをより簡単にする便利な引数を設定します。

<!-- markdownlint-disable MD013 -->
| 引数&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | 説明                                                                                                                                                                                                                    |
| -------------------------------------------------------------------------------- |:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `--verbose`                                                                      | Enables the output log window for IPA. This will show the debug console that mods use.                                                                                                                                |
| `fpfc`                                                                           | "First Person Flying Controller"<br /><br />This allows you to use WASD and the mouse to navigate around the menu in game. This makes testing much easier, because you don't have to put on your headset! |
| `-vrmode oculus`                                                                 | If you are running Beat Saber through Steam, this allows you to play the game on an Oculus headset.                                                                                                                   |
<!-- markdownlint-enable MD013 -->

## Other Links

* [BeatMods](https://beatmods.com)
* [BeatMods Approval Guidelines](https://docs.google.com/document/d/15RBVesZdS-U94AvesJ2DJqcnAtgh9E2PZOcbjrQle5Y/edit?usp=sharing)
* [Unity Scripting API](https://docs.unity3d.com/ScriptReference/index.html)
* [dnSpy](https://github.com/0xd4d/dnSpy)
* [Harmony](https://github.com/pardeike/Harmony)
* [Beat Saber IPA](https://bsmg.github.io/BeatSaber-IPA-Reloaded/)
