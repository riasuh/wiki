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
公式のエディタはBeat Games によって開発されており、Steam VRとOculus PC版ではあらかじめインストールされています。 これはゲーム内からワンクリックでアクセスできるのでテストプレイ中などに便利です。 公式のエディタは2次元なので3Dとして想像する力が必要です。これは初心者には難しいと思われます。 大多数の譜面作成者は[コミュニティのエディタ](#community-editors)を使っています。

* アクセスするためにはヘッドセット内でBeatSaverのエディタを起動するかPCからfpfcをつかって直接起動させてください。
* 標準的なマッピングの概要については、Megalonの [公式エディタチュートリアルビデオ](https://www.youtube.com/watch?v=5Ex6sOEVgrM) をご覧ください!

公式のエディタにはいくつかの[コミュニティのエディタ](#community-editors)の機能がありません。

* 1/5拍などの細かい配置
* オートセーブとバックアップ（公式エディタはテストと保存を実行したときのみセーブされます）
* 複数選択とコピー、ペースト
* 配置しながらの編集（ノーツを削除することなく方向を変更できます）
* Chroma RGB サポート
* オーディオのオフセット設定 (公式のオフセット/遅延のパラメータは曲だけでなくヒットサウンドも含まれます)
* エラーチェッカー
* コントリビューターフィールド
* MappingまたはNoodle Extensionsのサポート

#### 公式エディターからコミュニティエディターへの移行
[ コミュニティエディタ](#community-editors) を使用して[クイックスタート](#mapping-quick-start)ガイドに従って再度セットアップすることをお勧めします。公式のエディタに移行することができます。

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

譜面の編集を続ける準備ができました！

### データ損失防止とクラウドストレージ
ゲームをアップデートするとカスタム曲がすべてなくなることがあります。これを防ぐために [Symbolic Links](https://ja.wikipedia.org/wiki/ソフトリンク)を使うという方法があります。これは譜面情報をコンピュータの別の場所にも保存します。例えば、クラウドと同期されたファイルであったり、ゲーム内に直接保管します。 アップデートやアンインストールによりマップが削除された場合でも、作成されたリンクは削除されません。 再帰的な削除によって譜面を削除します

クラウドストレージフォルダを使用することで、複数のコンピュータ間で操作する場合やストレージディスクが破損したときなどに便利です。

以下の手順はWindows 10および11の場合のものです。

1. 現在のレベルフォルダを新しい場所に移動します。 (`Ctrl + c` の代わりに `Ctrl + x`)
   * これがクラウド上のファイルである場合は、オフラインで利用できるようにフォルダを設定してください!
2. コマンドプロンプトを開く
3. 場合によってはパラメータを調整するコマンドを実行します。  
     
   `mklink /j "Path to Beat Saber Install folder" "Path to New Location"`
    * コマンド例:  
      `mklink /j "C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\Beat Saber_Data\CustomLevels" "C:\Users\cmb\CloudStorage\CustomLevels"`

ネットワークドライブ上にある場合は、 `/j` を `/D` に置き換えます。 この方法を実行するにはコマンドプロンプトを開く必要があることに注意してください。

### 追加のマッピングツール

* [BS Viewer](https://skystudioapps.com/bs-viewer/) by **+1 Rabbit**  
  ゲームを起動しなくても譜面がどのよう見えるのかを確かめる便利なソフトです。
* [+1 Rabbit's Mapping Tools](https://skystudioapps.com/mapping-tools/) by **+1 Rabbit**  
  譜面作成における便利なツールが含まれています。
  * **Schema Fixer:** BeatSaver にアップロードできるようにMediocre Mapper Mk4.1 と Mk5 で作成したマップを簡単に修正してくれます。
  * **Tempo Changer:** マップ全体の BPM を変更し、それに応じてノーツ配置をシフトします。
  * **Offset Remover:** 浮動小数点誤差を軽減するために、エディタのオフセットを削除し、ノーツ/ボム、壁/イベントを一般的なタイミングにスナップします。
  * **Note Soter:** スタックを修正するために、マップファイル内の乱雑になっているノート/障害/イベントをソートします。
  * **Copy Timing:**特定のノーツを他の難易度にコピーします。 すべての難易度である音に対してタイミングを少しだけずらしたい時などに便利です。
  * **Copy Lighting:** 1つの難易度からほかの難易度すべてにカスタムイベントとすべての照明効果をコピーします。
  * **Map Diff:** 譜面のバージョンの比較。 テストプレイやModでどこに変更が加えられたかを見るときに便利です。
* [Parity Checker](https://galaxymaster2.github.io/bs-parity/) by **GalaxyMaster**  
  譜面でパリティの問題を見つけることができるエラーチェッカーツール。
* [Map Check](https://kivalevan.github.io/BeatSaber-MapCheck/) by **Kival Evan**  
  MMA2に組み込まれているものよりも汎用性の高いエラーチェッカーツール。
* [noodleLister](https://github.com/bloodcloak/noodleLister#readme) by **Bloodcloak**  
  BeatSaberの譜面を譜面のキーコマンドが入ったテキストファイルから簡単にプレリストへ変換できます。

#### レガシーツール
これらのツールはサポートされてはいませんが、現行のバージョンと互換性があり特定のケースで役に立つことがあります。

* [BeatMerge](https://github.com/ZelonGames/BeatMerge#readme) by **DarkGrisen**  
  他の譜面作者と一緒に大きなマップをつくるときに音源をきれいに張り合わせる作業を手動で行うのはわずらわしくないですか？ このツールは複数のマップを一つの大きなマップにしてくれます。
* [Cinder](https://github.com/zhaey/cinder#readme) by **zhaey**  
  Phythonで書かれた`.sm`ファイルをBeatSaberの`.dat`ファイルへと変換します。
* [BeatMapper Tools](https://beatmappertools.com/) by **Darkuni**  
  Mediocre MapperやMediocre Mapper Assistant 2のユーザーが簡単に変換や、テストプレイ、zipファイルの作成をすることができるツール.
* [osu! のBPMを調整するためのチュートリアルビデオ](https://www.youtube.com/watch?v=nIX0koHzW8c&t) by **Fayhe**  
  osu!のエディタを用いてBPMを検出する方法を紹介するビデオ

### 便利なMod
ここには譜面作成をすこし楽にするツールがあります。

* [SiraUtil](./basic-lighting.md#in-game-with-fpfc) by **auros**  
  一人称視点操作（FPFC）のパラメータを設定して、キーボードやマウスを使ってゲームのプレイ中に視点操作ができます。 Mod へのリンクや設定方法については、 [Basic Lighting](./basic-lighting.md#in-game-with-fpfc) のセクションを参照してください。
* [PracticePlugin](https://github.com/Kylemc1413/PracticePlugin) by **Kyle1413**  
  再生速度を調整し、ループを作成します。  [Mod Assistant](https://github.com/Assistant/ModAssistant#readme)から最新版をダウンロードできます。
* [ReLoader](https://github.com/Kylemc1413/ReLoader) by **Kyle1413**  
  メニューから再読み込みをせずに練習モードでマップをリロードできます。 ウォールマッピングの際に便利です。

## マッピングの練習
> "ルールを破るには、まずそれを熟知しなければならない。"  
> \- Uninstaller

マッピングの聖書はありませんが、このwikiのセクションには、コミュニティから寄せられたマッピングのあらゆる段階で有益な情報が得られます。 ある程度スキルを身に着けるまではここでのルールを守り、クリエイティブに、試行錯誤を行い、挑戦していきましょう。

### [**基本的なマッピング**](./basic-mapping.md)
これから譜面を作成しようとする人はみなこれを読む必要があります。**例外はありません！**

### [**中級者向けの譜面作成ガイド**](./intermediate-mapping.md)
多くのマッピングトピックを詳細に見る

### [**ダウンマッピング**](./downmapping.md)
より低い難易度を作るための包括的なガイド。

### [**上級者向け譜面作成**](./extended-mapping.md)
Mapping Extensions、追加要素や 360&deg;/90&deg; などの譜面作成方法

### Mapperのロール
[Beat Saber Modding Group Discord](https://discord.gg/beatsabermods)で**Mapper**のロールを獲得するには、3つ以上のプレイ可能なマップ（共同製作も可）をリリースしたうえで [Mapper Role Submission Form](https://forms.gle/mj66J3UopTykFJjXA)のフォームから応募してください。 マップの検証と申請の承認には時間がかかることがあります。

### キュレーション
Mappersは [BeastSaber Discord](https://bsaber.com/getting-started/curation/#donts) の#curation-requestチャンネル に [客観的な問題](https://discord.gg/VJZHUbt)なしで高品質のマップを提出することができます。 キュレーションされたマップは、サイトで優先的に表示され、キュレーター推奨フィードにいれられます。

### Modding & ランキング
ある[Ranking Criteria](https://scoresaber.com/criteria)の条件を満たし、”Moding”と呼ばれる検証と改善が行われた譜面はランク付けされる可能性があります。ランク付けされた譜面はリーダーボードに対応するパフォーマンスポイント(PP)がプレイヤーに与えられます。 より詳細な情報は [ScoreSaber Discord](https://discord.gg/WpuDMwU)にて参照してください。

* ランク付けを申請する前に、マップ作成者はランク付けの基準と [metadata standards](https://docs.google.com/document/d/1ehotupIYMVlc8x41JldO-24m7Am-oTVYnciF9KCRdNM/edit)の基準 を満たし、マップを経験豊富なスタッフに”Moding"される必要があります。

:::tip より詳しい情報 より概念的なランクについては[Ranking Criteria](https://scoresaber.com/criteria) を確認してください。 :::

* マップがModdingを受け、修正されるとランキングチームからの評価へと段階が進みます。
* ランキングチームがマップをランク付けされるにふさわしいと判断した場合、マップに投票が行われます。

### Mapping Anxiety
マップをアップロードすることに不安を感じたり、ダウンロード数が少ないことやダウンボートが多いことが心理的負荷を感じることはよくあることです。 多くのマッパーは、この感情を経験しています。 詳細については、 [不安なマッピングへの対処](./mapping-anxiety.md) ページをご覧ください。

## 照明効果
ライティングをするまでマップは完成していません。 ライティングはとても簡単な方法から追加のModを使うことでより細やかに設定することができます。

### [**基本的な照明効果**](./basic-lighting.md)
様々な側面からマップに照明効果をつけることがわかります。

### [**中級者向けライティング**](./intermediate-lighting.md)
ストロボ、リングスピンやコントラストの調整などのライティングのコツ

### [**高度なライティング**](./advanced-lighting.md)
高度で細やかな技術、カスタムプラットフォーム用の照明効果やChroma RGBについて**(このページは現在作成中です)**

### オートライティング
照明をつける準備ができていませんか？ ここにあなたの代わりにライティングを作成してくれるプログラムを紹介します。 覚えておいてほしいのは、手動でライティングをつけることはそれほど難しくはありません。曲の雰囲気をよりよく表現するにはこれらのプログラム使うより自分で行ったほうが良いことがあります。

* [Lolighter](https://github.com/Loloppe/Lolighter#readme) by **Loloppe#6435** - スタンドアローンで動作するライティング自動生成プログラム。 マップを修正するための機能も備えています。
* [LiteMapper](https://litemapper.net/) by **ItsOrius** - ノーツ配置に基づいて自動的にライトを生成するウェブサイト。 アルゴリズムの詳細については、 [Readme](https://github.com/ItsOrius/LiteMapper#readme) を参照してください。
* **Lightmap** - Mediaocre Map Assistant 2に統合されており、エラーチェックのメニューよりアクセスできます。

## テストプレイ
テストプレイはマッピングの**重要**なプロセスです。 テストプレイにより主要なプレイ感の調整やマップの感触を知ることができます。 [サードパーティーや外部](#community-third-party-testing)でのテストプレイはより建設的な意見がもらえたり自分でプレイしたときにはわからない部分を検証してくれる便利な方法です。

::: danger 注意 テストプレイを行うためにBeatSaverにマップをアップロードする**必要はありません** :::

* マップがバージョン1.0のフォーマットを使用している場合(.jsonと.oggファイル形式) **エディタを更新**しマップを変換しなければいけません。 [コミュニティのエディタ](.#community-editors)を参照してください。
* ver2.0のフォーマット（.dat や.ogg.egg）である場合はもう準備は完了しています。

### PCでテスト
コミュニティエディタで作成されたマップをPCを用いたVRシステムでテストプレイを行うには次の手順に従ってください。

1. WIPソングフォルダが `Beat Saber_Data_CustomWIPLevels` にない場合は、そこにマップのコピーを置きます。
2. ゲーム内のプレイリスト一覧からCustomWIPLevelsに行きます。 練習モードでプレイしてください。（プレイボタンの横のボタンを押してください）

**ゲーム起動中にマップに変更を加えたときは**  
ゲームウィンドウをクリックします。 次に、メインメニューまたは曲の選択画面でキーボードで <kbd>Ctrl + r</kbd> を押します。 ゲームを再起動せずにマップの変更がロードされます！

:::tip 注意点

* You will need to have the **SongCore** mod installed in order to see the CustomWIPLevels category and use the <kbd>Ctrl + r</kbd> shortcut.
* Having duplicate map files in `CustomLevels` and `CustomWIPLevels` can cause problems.
* Using Online Websites to convert audio to `.ogg` may result in your audio file being treated as invalid and will not be loaded by the game! Using Audacity and following the steps in [Basic Audio Setup](./basic-audio.md) is the easiest way to ensure your map loads in-game. :::

### Testing on a Quest
Follow these steps to test any of your maps made with a community editor using an Oculus Quest. You must have [SideQuest](https://sidequestvr.com) and [BMBF](https://bmbf.dev/stable) installed.

1. Locate your WIP song folder on your PC.
2. Establish a connection to your Quest from your PC with a USB cable.
3. Open SideQuest on your PC and click the folder icon on the top right. ![SideQuest Files](~@images/beginners-guide/sqfiles.png)
4. Navigate to `sdcard/ModData/com.beatgames.beatsaber/Mods/SongLoader/CustomWIPLevels`. If this folder does not exist, you can create it yourself.
5. Upload your WIP song folder from your PC to that folder on your Quest with SideQuest.
    * **NOTE:** You need to upload the actual song folder, not a zip file!
6. Your map will now show up on the CustomWIPLevels song pack inside your game. Keep in mind that you will only be able to play your map using the practice mode, and not with the regular Play button!

:::tip NOTE Using Online Websites to convert audio to `.ogg` may result in your audio file being treated as invalid and will not be loaded by the game! Using Audacity and following the steps in [Basic Audio Setup](./basic-audio.md) is the easiest way to ensure your map loads in-game. :::

### Community / Third Party Testing
The `#testplays` channel in the [Beat Saber Modding Group Discord](https://discord.gg/beatsabermods) makes it easy to have your work checked by knowledgeable mappers. Playtesters will provide constructive feedback on how to improve your map in either video or text format in a DM or in the `#mapping-discussion` channel.

:::warning Some things to note...

* Maps with less than 1 minute done will not get much feedback or be tested. Consider asking in `#mapping-discussion` to see if someone will take a look instead.
* Challenge/Super High difficulty maps may take longer to get feedback since there are not many playtesters at this skill level.
* Please keep to serious posts where you are looking to improve your mapping skills. Meme or Shitpost maps do not belong as they end up wasting the testplayers time.
* Make sure you have run your map through a checker program such as those built-in to your editor or external tools like Parity Checker or Map Check in [Additional Mapping Tools](#additional-mapping-tools) :::

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

次のテンプレートをコピー&ペーストしてDiscord内でご利用ください。

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
マッピングが終わり、ライティングをつけ、そしてテストプレイをおこなったら、それは世界にリリースする準備ができている完成した作品です！

### BeatSaver
[BeatSaver](https://beatsaver.com/) はすべてのカスタムマップが公開されています。

#### マップを公開する方法

::: danger 注意

* **完成していない**マップをBeatSaverにアップロードしないでください。
  * Uploading to BeatSaver equates to "Putting it on the store shelf" and should **only** be your final version.
  * See the [Playtesting](#playtesting) section for instructions on testing your map. :::

1. [Create an account](https://beatsaver.com/register) on BeatSaver with a username/password or by logging in via Discord.
    * Beatsaver usernames may only have alphanumeric characters and `-`. Usernames with spaces or `_` for example, are not allowed.
2. Click the <kbd>Upload</kbd> link in the top-right.
3. Add your BeatSaver map name and map description. Only the map name is searchable so be sure to include song name, song artist, and other terms that might make it easier to find your map.
    * Use "tags" like (Chroma), (OneSaber), or (Mapping Extensions) if your map uses some special modifications or characteristics you want to highlight.
    * Putting a link to a playthrough video in the map description can help you get more downloads as it is easier to share your map to others and lets people know what to expect.
4. Add your .zip file and identify whether your map was human-made or AI-assisted.
    * AI maps intentionally uploaded as human-made will be deleted.
5. Maps are initially uploaded to your unpublished tab. You must explicitly publish them to make them available to the public.

::: tip NOTE
Map files can now be updated on BeatSaver!
If you need to upload a new version of your map you must first recall the map to your unpublished tab before you can
upload a new version. This will retain your map key and statistics but will reset all leaderboards.
:::

### BeatSaver Troubleshooting
Here are solutions for some common errors when uploading a Beatmap.  
Encountered something not listed here? Drop into `#mapping-discussion` for assistance.

:::danger Remember:

* You should have your map [playtested](#playtesting) before uploading!
* You do not need upload maps created by auto-generation software such as Deepsaber or Beat Sage to install them in your game. If you are on PC, you can unzip the files into your `CustomLevels` folder. If you are on Quest, follow the [Testing on a Quest](#testing-on-a-quest) steps to install the map. :::

---

#### Map already uploaded

* The exact map files were uploaded previously. You must change something small in your map (i.e., remove a light block, save the map, replace the light block, and save again) to be able to upload.

---

#### _difficultyBeatmapSets[]._difficultyBeatmaps[].`Difficulty.dat`._version``: Must not be null

* You are using an old, outdated editor that is not compliant with the current data schema. See [Community Editors](#community-editors) for the current options.

---

#### Internal Server Error
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

#### Beatmap zip contains an illegal file! OLD

* Usually caused by extra/unsupported files, such as gifs, in the zip.

---

#### Beatmap does not contain an Info.dat file! OLD

* Usually caused by having the files in a subfolder. You need to zip the files instead of the folder. [How to Video](https://streamable.com/u20ci) Or use the handy export button in your editor instead. **NOTE: MMA2's export button does not include contributor images in the zip.**

---

#### One or more beatmap difficulty files cannot be found! OLD

* You might have forgotten to include all of your difficulty files are in the zip.
* A difficulty's `"_beatmapFilename"` in the `Info.dat` might be using a different file name than what is present in the folder.
* A deleted difficulty is still being referenced in your `Info.dat` file. Check to make sure you do not have unintended difficulties in the `"_difficultyBeatmaps"` cluster of each present characteristic.

---

#### Error in `MapDifficulty.dat`. Root should NOT have additional property: `_time`. OLD

`_time` is the common error for this type of message. However, the same solution applies if a different property is flagged.

* Your files are not compliant the map schema. See [Schema Change](#beatsaver-data-schema-change-october-27-2019) for solutions.

---

#### Beatmap could not be parsed! OLD

* This could be caused by extreme server load. Try again later or ask in `#mapping-discussion`.

---

#### Field `._customData._contributors[]._iconPath` contains an invalid filename. OLD

* Utilizing the contributors field requires all aspects to be included. Make sure all 3 aspects (Role, Name, iconPath) are filled and there is a unique square image for each iconPath entry in your zip.

---

### BeastSaber
[BeastSaber](http://www.bsaber.com) is a song review and curation site with social features including reviewing and commenting on songs. All songs published on BeatSaver are mirrored to BeastSaber within 10-15 minutes. Additionally, maps deleted from BeatSaver may take up to a day to be removed from BeastSaber.

## [クレジット](./mapping-credits.md)
Over *thirty* different mapping guides and tutorials have been combined into this wiki so that it can be maintained by the community as a whole. Many many **MANY** thanks to the mappers who blazed this trail and contributed content. Check out the whole list [here!](./mapping-credits.md)
