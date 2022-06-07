---
sidebar: "false"
tags:
  - bsmg
  - beat saber
  - wiki
  - 譜面作成
  - 譜面作成
  - ビートセイバーの譜面の作り方
  - カスタムレベル
  - カスタムマップを作成
  - カスタム チャート
description: |
  譜面にアニメーションが多すぎますか？ 十分なアニメマップがありませんか？
  あなた自身がその問題を解決するための方法を学びましょう
---

# マッピング

譜面にアニメーションが多すぎますか？ 十分なアニメーションのある譜面がありませんか？ここで譜面を作る方法を学び自分でその問題を解決しましょう！

::: tip INFO  
もしよりよい譜面作成のリソースを提供するためのフィードバックがありましたら [フォーム](https://docs.google.com/forms/d/e/1FAIpQLSfVS6_EMZOujxthR3lTa2eEwHg5C3x1INouLgnbHhBDpv1M5A/viewform)に記入をお願いします

`#mapping-discussions` の [Beat Saber Modding Group Discord](https://discord.gg/beatsabermods) にアクセスして参加することもできます！ :::

* [譜面作成の用語](./glossary.md)

## クイックスタート
> wikiはあなたの構築ブロックであり、コミュニティはあなたのインスピレーションであり、あなたは創造性です。

偉大な譜面作者には一日でなれるものではありません。 だれもあなたに追いつけなくなるようになるには努力が必要です。 私ができる最大限のことはあなたにこのwikiを提供し、あなたが譜面作成を成功させるためのすべての疑問を明確に解決します。

1. 譜面作成に必要なツールをダウンロードします。[オーディオエディタ](https://www.audacityteam.org/)や[マップエディタ](#map-editing-resources)です。
2. [オーディオファイル](#audio-editing-resources)を設定し、BPMを設定して確認し、OGG形式でエクスポートします。
3. [マッピングエディター](#map-editing-resources) で曲を設定します (ステップはエディターによって異なります)。
4. 譜面を作りましょう！ 始める前に [基本的なマッピングの実践](./basic-mapping.md) を確認してください。 早めに、そして譜面作成途中などに[テストプレイ](#playtesting)してください。
5. 照明を作りましょう！ [基本的な照明](#lighting-practices) を参照してください。 シンプルな照明は意外と簡単です!
6. [テストプレイ](#playtesting)しましょう！ [BSMG Discord](https://discord.gg/beatsabermods) を介したサードパーティのプレイテストは、建設的なフィードバックを得たり、自分では得られない気付きを得られたりします。
7. 譜面が作成され、照明効果も設定され、テストプレイされたら、 [](#publishing-songs) あなたの曲を BeatSaver で世界にリリースする準備は万端です。

### ビデオチュートリアル
テキストガイドはあなたの好みではありませんか これらのビデオをチェックしてみてください。  
:::tip Remember: テキストガイドはより簡単に迅速に変えることが可能なので、いつでも最新の情報が記載されています。 :::

#### おすすめ

* [Helen Carnateのマッピングチュートリアル](https://www.youtube.com/watch?v=6O3sXmh-kAA) - マッピングを開始するための17分のガイド!
* [Fruheadの初心者向けマッピングガイド](https://www.youtube.com/playlist?list=PL5F3WJ0s0nscdpqiWlOpM_4tJcF-CnWbm) - 初めての譜面作成に関する包括的なレクチャーシリーズ。
* [ChroMapper Editor Guide](https://youtube.com/playlist?list=PLS0PknCDCujE3Tf1pkbkA_uUijkV6v52y) - ChroMapper Editor の主な機能の使用方法に関するビデオ。
* [初心者として回避すべきCyrixのパターン](https://www.youtube.com/watch?v=mgGaqZ20Scw) - [Basic Mapping](./basic-mapping.md) で議論されている最も一般的な問題をカバーします。
* [TransquillizeMe's Beat Saber Lighting Techniques チュートリアル](https://www.youtube.com/watch?v=EDbPRN_u3jc) - さまざまな照明効果と一般的な照明のヒントをカバーします。

:::warning このページのチュートリアルは BSMG によって調査されています。 他のビデオチュートリアルは、最新の情報でなかったり、正確でない可能性があります。それらのビデオを見る場合はご自身でそのリスクを理解する必要があります。

あなたのチュートリアルをこのリストに入れたい場合は、 [こちらからお問い合わせください](https://bsmg.dev/contact) :::

#### レガシービデオ
::: warning チュートリアルでは古いエディタ(Mediocre Mapper and EditSaber) を使用しています。 UIといくつかのプロセスは、最新の推奨エディタ [MMA2](./mediocre-map-assistant.md) で変更されましたが、コンテンツは素晴らしいです! :::

* [BennyDaBeastのマッピングチュートリアル](https://bsaber.com/benny-custom-mapping/)
* [Freek のマッピングとエディターチュートリアル](https://www.youtube.com/playlist?list=PLYeZR6d3zDPgDgWogOwMteL-5SQWAE14b)

## オーディオ編集
譜面を作成する前に、譜面作成エディターで読み込むことができる音源を準備する必要があります。 このセクションでは音源の準備や編集を行うことができるフリーソフト[Audacity](https://www.audacityteam.org/)のセットアップを解説します。

### [**基本的なオーディオ設定**](./basic-audio.md)
音源なしで譜面を作成することは不可能です。 簡単に譜面作成を行うための音源準備の方法を学びましょう

### [**高度なオーディオ設定**](./advanced-audio.md)
音源のショートバージョンを作成したり、BPMの変更するなど詳細な音響の調整方法について説明します。

## 譜面作成用資料

### コミュニティのエディタ
::: warning
標準のエディタはたくさん機能がありVRを必要としません。しかしバグが起きる可能性があり、注意が必要です。
::: これらのエディタのキーボードショートカットの一覧は[こちらから](./editor-keybinds.md)利用できます。

#### ChroMapper
**オープンベータ公開！** 主に照明効果に特化されており、Chroma、Noodle Extensionsや360/90譜面がサポートされた3Dマッピングツールです。Beat Saber内のアセットが用意されているのでより詳細なプレビューを見ることができます。 FAR では、コミュニティで利用可能なエディターで最も機能が豊富です。

[ChroMapper Discord](https://discord.gg/wFjZt4z) に参加することをお勧めします。プラグイン、スクリプト、アプリケーション へのアクセスをお勧めします(マッピングサポートは BSMG で利用できます)。

* [ChroMapperランチャーのダウンロード](https://cm.topc.at/dl)
* [ChroMapper 初回セットアップガイド](https://chromapper.atlassian.net/wiki/spaces/UG/pages/917506/First-time+setup)
* [ChroMapper Wiki](https://chromapper.atlassian.net/wiki/spaces/UG/overview)

#### Mediocre Map Assistant 2
MMA2 は、ChroMapper のベータ版が完成するまでマッピングコミュニティの大半が使用していました。

* [Mediocre Map Assistant 2のダウンロード](https://git.bsmg.wiki/Top_Cat/MediocreMapAssistant2/releases/latest)
* [Mediocre Map Assistant 2のガイド](./mediocre-map-assistant.md)

#### Beatmapper.app
ブラウザ上で起動する３Dマップエディターは誰でもマッピングができます。 拡張機能がない標準的な機能ですが、いくつか新しい機能が追加されています。

* [Beatmapper ウェブサイト](https://beatmapper.app/)
* [Beatmapper ユーザーマニュアル](https://beatmapper.app/docs/manual/getting-started)

::: tip 自分のエディタやコンバーターを作ることに興味がありますか? [マップフォーマットページ](./map-format.md) と [SongCore Readme](https://github.com/Kylemc1413/SongCore/blob/master/README.md) が役に立ちます！ :::

### 公式版エディター
公式のエディタはBeat Games によって開発されており、Steam VRとOculus PC版であらかじめインストールされています。

:::tip Info Coming Soon
Check back later for information on the new 3D official editor that supports the new note types and lighting system!
:::

#### 公式エディターからコミュニティエディターへの移行
:::warning NOTE
These instructions are for the old 2D editor that was retired since Beat Saber version 1.8.0
:::

Although it is recommended to start setup again following the [Quick Start](#mapping-quick-start) guides with a [Community Editor](#community-editors), it is possible to transfer your work in the Official Editor over.

1. [コミュニティエディタ](#community-editors)をインストールします。
2. `CustomLevels`にあなたの譜面を入れます。
    * Steamの場合 ファイルの場所: `C:\Program Files (x86)\Steam\steamaps\common\Beat Saber\Beat Saber_Data_CustomLevels`
    * Oculusの場合 ファイルの場所: `C:\Program Files\Oculus\Software\hyperbolic-magnetism-beat-saber\Beat Saber_Data\CustomLevels`
3. エディタが探せる場所にファイルを移動します。 普通`Beat Saber_Data`の`CustomWIPLevels`ファイルのことを指します。
    * Steamの場合 ファイルの場所: `C:\Program Files (x86)\Steam\steamaps\common\Beat Saber\CustomWIPLevels`
    * Oculusの場合 ファイルの場所: `C:\Program Files\Oculus\Software\hyperbolic-magnetism-beat-saber\Beat Saber_Data\CustomWIPLevels`
4. オーディオファイルを `.wav` から `.ogg` 形式に変換します。
    1. [Audacity](https://www.audacityteam.org/) をダウンロードしてインストールする
    2. Audacity で `.wav` ファイルを開く
    2. `File メニュー -> Export -> Export as OGG`
    3. ファイルに`song.ogg` と名前を付け、 <kbd>Save</kbd> をクリックします。
    4. 譜面フォルダに `song.ogg` ファイルを入れます。
        * フォルダに `.wav`ファイルは不要です。
5. コミュニティエディターでマップを開き、曲ファイル名を `song.ogg` に変更し、保存ボタンをクリックします。

You are now ready to continue editing your map!

### データ損失防止とクラウドストレージ
Updating your game may remove all Custom Level data, one way you can prevent complete data loss is with [Symbolic Links!](https://en.wikipedia.org/wiki/Symbolic_link) This allows you to store your maps in a different place on your computer, such as a folder synchronized to the cloud, and mirror them in the game directory. The link created will not delete your maps if it is removed due to updating or uninstalling the game however, recursive deletion will remove your maps.

Using a cloud storage folder is useful if you jump between multiple computers or extra security for your files in case of storage disk corruption.

The following instructions are for Windows 10 and 11.

1. 現在のレベルフォルダを新しい場所に移動します。 (`Ctrl + c` の代わりに `Ctrl + x`)
   * これがクラウド上のファイルである場合は、オフラインで利用できるようにフォルダを設定してください!
2. コマンドプロンプトを開く
3. 場合によってはパラメータを調整するコマンドを実行します。  
     
   `mklink /j "Path to Beat Saber Install folder" "Path to New Location"`
    * Heres an example command:  
      `mklink /j "C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\Beat Saber_Data\CustomLevels" "C:\Users\cmb\CloudStorage\CustomLevels"`

If it's on a network drive, replace `/j` with `/D`. Note that you will need to open command prompt as administrator for this to succeed.

### 追加のマッピングツール

* [BS Viewer](https://skystudioapps.com/bs-viewer/) by **+1 Rabbit**  
  A convenient way to see how your map might look in game without the game.
* [+1 Rabbit's Mapping Tools](https://skystudioapps.com/mapping-tools/) by **+1 Rabbit**  
  A suite of tools for mappers that includes:
  * **Schema Fixer:** Easily fix maps made in Mediocre Mapper Mk4.1 and Mk5 for upload to BeatSaver.
  * **Tempo Changer:** Change the BPM of an entire map and shift block placements accordingly.
  * **Offset Remover:** Removes editor offset and snaps notes/obstacles/events to common precisions to try and mitigate floating point error.
  * **Note Sorter:** Sorts unordered notes/obstacles/events in the map file to fix stack spawning.
  * **Copy Timing:** Moves notes in one difficulty based on another within a certain window. Useful to apply small timing changes across all difficulties for specific sounds.
  * **Copy Lighting:** Copies all of the lights, with the option to include/exclude custom events from one difficulty to all other difficulties.
  * **Map Diff:** Compare between two versions of a map. Useful for testplayers and Ranking Team members to see if any changes were made.
* [Parity Checker](https://galaxymaster2.github.io/bs-parity/) by **GalaxyMaster**  
  An error checker tool that focuses on finding issues with parity in a map.
* [Map Check](https://kivalevan.github.io/BeatSaber-MapCheck/) by **Kival Evan**  
  An error checker tool that is much more versatile than the one built into MMA2.
* [noodleLister](https://github.com/bloodcloak/noodleLister#readme) by **Bloodcloak**  
  Easily compile a game playlist from a txt file containing BeatSaver map keys.

#### レガシーツール
These tools may no longer be supported, compatible with the latest software, or relevant with current practices, but could still fulfill a niche use case.

* [BeatMerge](https://github.com/ZelonGames/BeatMerge#readme) by **DarkGrisen**  
  Ever thought that it is a lot of annoying work to make big maps with other people or to perfectly cut the audio files so you can merge them manually later? This tool allows you to merge two or more maps into one single super long map.
* [Cinder](https://github.com/zhaey/cinder#readme) by **zhaey**  
  Python program that converts stepmania `.sm` files to Beat Saber `.dat` files for timing notes.
* [BeatMapper Tools](https://beatmappertools.com/) by **Darkuni**  
  A utility for users of Mediocre Mapper and Mediocre Map Assistant 2 to easily convert, test, and package their maps.
* [osu! Editor Timing Tutorial](https://www.youtube.com/watch?v=nIX0koHzW8c&t) by **Fayhe**  
  Video guide on using the timing feature of osu!'s editor to find map bpm.

### 便利なMod
Here are some mods that might make your mapping workflow a little easier.

* [SiraUtil](./basic-lighting.md#in-game-with-fpfc) by **auros**  
  With the First Person Flying Controller (FPFC) launch parameter, this allows you to control the game while a map is playing with your keyboard and mouse without using a headset. See the section in [Basic Lighting](./basic-lighting.md#in-game-with-fpfc) for links to the mods and how to set it up.
* [PracticePlugin](https://github.com/Kylemc1413/PracticePlugin) by **Kyle1413**  
  Mod for Beat Saber to control playback speed, seek through songs and set up looping sections. Install the latest version from [Mod Assistant](https://github.com/Assistant/ModAssistant#readme)!
* [ReLoader](https://github.com/Kylemc1413/ReLoader) by **Kyle1413**  
  Allows you to hot reload beatmaps in practice mode without needing to return to the menu to refresh. Really convenient for wall mapping.

## マッピングの練習
> "ルールを破るには、まずそれを熟知しなければならない。"  
> \- Uninstaller

There is no holy bible of mapping but this section of the wiki includes a lot of tribal knowledge from the community on best practices at all levels of mapping. Our advice is to follow these rules until you're comfortable with your skills and then get creative, experiment, and innovate!

### [**基本的なマッピング**](./basic-mapping.md)
All new mappers need to read this, **no exceptions!**

### [**中級者向けの譜面作成ガイド**](./intermediate-mapping.md)
A more in-depth look at many mapping topics

### [**ダウンマッピング**](./downmapping.md)
A comprehensive guide to making lower difficulties.

### [**上級者向け譜面作成**](./extended-mapping.md)
Mapping Extensions, Extra Characteristics, and 360&deg;/90&deg; mapping

### Mapperのロール
To apply for the **Mapper** role on the [Beat Saber Modding Group Discord](https://discord.gg/beatsabermods) you must have released three solid/playable maps (collaborations are acceptable) and complete the [Mapper Role Submission Form](https://forms.gle/mj66J3UopTykFJjXA). Your application and maps may take a decent amount of time to be reviewed and approved.

### キュレーション
Mappers can submit high quality maps, free of [objective issues](https://bsaber.com/getting-started/curation/#donts) to the #curation-request channel on the [BeastSaber Discord](https://discord.gg/VJZHUbt). Maps selected for curation are given extra visibility on the site and included in the Curator Recommended feed.

### Modding & ランキング
Maps that meet specific [Ranking Criteria](https://scoresaber.com/criteria) and go through an intensive review process called "modding" have the potential to become ranked, awarding players Performance Points (PP) toward global leaderboards. More information and an in-depth FAQ is available on the [ScoreSaber Discord](https://discord.gg/WpuDMwU)

* Prior to requesting ranking, mappers should thoroughly review the ranking criteria and [metadata standards](https://docs.google.com/document/d/1ehotupIYMVlc8x41JldO-24m7Am-oTVYnciF9KCRdNM/edit) and have their map modded by a knowledgeable source.

:::tip Want an even more detailed look? Review the [Ranking Criteria](https://scoresaber.com/criteria) for some of the more ambiguous ranking considerations. :::

* Once your map has been modded and revised, it’s ready to be presented to a ranking team member or recruit to review.
* If the ranking team member deems the map acceptable it will be added to the ranking request queue to be voted on by the full ranking team.

### マッピングに不安を感じる
If you're finding it difficult to muster up the courage to upload your map, or are finding it emotionally taxing coping with a lack of downloads or a lot of dislikes, you're not alone. Many mappers have experienced these feelings. You can read more about it on the [Coping with Mapping Anxiety](./mapping-anxiety.md) page.

## 照明効果
A map is not finished until some form of lighting is included. Lighting can range from very basic to incredibly detailed using additional mods to enable more features.

### [**基本的な照明効果**](./basic-lighting.md)
Learn the various aspects to lighting your map manually

### [**中級者向けライティング**](./intermediate-lighting.md)
Take your lighting skills a bit further into strobing, ring spins, and contrast practices

### [**高度なライティング**](./advanced-lighting.md)
Advanced and nuanced techniques, lighting for custom platforms, and Chroma RGB **(This page is still a work in progress!)**

### オートライティング
Not ready to make your own lighting? Here are some programs to do it for you. Keep in mind, creating simple manual lighting is not difficult and will always be better at expressing the atmosphere of the song than using these programs.

* [Lolighter](https://github.com/Loloppe/Lolighter#readme) by **Loloppe#6435** - Standalone program for automated lighting and has other features to modify your map.
* [LiteMapper](https://litemapper.net/) by **ItsOrius** - A website that automatically generates lights based on pacing, emphasis, and note placement. For more information on the algorithm check out the [Readme](https://github.com/ItsOrius/LiteMapper#readme).
* **Lightmap** - It is integrated into Mediocre Map Assistant 2 and can be accessed in the error checker menu.

## テストプレイ
Testing your work is a **critical** part of mapping. Testing as you work helps you adjust for major playability issues and get a feel for your map. [Third-party or "outside"](#community-third-party-testing) playtesting is when someone other than yourself tests your pre-release map and provides constructive feedback and is helpful in highlighting issues to which you may be "map blind."

::: danger You **DO NOT** need to upload your map to BeatSaver in order for you or anyone else to test. :::

* If your map is using the 1.0 song format (your files are .json and .ogg) you must convert your map by **updating your editor**, opening and saving the map. See [Community Editors](.#community-editors) for links to modern editors.
* If your map is using the 2.0 song format (your files are .dat and .ogg/.egg) you’re ready to test.

### PCでテスト
Follow these steps to test any of your maps made with a community editor using PC-based VR.

1. WIPソングフォルダが `Beat Saber_Data_CustomWIPLevels` にない場合は、そこにマップのコピーを置きます。
2. ゲーム内のプレイリスト一覧からCustomWIPLevelsに行きます。 練習モードでプレイしてください。（プレイボタンの横のボタンを押してください）

**Made changes to your map while the game is open?**  
Click on the game window. Then while you are on the Main Menu or Song Select Menu press <kbd>Ctrl + r</kbd> on your keyboard. Your changes will be loaded without needing to restart the game!

:::tip NOTE

* You will need to have the **SongCore** mod installed in order to see the CustomWIPLevels category and use the <kbd>Ctrl + r</kbd> shortcut.
* Having duplicate map files in `CustomLevels` and `CustomWIPLevels` can cause problems.
* Using Online Websites to convert audio to `.ogg` may result in your audio file being treated as invalid and will not be loaded by the game! Using Audacity and following the steps in [Basic Audio Setup](./basic-audio.md) is the easiest way to ensure your map loads in-game. :::

### Questでテストプレイ
Follow these steps to test any of your maps made with a community editor using an Oculus Quest. You must have [SideQuest](https://sidequestvr.com) and [BMBF](https://bmbf.dev/stable) installed.

1. PC上でWIPソングフォルダを探します。
2. PCとQuestを接続します。
3. PCでSideQuestを開き、右上のフォルダアイコンをクリックします。 ![SideQuest Files](~@images/beginners-guide/sqfiles.png)
4. `sdcard/ModData/com.beatgames.beatsaber/Mods/SongLoader/CustomWIPLevel` に移動します。 このフォルダが存在しない場合は、 自分で作成できます。
5. PCからSideQuestでそのフォルダにテストプレイしたい曲をアップロードします。
    * **注意:** zipファイルではなく、解凍したフォルダが必要です。
6. ゲーム内のCustomWIPLevelsのプレイリストにマップが表示されます。 通常のPlayボタンではなく、 練習モードのプレイしかできないことに注意してください！

:::tip NOTE Using Online Websites to convert audio to `.ogg` may result in your audio file being treated as invalid and will not be loaded by the game! Using Audacity and following the steps in [Basic Audio Setup](./basic-audio.md) is the easiest way to ensure your map loads in-game. :::

### コミュニティ/サードパーティーテスト
The `#testplays` channel in the [Beat Saber Modding Group Discord](https://discord.gg/beatsabermods) makes it easy to have your work checked by knowledgeable mappers. Playtesters will provide constructive feedback on how to improve your map in either video or text format in a DM or in the `#mapping-discussion` channel.

:::warning Some things to note...

* Maps with less than 1 minute done will not get much feedback or be tested. Consider asking in `#mapping-discussion` to see if someone will take a look instead.
* Challenge/Super High difficulty maps may take longer to get feedback since there are not many playtesters at this skill level.
* Please keep to serious posts where you are looking to improve your mapping skills. Meme or Shitpost maps do not belong as they end up wasting the testplayers time.
* Make sure you have run your map through a checker program such as those built-in to your editor or external tools like Parity Checker or Map Check in [Additional Mapping Tools](#additional-mapping-tools) :::

1. 譜面を圧縮して.zip ファイルを作成します。
    * [MMA2](./mediocre-map-assistant.md)を使用している場合は`Package Song to Zip` ボタンを押すと、zipファイルが作成されます。  
      ![Package Song to Zip button](~@images/mapping/mma2-package-zip.jpg)
    * [Beatmapper.app](#beatmapper-app)を使用している場合は [ダウンロード方法](https://beatmapper.app/docs/manual/publishing#downloading-your-map) に従ってください。
    * [このガイド](https://streamable.com/u20ci)のように手動でzipファイルを作成することもできます。
2. Upload your map to `#testplays` using the following format:

* **Map:** The name and artist of your map
* **Length:** The length of the song
* **BPM:** The BPM of the song
* **Difficulty:** Which difficulties are included
* **NPS:** The notes per second of each difficulty available
* **Feedback:** Any requests for feedback (specific difficulties to be tested, things to look for etc.)
* **Status:** What state is the map in? (i.e., First draft complete, no lights; 1:45 mapped; release candidate w/ lighting; etc.)

3. テストプレイヤーは1-7日の間にあなたのマップをみて絵文字でリアクションを取ります。`#testplays`チャンネルでピン止めされている絵文字リストを 参照してください。

:::warning Remember: If you make changes after posting or getting feedback React with a 🛑 `:octagonal_sign:` to indicate stop testing this version :::

You can copy and paste the following template into Discord:

```txt
**Map:**
**Length:**
**BPM:**
**Difficulty:**
**NPS:**
**Feedback:**
**Status:**
```

### テストプレイする方法
Do you like the idea of playing new songs before they are ever released on BeatSaver? Do you want to help shape the mapping community? Consider becoming a testplayer! Check out the [How to Testplay](./how-to-testplay.md) guide to get started!

## マップを公開する
Once your song has been mapped, lighted, and playtested and it’s a finished product you’re ready to release it to the world!

### BeatSaver
[BeatSaver](https://beatsaver.com/) is the public repository for all custom Beat Saber maps.

#### マップを公開する方法

::: danger

* Please **DO NOT** upload an incomplete WIP map to BeatSaver!
  * Uploading to BeatSaver equates to "Putting it on the store shelf" and should **only** be your final version.
  * See the [Playtesting](#playtesting) section for instructions on testing your map. :::

1. [ユーザー名/パスワードを使用して BeatSaver で](https://beatsaver.com/register) アカウントを作成するか、Discord経由でログインしてください。
    * Beatsaverのユーザー名には英数字と `-`のみ使用できます。 例えば、スペースや `_` はユーザー名に 使用できません。
2. 右上の <kbd>Upload</kbd> リンクをクリックします。
3. 譜面の名前とその説明を書きます。 譜面の名前が検索されるので、曲名、アーティストや関連する単語を入れると譜面が見つけやすくなります。
    * Use "tags" like (Chroma), (OneSaber), or (Mapping Extensions) if your map uses some special modifications or characteristics you want to highlight.
    * Putting a link to a playthrough video in the map description can help you get more downloads as it is easier to share your map to others and lets people know what to expect.
4. .zipファイルを追加し、譜面を人が作ったのかAIの補助があったのかを確認します。
    * 自動作成された譜面を人が作成したものとしてアップロードした場合、譜面は削除されます。
5. マップは最初に未公開のタブにアップロードされます。 公開するためには、パブリッシュする必要があります。

::: tip NOTE
Map files can now be updated on BeatSaver!
If you need to upload a new version of your map you must first recall the map to your unpublished tab before you can
upload a new version. This will retain your map key and statistics but will reset all leaderboards.
:::

### BeatSaver トラブルシューティング
Here are solutions for some common errors when uploading a Beatmap.  
Encountered something not listed here? Drop into `#mapping-discussion` for assistance.

:::danger Remember:

* You should have your map [playtested](#playtesting) before uploading!
* You do not need upload maps created by auto-generation software such as Deepsaber or Beat Sage to install them in your game. If you are on PC, you can unzip the files into your `CustomLevels` folder. If you are on Quest, follow the [Testing on a Quest](#testing-on-a-quest) steps to install the map. :::

---

#### Map already uploaded（マップはすでにアップロードされています）

* The exact map files were uploaded previously. You must change something small in your map (i.e., remove a light block, save the map, replace the light block, and save again) to be able to upload.

---

#### _difficultyBeatmapSets[]._difficultyBeatmaps[].`Difficulty.dat`._version``: Must not be null

* You are using an old, outdated editor that is not compliant with the current data schema. See [Community Editors](#community-editors) for the current options.

---

#### サーバー内部エラー
This is the default error message, causes include:

* An upload that is close to or over the actual file size limit of 15 MB. Reduce the audio export quality slightly to make space.
* Unsupported characters are present in a file. Make sure your metadata and bookmarks don't contain special characters such as, Japanese (日本語/にほんご), Kaomoji (٩(◕‿◕｡)۶), Chinese (汉语/漢語), Arabic (اَلْعَرَبِيَّةُ‎), and accented characters (Ä/é/õ/Æ/ø/ß/Œ/Ð/ƒ).
  * [+1 Rabbit's Mapping Tools](https://skystudioapps.com/mapping-tools/) by **+1 Rabbit** may be useful in finding the specific problem.
* Expired web session. If you refresh the page, you should be logged out. Login and try to upload again.

---

#### Could not verify user []

* This error is related to recaptcha. Please reload the page.

---

#### ``_difficultyBeatmapSets[]._difficultyBeatmaps[]`Difficulty.dat`._notes[]_time:`` Must be between 0 and x

* Your map contains notes outside of the playable map (usually from a copy and paste error). Remove them and reattempt your upload.

---

#### Beatmap zip contains an illegal file! 旧バージョン

* Usually caused by extra/unsupported files, such as gifs, in the zip.

---

#### Beatmap does not contain an Info.dat file! 旧バージョン

* Usually caused by having the files in a subfolder. You need to zip the files instead of the folder. [How to Video](https://streamable.com/u20ci) Or use the handy export button in your editor instead. **NOTE: MMA2's export button does not include contributor images in the zip.**

---

#### One or more beatmap difficulty files cannot be found! 旧バージョン

* You might have forgotten to include all of your difficulty files are in the zip.
* A difficulty's `"_beatmapFilename"` in the `Info.dat` might be using a different file name than what is present in the folder.
* A deleted difficulty is still being referenced in your `Info.dat` file. Check to make sure you do not have unintended difficulties in the `"_difficultyBeatmaps"` cluster of each present characteristic.

---

#### Error in `MapDifficulty.dat`. Root should NOT have additional property: `_time`. 旧バージョン

`_time` is the common error for this type of message. However, the same solution applies if a different property is flagged.

* Your files are not compliant the map schema. See [Schema Change](#beatsaver-data-schema-change-october-27-2019) for solutions.

---

#### Beatmap could not be parsed! 旧バージョン

* This could be caused by extreme server load. Try again later or ask in `#mapping-discussion`.

---

#### Field `._customData._contributors[]._iconPath` contains an invalid filename. 旧バージョン

* Utilizing the contributors field requires all aspects to be included. Make sure all 3 aspects (Role, Name, iconPath) are filled and there is a unique square image for each iconPath entry in your zip.

---

### BeastSaber
[BeastSaber](http://www.bsaber.com) is a song review and curation site with social features including reviewing and commenting on songs. All songs published on BeatSaver are mirrored to BeastSaber within 10-15 minutes. Additionally, maps deleted from BeatSaver may take up to a day to be removed from BeastSaber.

## [クレジット](./mapping-credits.md)
Over *thirty* different mapping guides and tutorials have been combined into this wiki so that it can be maintained by the community as a whole. Many many **MANY** thanks to the mappers who blazed this trail and contributed content. Check out the whole list [here!](./mapping-credits.md)
