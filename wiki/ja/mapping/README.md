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
3. マッピングエディタで曲を設定します(ステップはエディタによって異なりますが、ここでは MMA2の[ユーザーガイド](./mediocre-map-assistant.md)に従います)
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
* [初心者として回避すべきCyrixのパターン](https://www.youtube.com/watch?v=mgGaqZ20Scw) - [Basic Mapping](./basic-mapping.md) で議論されている最も一般的な問題をカバーします。
* [TransquillizeMe's Beat Saber Lighting Techniques チュートリアル](https://www.youtube.com/watch?v=EDbPRN_u3jc) - さまざまな照明効果と一般的な照明のヒントをカバーします。

:::warning このページのチュートリアルは BSMG によって調査されています。 他のビデオチュートリアルは、最新の情報でなかったり、正確でない可能性があります。それらのビデオを見る場合はご自身でそのリスクを理解する必要があります。

あなたのチュートリアルがこのリストに入れたい場合は、 [お問い合わせください](http://bit.ly/MessageBSMG). :::

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
::: warning 標準のエディタはたくさん機能がありVRを必要としません。しかしバグが起きる可能性があり、注意が必要です。 ::: これらのエディタのキーボードショートカットの一覧は[こちらから](./editor-keybinds.md)利用できます。

#### Mediocre Map Assistant 2
MMA2はもっとも機能的な3Dエディタで譜面編集コミュニティで大多数のひとが使用しています。

* [Mediocre Map Assistant 2のダウンロード](https://git.bsmg.wiki/Top_Cat/MediocreMapAssistant2/releases/latest)
* [Mediocre Map Assistant 2のガイド](./mediocre-map-assistant.md)

#### Beatmapper.app
ブラウザ上で起動する３Dマップエディターは誰でも譜面作成ができます。 拡張機能なしの標準的な機能がありますが、いくつかの新しい機能が付かされています。

* [Beatmapper ウェブサイト](https://beatmapper.app/)
* [Beatmapper ユーザーマニュアル](https://beatmapper.app/docs/manual/getting-started)

#### ChroMapper - *近日公開*
3Dエディタは照明効果、ChromaでのRGBなどビートセイバーとよく似たセッティングを持っていることによりより正確なプレビュー表示ができます。 ChroMapper は現在クローズドベータ版で公開予定日はありません。

::: tip 自分のエディタやコンバーターを作ることに興味がありますか? [マップフォーマットページ](./map-format.md) と [SongCore Readme](https://github.com/Kylemc1413/SongCore/blob/master/README.md) が役に立ちます！ :::

### 公式版エディター
公式のエディタはBeat Games によって開発されており、Steam VRとOculus PC版であらかじめインストールされています。 これはゲーム内からワンクリックでアクセスできるのでテストプレイ中などに便利です。 公式のエディタは2次元なので3Dとして想像する力が必要です。これは初心者には難しいと思われます。 大多数の譜面作成者は[コミュニティのエディタ](#community-editors)を使っています。

* アクセスするためにはヘッドセット内でBeatSaverのエディタを起動するかPCからfpfcをつかって直接起動させてください。
* 標準的なマッピングの概要については、Megalonの [公式エディタチュートリアルビデオ](https://www.youtube.com/watch?v=5Ex6sOEVgrM) をご覧ください!

公式が [Community Editors](#community-editors) と比較して以下の機能を搭載していません。

* 1/5などの珍しい倍率での設定
* オートセーブとバックアップ（公式エディタはテスト時と保存したときのみセーブされます）
* 複数選択とコピー、ペースト
* 配置しながらの編集（ノーツを削除することなく方向を変更できます）
* Chroma RGB サポート
* オーディオのオフセット設定 (公式のオフセット/遅延のパラメータは曲だけでなくヒットサウンドも含まれます)
* エラーチェッカー
* コントリビューターフィールド
* MappingまたはNoodle Extensionsのサポート

#### Migrating from Official Editor to a Community Editor
Although it is recommended to start setup again following the [Quick Start](#mapping-quick-start) guides with a [Community Editor](#community-editors), it is possible to transfer your work in the Official Editor over.

1. Install a [Community Editor](#community-editors)
2. Locate your map files in your game's `CustomLevels` folder.
    * Steam Example Location: `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\Beat Saber_Data\CustomLevels`
    * Oculus Example Location: `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber_Data\CustomLevels`
3. Move it to the folder your editor is looking in. This is commonly the `CustomWIPLevels` in the `Beat Saber_Data` folder.
    * Steam: `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\Beat Saber_Data\CustomWIPLevels`
    * Oculus: `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber_Data\CustomWIPLevels`
4. Convert your audio file to the `.ogg` format from `.wav` if you have not done so.
    1. Download and Install [Audacity](https://www.audacityteam.org/)
    2. Open the `.wav` file in Audacity
    2. Click the `File menu -> Export -> Export as OGG.`
    3. Name your file `song.ogg` and click <kbd>Save</kbd>.
    4. Place the `song.ogg` file into the map folder.
        * You no longer need the `.wav` song file in this folder
5. Open the map in the community editor and change the song file name to `song.ogg` and click the save button.

You are now ready to continue editing your map!

### 追加のマッピングツール

* [BS Viewer](https://skystudioapps.com/bs-viewer/) by **+1 Rabbit**  
  A convenient way to see how your map might look in game without the game.
  * IOS and Safari are currently not supported
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
  An error checker tool that is much more versatile than the one built into MMA2
* [BeatMapper Tools](https://mappers.beatmappertools.com/) by **Darkuni**  
  A utility for users of Mediocre Mapper and Mediocre Map Assistant 2 to easily convert, test, and package their maps
* [noodleLister](https://github.com/bloodcloak/noodleLister#readme) by **Bloodcloak**  
  Easily compile a game playlist from a txt file containing BeatSaver map keys.
* [BeatMerge](https://github.com/ZelonGames/BeatMerge#readme) by **DarkGrisen**  
  Ever thought that it is a lot of annoying work to make big maps with other people or to perfectly cut the audio files so you can merge them manually later? This tool allows you to merge two or more maps into one single super long map.
* [Cinder](https://github.com/zhaey/cinder#readme) by **zhaey**  
  Python program that converts stepmania `.sm` files to Beat Saber `.dat` files for timing notes.

#### Legacy Tools

* [BPM Saber](https://github.com/zevdg/bpm-saber#readme) by **Zevdg**  
  **Only works on old format .json files. For .dat maps use the Tempo Changer in +1 Rabbit's Mapping Tools.** Change the BPM of an entire map and shift block placements accordingly
* [BPM Saber](https://bsaber.com/bpmsaber/) by **Elliotttate**  
  A utility for finding the BPM of a song by upload or tapping.
* [osu! Editor Timing Tutorial](https://www.youtube.com/watch?v=nIX0koHzW8c&t) by **Fayhe**  
  Video guide on using the timing feature of osu!'s editor to find map bpm.

### Useful Mods
Here are some mods that might make your mapping workflow a little easier.

* [SiraUtil](./basic-lighting.md#in-game-with-fpfc) by **auros**  
  With the First Person Flying Controller (FPFC) launch parameter, this allows you to control the game while a map is playing with your keyboard and mouse without using a headset. See the section in [Basic Lighting](./basic-lighting.md#in-game-with-fpfc) for links to the mods and how to set it up.
* [PracticePlugin](https://github.com/Kylemc1413/PracticePlugin) by **Kyle1413**  
  Mod for Beat Saber to control playback speed, seek through songs and set up looping sections. Install the latest version from [Mod Assistant](https://github.com/Assistant/ModAssistant#readme)!
* [ReLoader](https://github.com/Kylemc1413/ReLoader) by **Kyle1413**  
  Allows you to hot reload beatmaps in practice mode without needing to return to the menu to refresh. Really convenient for wall mapping.

## Mapping Practices
> "You have to know the rules before you can break them."  
> \- Uninstaller

There is no holy bible of mapping but this section of the wiki includes a lot of tribal knowledge from the community on best practices at all levels of mapping. Our advice is to follow these rules until you're comfortable with your skills and then get creative, experiment, and innovate!

### [**基本的なマッピング**](./basic-mapping.md)
これから譜面を作成しようとする人はみなこれを読む必要があります。**例外はありません！**

### [**中級者向けの譜面作成ガイド**](./intermediate-mapping.md)
A more in-depth look at many mapping topics **(This page is still a work in progress!)**

### [**Extended Mapping**](./extended-mapping.md)
Mapping Extensions, Extra Characteristics, and 360&deg;/90&deg; mapping

### Mapper Roles
To apply for the **Mapper** role on the [Beat Saber Modding Group Discord](https://discord.gg/beatsabermods) you must have released three solid/playable maps (collaborations are acceptable) and complete the [Mapper Role Submission Form](https://forms.gle/mj66J3UopTykFJjXA). Your application and maps may take a decent amount of time to be reviewed and approved.

### Modding & Ranking
Maps that meet specific [Ranking Criteria](https://scoresaber.com/criteria) and go through an intensive review process called "modding" have the potential to become ranked, awarding players Performance Points (PP) toward global leaderboards. More information and an in-depth FAQ is available on the [ScoreSaber Discord](https://discord.gg/WpuDMwU)

* Prior to requesting ranking, mappers should thoroughly review the ranking criteria and [metadata standards](https://docs.google.com/document/d/1ehotupIYMVlc8x41JldO-24m7Am-oTVYnciF9KCRdNM/edit) and have their map modded by a knowledgeable source.

:::tip Want an even more detailed look? Review the [Ranking Criteria](https://scoresaber.com/criteria) for some of the more ambiguous ranking considerations. :::

* Once your map has been modded and revised, it’s ready to be presented to a ranking team member or recruit to review.
* If the ranking team member deems the map acceptable it will be added to the ranking request queue to be voted on by the full ranking team.

## 照明効果
A map is not finished until some form of lighting is included. Lighting can range from very basic to incredibly detailed using additional mods to enable more features.

### [**基本的な照明効果**](./basic-lighting.md)
Learn the various aspects to lighting your map manually

### [**中級照明効果**](./intermediate-lighting.md)
Take your lighting skills a bit further into strobing, ring spins, and contrast practices

### [**高度な照明効果**](./advanced-lighting.md)
Advanced and nuanced techniques, lighting for custom platforms, and Chroma RGB **(This page is still a work in progress!)**

### Additional Resources
Older guides linked here as we migrate their content over to the wiki pages.

* [Beginner's Guide to Lighting](https://docs.google.com/document/d/1wpZgBeOD1-UbJpXf-b6gX5ICNYygCd6UK6LOPm-t5QM/edit) by Puds
* [Lighting Environment Guide](https://bsaber.com/creating-lighting-environment-guide/) by ManDynasty
* [Using Flash & Fade Lighting Events](https://bsaber.com/creating-lighting-how-flash-fade-notes-actually-work-in-game/) by ManDynasty
* [Side Laser Speed Reference](https://docs.google.com/spreadsheets/d/1tIERmSyFI4ssjDkE-oJjBBvUZUJ7eoVhCQyM3_BsJwE/edit?usp=sharing) by LittleAsi

### Automated Lights
Not ready to make your own lighting? Here are some programs to do it for you. Keep in mind, creating simple manual lighting is not difficult and will always be better at expressing the atmosphere of the song than using these programs.

* [Lolighter](https://github.com/Loloppe/Lolighter#readme) by **Loloppe#6435** - Standalone program for automated lighting and has other features to modify your map.
* **Lightmap** - It is integrated into Mediocre Map Assistant 2 and can be accessed in the error checker menu.

## Playtesting
Testing your work is a **critical** part of mapping. Testing as you work helps you adjust for major playability issues and get a feel for your map. [Third-party or "outside"](#community-third-party-testing) playtesting is when someone other than yourself tests your pre-release map and provides constructive feedback and is helpful in highlighting issues to which you may be "map blind."

::: danger You **DO NOT** need to upload your map to BeatSaver in order for you or anyone else to test. :::

* If your map is using the 1.0 song format (your files are .json and .ogg) you must convert your map using one of several available tools like [Songe Converter](https://github.com/lolPants/songe-converter) by lolPants or [BeatMapper Tools](https://mappers.beatmappertools.com/) by Darkuni. **Update your editor to MMA2 or Beatmapper**. See [Community Editors](.#community-editors) for links.
* If your map is using the 2.0 song format (your files are .dat and .ogg/.egg) you’re ready to test.

### Testing on a PC
Follow these steps to test any of your maps made with a community editor using PC-based VR.

1. If your WIP song folder isn’t already in `Beat Saber_Data\CustomWIPLevels` then place a copy there.
2. Access your map in-game via the CustomWIPLevels category in the song pack menu. Use practice mode to play (the button next to the play button).

**Made changes to your map while the game is open?**  
Click on the game window. Then while you are on the Main Menu or Song Select Menu press <kbd>Ctrl + r</kbd> on your keyboard. Your changes will be loaded without needing to restart the game!

:::tip NOTE

* You will need to have the **SongCore** mod installed in order to see the CustomWIPLevels category and use the <kbd>Ctrl + r</kbd> shortcut.
* Having duplicate map files in `CustomLevels` and `CustomWIPLevels` can cause problems.
* Using Online Websites to convert audio to `.ogg` may result in your audio file being treated as invalid and will not be loaded by the game! Using Audacity and following the steps in [Basic Audio Setup](./basic-audio.md) is the easiest way to ensure your map loads in-game. :::

### Testing on a Quest
Follow these steps to test any of your maps made with a community editor using an Oculus Quest. You must have [SideQuest](https://sidequestvr.com) and [BMBF](https://bmbf.dev/stable) installed.

1. Zip up the song as normal, only zipping the files and not the folder itself. [How to Video](https://streamable.com/u20ci)
   * If you are using [MMA2](#mediocre-map-assistant-2) there is a `Package To Zip` button you can use in the song info screen to do this for you.
2. Establish a connection to your Quest from your PC. This can be done in two ways, [wired](#connect-wired-usb) and [wirelessly](#connect-wirelessly).

#### Connect Wirelessly

1. Open BMBF on the Oculus Quest. BMBF must be running for the connection to succeed.
2. Inside BMBF go to the `Tools` tab. There you should see a web address and a version number similar to what is shown below. <br/>![ip](~@images/mapping/ip.png)
3. Open a modern web browser on your PC and type the address into the search bar. You should be greeted with this screen below.<br/>![BMBF Web](~@images/mapping/bmbfweb.png)
4. You are now connected! Continue on to the [Upload Test File to Quest](#upload-test-file-to-quest) steps below.

#### Connect Wired USB

1. Connect your Oculus Quest to the PC via USB and keep SideQuest open
2. Open BMBF on the Oculus Quest. BMBF must be running for the connection to succeed
3. Look at the top of SideQuest, which will give you the IP to get into BMBF. You can also access your IP through the Tools tab of BMBF.
4. Type into any web browser: "192.168.X.XXX:50000" with X being replaced with the IP displayed in SideQuest, or the Tools tab<br/>![Quest IP](~@images/mapping/quest_ip.png)  
   For example, from the picture you would enter `192.168.0.19:50000` into a web browser of choice (Chrome, Firefox, etc.).
5. You are now connected! Continue on to the [Upload Test File to Quest](#upload-test-file-to-quest) steps below.

#### Upload Test File to Quest

1. Drag and drop the files into BMBF's upload page (indicated by /main/upload at the end of the link)
2. Once uploaded, click Sync to Beat Saber at the top right corner of the page <br/>![BMBF Browser](~@images/mapping/bmbf_browser.png)
3. Access your map in-game via the Custom Songs playlist in the song pack menu. Use practice mode to play (the button next to the play button).

:::tip NOTE

* If after deleting an old copy of a map and reuploading it with a new version on a quest still results with the old version being played, rename the zip file before uploading it through BMBF.
* BMBF may have issues importing your map if your song file or cover image name contains `-` or spaces. You may need to rename these files and update the song info accordingly for a successful upload.
* Using Online Websites to convert audio to `.ogg` may result in your audio file being treated as invalid and will not be loaded by BMBF! Using Audacity and following the steps in [Basic Audio Setup](./basic-audio.md) is the easiest way to ensure your map loads in-game.
* If your song audio file was automatically converted to `.egg`, you may run into issues when uploading onto BMBF. Try renaming the `.egg` back to `.ogg`. :::

### Community / Third Party Testing
The `#testplays` channel in the [Beat Saber Modding Group Discord](https://discord.gg/beatsabermods) makes it easy to have your work checked by knowledgeable mappers. Playtesters will provide constructive feedback on how to improve your map in either video or text format in a DM or in the `#mapping-discussion` channel.

:::warning Some things to note...

* Maps with less than 1 minute done will not get much feedback or be tested. Consider asking in `#mapping-discussion` to see if someone will take a look instead.
* Challenge/Super High difficulty maps may take longer to get feedback since there are not many playtesters at this skill level.
* Please keep to serious posts where you are looking to improve your mapping skills. Meme or Shitpost maps do not belong as they end up wasting the testplayers time. :::

1. Create a compressed .zip file of the individual song files.
    * If you are using [MMA2](./mediocre-map-assistant.md), you can press the `Package Song to Zip` button in the Song Info Settings to create a compressed .zip of your map.  
      ![Package Song to Zip button](~@images/mapping/mma2-package-zip.jpg)
    * If you are using [Beatmapper.app](#beatmapper-app), follow their [downloading instructions](https://beatmapper.app/docs/manual/publishing#downloading-your-map).
    * You can manually create the zip by following this [How to Video](https://streamable.com/u20ci) if you are not using a web based editor.
2. Upload your map to `#testplays` using the following format:

* **Map:** The name and artist of your map
* **Length:** The length of the song
* **BPM:** The BPM of the song
* **Difficulty:** Which difficulties are included
* **NPS:** The notes per second of each difficulty available
* **Feedback:** Any requests for feedback (specific difficulties to be tested, things to look for etc.)
* **Status:** What state is the map in? (i.e., First draft complete, no lights; 1:45 mapped; release candidate w/ lighting; etc.)

3. Testers will usually look at your map within 1-7 days and will use a number of reaction emojis (listed in `#testplays` pinned posts) to track testing status.

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

### Help Playtest
Do you like the idea of playing new songs before they are ever released on BeatSaver? Do you want to help shape the mapping community? Consider becoming a testplayer! Check out the [How to Testplay](./how-to-testplay.md) guide to get started!

## Publishing Songs
Once your song has been mapped, lighted, and playtested and it’s a finished product you’re ready to release it to the world!

### BeatSaver
[BeatSaver](https://beatsaver.com/) is the public repository for all custom Beat Saber maps. Songs must be in the 2.0 song format (files are .dat and .ogg/.egg/.wav) to be uploaded.

#### How to Release a Map

::: danger

* Please **DO NOT** upload an incomplete WIP map to BeatSaver!
  * Uploading to BeatSaver equates to "Putting it on the store shelf" and should **only** be your final version.
  * See the [Playtesting](#playtesting) section for instructions on testing your map. :::

1. [Create an account](https://beatsaver.com/auth/register) on BeatSaver.
    * Beatsaver usernames may only have alphanumeric characters and `-`. Usernames with spaces or `_` for example, are not allowed.
    * If you did not receive a verification email, fill out this [contact form](https://beatsaver.com/contact).  
      **Note** you must provide a valid username *and* the email used to sign up in the form to complete the verification!
2. Click the <kbd>Upload</kbd> link in the top-right.
3. Add your BeatSaver map name and map description. Only the map name is searchable so be sure to include song name, song artist, and other terms that might make it easier to find your map.
    * Use "tags" like (Chroma), (OneSaber), or (Mapping Extensions) if your map uses some special modifications or characteristics you want to highlight.
    * Putting a link to a playthrough video in the map description can help you get more downloads as it is easier to share your map to others and lets people know what to expect.
4. Add your .zip file and click the <kbd>Upload</kbd> button.

::: tip NOTE Map files currently cannot be updated on BeatSaver. If you need to upload a new version of your map you will need to delete the old one and re-post. :::

### BeatSaver Troubleshooting
Here are solutions for some common errors when uploading a Beatmap.  
Encountered something not listed here? Drop into `#mapping-discussion` for assistance.

:::danger Remember:

* You should have your map [playtested](#playtesting) before uploading!
* You do not need upload maps created by auto-generation software such as Deepsaber or Beat Sage to install them in your game. If you are on PC, you can unzip the files into your `CustomLevels` folder. If you are on Quest, follow the [Testing on a Quest](#testing-on-a-quest) steps to install the map. :::

---

**Something went wrong! Try again later.** This is the default error message, causes include:

* An upload that is close to or over the actual file size limit of 14.3 MB. The 15 MB listed is not accurate at this time. Reduce the audio export quality slightly to make space.
* Unsupported characters are present in a file. Make sure your metadata and bookmarks don't contain special characters such as, Japanese (日本語/にほんご), Kaomoji (٩(◕‿◕｡)۶), Chinese (汉语/漢語), Arabic (اَلْعَرَبِيَّةُ‎), and accented characters (Ä/é/õ/Æ/ø/ß/Œ/Ð/ƒ).
  * [+1 Rabbit's Mapping Tools](https://skystudioapps.com/mapping-tools/) by **+1 Rabbit** may be useful in finding the specific problem.
* Expired web session. If you refresh the page, you should be logged out. Login and try to upload again.

---

**Field `._customData._customEnvironment` cannot be blank.**

* Your files are not compliant the map schema. See [Schema Change](#beatsaver-data-schema-change-october-27-2019) for solutions.

---

**Beatmap zip contains an illegal file!**

* Usually caused by extra/unsupported files, such as gifs, in the zip.

---

**Beatmap already exists!**

* The exact map files were uploaded previously. You must change something small in your map (i.e., remove a light block, save the map, replace the light block, and save again) to be able to upload.

---

**Beatmap does not contain an Info.dat file!**

* Usually caused by having the files in a subfolder. You need to zip the files instead of the folder. [How to Video](https://streamable.com/u20ci) Or use the handy export button in your editor instead. **NOTE: MMA2's export button does not include contributor images in the zip.**

---

**One or more beatmap difficulty files cannot be found!**

* You might have forgotten to include all of your difficulty files are in the zip.
* A difficulty's `"_beatmapFilename"` in the `Info.dat` might be using a different file name than what is present in the folder.
* A deleted difficulty is still being referenced in your `Info.dat` file. Check to make sure you do not have unintended difficulties in the `"_difficultyBeatmaps"` cluster of each present characteristic.

---

**Error in `MapDifficulty.dat`. Root should NOT have additional property: `_time`.**

`_time` is the common error for this type of message. However, the same solution applies if a different property is flagged.

* Your files are not compliant the map schema. See [Schema Change](#beatsaver-data-schema-change-october-27-2019) for solutions.

---

**Beatmap could not be parsed!**

* This could be caused by extreme server load. Try again later or ask in `#mapping-discussion`.

---

**Field `._customData._contributors[]._iconPath` contains an invalid filename.**

* Utilizing the contributors field requires all aspects to be included. Make sure all 3 aspects (Role, Name, iconPath) are filled and there is a unique square image for each iconPath entry in your zip.

---

#### BeatSaver Data Schema Change - October 27, 2019
BeatSaver now enforces a schema in order for your maps to be uploaded, of which public MediocreMapper is not compliant with. The most breaking change happened in the difficulty data files, where MM-specific fields were moved inside a `_customData` object.

**Resolution #1:**  
Switch to the [Mediocre Map Assistant 2](#mediocre-map-assistant-2) editor. Open each difficulty file and save it to correct the schema. Use MMA2 going forward.

**Resolution #2:**  
Use the [Schema Updater Utility](https://skystudioapps.com/mapping-tools/#schema-fixer) by **+1 Rabbit** to fix your files before uploading. Then switch to a [supported editor](#community-editors).

**Resolution #3 (The Hard Way):**  
If you wish to fix this yourself, here is a quick template which shows you where everything should go in order for your map to be compliant with BeatSaver's new schema.

Alternatively, since `_customData` is **NOT** a required field, you can go ahead and remove everything that would be placed in there, and upload that result.

```json
{
  "_version": "2.0.0",
  "_notes": [],
  "_obstacles": [],
  "_events": [],
  "_customData": {
    "_bpmChanges": [],
    "_bookmarks": [],
    "_time": 0
  }
}
```

To be compliant with the new schema, please also find and remove or fill in any **blank fields** in your `Info.dat` or difficulty files.

### BeastSaber
[BeastSaber](http://www.bsaber.com) is a song review and curation site with a social side for member profiles, forums, news, and tutorials. All songs published on BeatSaver are mirrored to BeastSaber within 10-15 minutes. Additionally, maps deleted from BeatSaver may take up to a day to be removed from BeastSaber.

### Mapping Anxiety
If you're finding it difficult to muster up the courage to upload your map, or are finding it emotionally taxing coping with a lack of downloads or a lot of dislikes, you're not alone. Many mappers have experienced these feelings. You can read more about it on the [Coping with Mapping Anxiety](./mapping-anxiety.md) page.

## [Credits](./mapping-credits.md)
Over *thirty* different mapping guides and tutorials have been combined into this wiki so that it can be maintained by the community as a whole. Many many **MANY** thanks to the mappers who blazed this trail and contributed content. Check out the whole list [here!](./mapping-credits.md)
