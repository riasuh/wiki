---
sidebar: auto
---

# Quest Modding

## はじめに

* このガイドはQuest1とQuest2のためのものです。
* 今までModによってBANされたことはありません。

::: danger 注意 しっかりと理解してからModを利用しましょう

* 初期設定（バニラ）には存在しない問題が発生する可能性があります。 99.9％のバグ、クラッシュや遅延はModによるものです。
* Modはゲームのアップデートによって動かなくなる可能性がありますが、普通のことです。このようなことが起きた場合は忍耐強く、敬意をもって待ちましょう。Mod作成者はボランティアです。
* Beat Gamesは、意図的にMODを破壊しようとはしていません。 コードベースで動作することを想定しているので、Modを壊すこともありますが、Modを排除しようとはしません。

Modに関連する問題でゲーム開発者を非難しないでください。 ただのクレーマーになってはいけません。 :::

:::warning Youtubeのビデオチュートリアルを見たのですが、うまくいかず困っています。 どうすればいいですか？ BSMGでは、改造のためにビデオチュートリアルを使用しないことを**強く**お勧めします。 多くの場合、それらの情報は古いものであったり、不完全であったり、誤った情報であったりすることがあります。

代わりに、ここで書かれたガイドに従うか、 [BSMG Discord](https://discord.gg/beatsabermods) のヘルプを探してください。（いくつかの日本語サイトも古い情報を含んでいるので注意してください） :::

## インストール
現在、カスタム曲やMODをインストールする唯一の推奨方法は、SideQuestでBMBFをロードすることです。

PCにアクセスできない場合は、 [Android Phone](#installing-bmbf-with-an-android-phone) を使用できます。

* [BMBF apk](https://bmbf.dev/stable) :::warning　警告 BMBFをインストールしModを導入するとゲーム公式のマルチプレイ、リプレイの視聴、公式のリーダーボードへの更新ができなくなります。 もしModが導入された状態でマルチプレイを行いたい場合は`Beat Together`が必要になります。これはPCとQuestのクロスプレイを可能にします。また、両方とものカスタムソングで遊ぶことができます。 Modは、 #quest-mods `または` Questboard [サイトの Beat Saber](https://questmodding.com) Modding Group にあります。

ランク付けされた曲からパフォーマンスポイント(PP)を得るためには、 [ScoreSaber](https://new.scoresaber.com/quest) modが必要です。 [このリンク](https://new.scoresaber.com/quest) では、 ScoreSaberページに移動して設定する方法が書いてあります。 Scoresaberはベースのゲームのリーダーボードを置き換えるものではなく、カスタム曲のリーダーボードだけが追加されます。

**注意** [ScoreSaber Discord](https://discord.gg/WpuDMwU)のサーバーでModが現在のゲームバージョンで使えるかチェックしてください。 :::

### SideQuestでBMBFをインストールする
まだ設定していない場合は、 [SideQuest](https://sidequestvr.com/#/setup-howto) をダウンロードしてセットアップしてください。

SideQuestを開き、QuestをPCに接続します。

:::tip 以前にModが導入されたBeat Saberやスコアがあれば、バックアップしたいスコアがあれば、 [最初にデータの保存をバックアップしてください!](#backup-save-data-using-sidequest) :::

Modが導入されているのであればそれらも`UNINSTALL APP`ボタンからアンインストールする必要があります。 Mod導入後、同じメニューから復元できます。

Select the 以下に示す`Install APK from folder`ボタンを選択して最新のBMBF apkをみつけダウンロードしてください。もしくはSideQuestにドラッグしてください。 そのどちらの方法でもBMBFをクエストにインストールできます。

![APKのインストール](~@images/beginners-guide/apkfromfolder.png)

正常にインストールされたら、最新バージョンの Beat Saber がインストールされており、Modがないことを確認してください。

:::warning Modを入れる前に、Beat Saberを一度起動し、任意の曲を一回プレイしてください。すぐに失敗しても大丈夫です。

現状、マルチユーザー機能を利用している場合、Modは動作しません。 Modを導入する前に一時的にサブアカウントをすべて削除する必要があります。 希望のModをインストールし終えたらあとで元に戻すことができます。 :::

Beat Saberを一度実行した後、以下の写真のように、unknown sources(提供元不明) からBMBFを開きます。 ![UnknownSourced](~@images/beginners-guide/quest_home-menu.jpg)

開いたら、BMBFの各手順に沿ってゲームの改造を進めてください。 完了すると、BMBFアプリの [Bsaber.com](https://www.bsaber.com) が表示されます。 そこで利用可能な任意のカスタム曲をダウンロードすることができます。 右上にある地球儀アイコンをクリックして、ビートセーバーに曲をダウンロードすることもできます。

インストールプロセス中に `Restore App` ポップアップが表示されることがありますが、そのときは `Close` をクリックしてください。 この警告は海賊版ゲームに向けられたものなので、Modを導入しているだけの場合は、無視してもほとんど影響はありません。

![RestoreApp](~@images/beginners-guide/restoreapp.png)

引き続き[コアMod](#core-mods)のインストールステップに進んでください。

### Android端末でBMBFをインストールする
この BMBFをインストールする方法は**推奨方法ではないため**、PCにアクセスできない場合にのみ使用してください。

* [準備するもの](#requirements)
* [携帯電話のセットアップ](#setup-your-phone)
* [Android端末でBMBFをインストールする](#installing-bmbf-with-your-phone)
* [Beat Saberのセットアップ](#setup-beat-saber)

#### 準備するもの

* Android携帯もしくはタブレット（iPhoneやiPadはサポートされていません）
* Oculus Quest Storeで**支払いが完了**したBeat Saber
* クエストを携帯につなげるケーブル（もし携帯がタイプCの充電方式であればクエストでも機能するでしょう）

#### 携帯電話のセットアップ

1. [Bugjaeger app](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)をGoogleストアからダウンロードします。
2. 最新の[BMBF APK from bmbf.dev/stable](https://bmbf.dev/stable)をダウンロードします。
3. この[ガイド](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ)を参考にクエストで開発者モードを実行できるようにしてください。
4. 開発者モードを有効にする。
    1. Androidの設定をひらく
    2. 機器の設定を開く
    3. ソフトウエアの情報をタップ
    4. ビルド番号をタップして開発者モードを有効にします 7回タップします
5. USBであなたの携帯に接続します。
    1. 設定に戻ります
    2. 開発者オプションをタップ
    3. USBのデバッグを有効にします

#### Android端末でBMBFをインストールする
:::warning Modを入れる前にBeatSaberを一度起動し、任意の曲を一回プレイしてください。すぐに失敗しても大丈夫です。 :::

Bugjaegerを携帯で起動します。その後クエストと接続します。 Questと携帯電電話に、USBデバッグのポップアップが表示されます。 両方のデバイスで許可を選択してください。 クエストがBugjaegerを認識したら、以下のようにBMBFをインストールしてください。

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

「OK」を選択して`com.weloveoculus.BMBF.apk`とラベルが付いたダウンロードされたAPKへのアクセスを許可します。 apkファイルがQuestにインストールされます。

#### Beat Saberのセットアップ
BMBFを正常にインストールし終えたら、クエストのライブラリ内に提供元不明としてアプリを見つけることができます。

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

それを起動するとファイルへのアクセス許可を促すポップが表示されます 画面上の指示に従ってください。 終わったら、 [BeastSaber](https://bsaber.com) を見てください

インストールプロセス中に `Restore App` ポップアップが表示されることがありますが、そのときは `Close` をクリックしてください。 この警告は海賊版を防止するために表示されるものなので、正規版を購入している場合は無視をしてもかまいません。

引き続き[Core Mods](#core-mods)のインストールステップに進んでください。

## 保存データの管理

### SideQuest を使用して保存データをバックアップ

SideQuestを開き、QuestをPCに接続します。 ウィンドウの上部バーにある `My App` に移動し、Beat Saberを探します。

SideQuest ファイルエクスプローラを使用して、 `sdcard/Android/data/com.beatgames.beatsaber/files` に移動します。

`AvatarData.dat`と`PlayerData.dat` と `settings.cfg` を PC 上のフォルダに保存します。 ここにはあなたのスコアやその他設定が含まれているので、なくさないようにしてください。

### SideQuest を使用して保存データを復元

データを復元するには、SideQuestを開き、クエストをPCに接続します。 ウィンドウの上部バーにある `My App` に移動し、Beat Saberを探します。 SideQuestのファイルエクスプローラーを使用し、「[SideQuest を使用して保存データをバックアップ](#backup-save-data-using-sidequest)」で保存した`AvatarData.dat`、`PlayerData.dat`、 `settings.cfg`の3つのファイルを、`sdcard/Android/data/com.beatgames.beatsaber/files`フォルダに保存してください。

その後、メニューに戻り、最新のバックアップの横にある円形の矢印を押します。 スコアと設定が復元されます。

## Modをインストール

### Core mod
追加のMODをインストールする前に、BMBFウェブインターフェースの右上に「`Sync to Beat Saber`」という赤いボタンが表示されているはずです。 これをクリックして同期を完了させます。 BMBFの `mods` タブに移動します。 5つのコアModがあることを確認してください:

* Codegen
* Goodbye bug
* PinkCore
* QuestUI
* Custom Types

:::danger これらのコアModがインストールされていなかったり有効になっていない場合、他のModは動作しません。

コアMODのいずれかが有効になっていない場合は、そのModを削除し、再度 `Sync to Beat Saber` をクリックして再度ダウンロードしてください。 ダウンロードして有効になっているかどうかを再確認してください。 それでも動かない場合（Modが有効になっているにもかかわらず）トラブルシューティングの[Core Mod が起動しません](#core-mods-don-t-work)を参照してください。 :::

### Quest 内での操作
:::warning QuestBoardにあるすべてのModが使えるわけではありません!  
もしお探しのModがここで見当たらない場合は [PCを使った方法](#using-your-pc) を代わりにお試しください。 :::

QuestでBMBFを開き、 `Browser` タブに移動します。そこには、下図のような地球儀のアイコンが表示されます。 クリックして `QuestBoard` ボタンをクリックします。

![globequestboard](~@images/beginners-guide/globequestboard.png)

以下の [QuestBoard](https://www.questmodding.com/) ウェブサイトにアクセスしてください 次に、 `MOWNLOAD MODS` タブを選択します。

![questboardhome](~@images/beginners-guide/questboardhome.png)

スティックを使って下にスクロールします。 そのリストから任意のModを選択し、その隣のダウンロードボタンを押してダウンロードすることができます。 一部のダウンロードは、ウェブサイトまたはGitHubページにリダイレクトされる場合があります。 その場合は、画面上の指示に従うか、リリースリストで最新の `.zip` をそれぞれ選択します。

![questboardmods](~@images/beginners-guide/questboardmods.png)

### PCを使った方法
[BSMG Discord](https://discord.com/invite/beatsabermods)の`#quest-mods`チャンネルで他のModを探してインストールすることができます。

:::warning 警告 クエストとPCが同じネットワークに接続されていること、httpsではなくhttpであることを確認してください。 :::

QuestでBMBFを開き、 `Tools` タブに移動します そこにウェブアドレスとバージョン番号が表示されます

![ip](~@images/beginners-guide/ip.png)

お使いの PC でブラウザを開き、検索バーにアドレスを入力します。

以下の画面にアクセスできるはずです。

これがうまくいかない場合は、 [こちら](#bmbf-web-interface-not-loading) をクリックしてトラブルシューティングの手順にしたがってください。

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

あとは、Questに対応したMODをアップロードボックスにドラッグして同期するだけです。 もともと古いバージョン用に作られたMODの場合は、自動的に有効にはなりません。 古いMODを有効にするには、 `Mods` タブに移動し、そこから有効にします。

## 曲のインストール
::: tip 「すべての曲から」「レート」「ダウンロード数」「プレイ数」によってソートできます。 最高のカスタム曲を体験するために、2019年後半から今までに作成された譜面をダウンロードしてみてください。 :::

### Quest 内での操作
ブラウザーウィンドを使用してQuest内にカスタム曲を取得するには、2つのソースがあります。

* キュレーションされたマップとプレイリストをお探しなら、 [BeastSaber](https://bsaber.com/) をご覧ください。
* BeastSaberのUIが気に入らない場合は、 [BeatSaver](https://beatsaver.com/)を試すこともできます。

どちらにもOneClick™ ボタンがあり、Questにその曲を簡単にインストールできます。 ブラウザウィンドウの右上にある地球儀アイコンを使用して、これらのウェブサイトを切り替えることができます。

様々な種類の曲を簡単にダウンロードする方法は`Syncsaber`を使うことです。クエストのBMBFにアクセスして`Syncsaber`というタブをクリックしてください。 ここではボタンをクリックするだけで曲をダウンロードすることができ、様々な「設定」から選ぶことができます。 例えば[Beatsaver's](https://beatsaver.com/)でのトップ20をダウンロードしたい場合は"hot"を選んでください。もしくは50の最も難しい曲を選ぶこともできます。

また別の方法としては[Beastsaber](https://bsaber.com/)の`Bookmark`という機能を使う方法です。 アカウントを作成した後、曲についている小さいブックマークをクリックすると、もし後でQuestからすべての曲を削除した場合でも、OneClick™でブックマークされている曲を再ダウンロードすることができます。

### PCを使った方法
Quest内に曲をインストールできない場合は、modのインストールと同様にPCを使用して楽曲をインストールできます。

1. お使いのコンピューターで [BeastSaber](https://bsaber.com/) または [BeatSaver](https://beatsaver.com/) をご覧ください
2. zipファイルをダウンロード
3. [PC を使用して Mod をインストールする](#using-your-pc) の手順に従って、ファイルのアップロード画面を開きます。
4. マップのzipファイルをドラッグアンドドロップするとインストールされます！

これでウェブがうまく動かない場合は [こちら](#bmbf-web-interface-not-loading) をクリックしてトラブルシューティングの手順にしたがってください。

:::tip プレイリストも同様にダウンロードできます。 様々なプレイリストが[Beastsaber](https://bsaber.com/category/playlists/)やディスコードのチャンネルで見つけることができます。 また、 [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager)や[Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/)を使って自分自身だけのプレイリストを作ることもできます。

:::tip 作成したマップをテストしたい場合は、 [Questでテスト](/mapping/#testing-on-a-quest) の譜面作成セクション内の「テスト用」セクションを参照してください。 :::

## モデルのインストール
[Qosmetics Community](https://discord.gg/qosmetics) に参加して、メニューのタイトル、セイバー、ブロック、壁の見た目をゲーム内で変えましょう！

## 役に立つリンク

* [Qosmetics Community](https://discord.gg/qosmetics) - Quest用にセイバー、ブロック、壁が保存されているサーバー。
* [Qosmetics Creation Guides](https://github.com/RedBrumbler/Qosmetics/wiki) - クエスト用に独自のカスタムセイバー、ブロックス、壁を作成するためのガイド。
* [Questboard website](https://questmodding.com) - Beat Saber関連のニュースや最新の modsリリースの情報など！
* [Questboard discord server](https://discord.gg/P7sUKVnP) - BeatSaberのクエストに関係する情報があります。またModがリリースされたときに通知を受けることもできます。
* [オーディオ同期ズレの修正](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - カスタム曲のゲーム内ランキング

## トラブルシューティング
:::warning YouTubeのビデオチュートリアルを視聴して手順を試しましたが、うまく動作しません。 どうすればいいですか？ BSMGは他のチュートリアルを使用しないことを**強く**お勧めします。 多くの場合、それらのビデオは情報が古い・不完全、もしくは誤った情報が含まれています。

代わりに、ここで書かれたガイドに従うか、 [BSMG Discord](https://discord.gg/beatsabermods) のヘルプを探してください。 :::

### beatmods.comまたはmodelsaber.comから手に入れたmodsが動きません。
[BeatMods](https://beatmods.com/) や [ModelSaber](https://modelsaber.com/) のMODが動作しないのはそれらがPC用であるからです。

Questに互換性のあるModは [Questboard](https://www.questmodding.com/) かBeat Saber Moddingのディスコードチャンネル`#quest-mods`から、セイバー、ブロック、壁は[Qosmetics Community](https://discord.gg/qosmetics)から入手してください。 ModまたはモデルのZIPを取得したら、 [BMBF Webインターフェイス](#using-your-pc) を使用してインストールします。

### BMBFのサイドローディングに失敗しました
BMBFをサイドローディングするとエラーが表示されます `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF signatures do not match the previously installed version; ignoring!`

QuestでBMBFバージョンをアンインストールする必要があります。 SideQuestの `My Apps` メニューから行うことができます。

### Core Mod が起動しません

Core Mod に問題がある場合は、古いModを使用していないかを確認してください。 以前のバージョンで作成されたModはすべて古いModとして認識されます。 一度それらを削除し、下記手順を試行してください。

1. `Tools`に移動します。
2. `exit BMBF`をクリックします
3. BMBFをもう一度開きます
4. `Tools`に移動します。
5. `Quick fix`をクリックします
6. BMBF アプリの `ブラウザー` セクションに移動します。
7. 右上隅の小さな地球儀アイコンをクリックします
8. `QuestBoard`をクリックします
9. `Download Mods` をクリックします。
10. 下にスクロールし、 `Download All Core Mods` をクリックします
11. `Sync to Beat Saberをクリック`

---

### BMBF Web インターフェイスが読み込まれていません
BMBF Web インターフェイスが読み込まれていない場合 同じネットワークにあるコンピューターのブラウザにツールタブからIPアドレスを入力していることを確認してください。 下記の順番で確認を行ってください。

1. 以下を確認してください: 1) IPアドレスが `127.0.0.1`ではない場合、ヘッドセットやルーターを再起動してみてください。
2. ヘッドセット内でBMBFを起動している
3. リンクの先頭に `http://` があり、 `https://` ではない
4. リンクの最後に `:50000` があります
5. PCとクエストは同じWi-Fiネットワーク上にあります
6. IPアドレスは時々変更されていない

これらのいずれも確認して動かない場合は、Questを再起動し、リストを再度確認してください。

---

### BMBFが数分間、設定を読み込みません
これはBMBFが対応していないゲームバージョンでBMBFを使用したことが原因と考えられます。 例えばバージョン `1.13.0`用のBMBFをバージョン`1.12.2`のBeatSaberがインストールされたヘッドセットで起動するような場合です。  
もしリリースページで言われているゲームバージョンとBMBFの対応するバージョンが一致する場合は再起動してください。 それでも動作しない場合は、 [BMBF Web インターフェイス](#using-your-pc) を使用し、ツール タブの `Quick Fix` をクリックします。

### Beat Saberが起動時にブラックアウトします。
Questでライブラリを開きます。 Beat Saberの隣にある3つの点をクリックし、 `Permissions`をクリックします。 表示されるメニューで、ストレージのアクセス許可を有効にして、ゲームを再起動してみてください。

---

### SaberとModが有効になりません！
これは、BMBFアプリが古いことが原因である可能性が高いため、最新の [BMBFリリース](https://bmbf.dev/stable)を入手してください。 適切なBeat SaberのBMBFバージョンがない場合は、BMBFが更新されるまでしばらくお待ちください。

* あなたのMODがBMBFのバージョンと互換性があるはずの場合。 zipファイルを区切るフォルダがないことを確認してください。
* カスタム曲がロードされない場合は、#quest-mods からmapping extensionsをインストールしてみてください. Noodle ExtensionsというModを要求されることがありますがこれはまだQuestには実装されていません。
* あなたのBMBFが最新バージョンで、ゲーム内でMODが有効になっていない場合 BMBF ToolsタブのUninstall BSボタンでBeat Saberをアンインストールし、再インストールしてリモートします。
* 非常に非常に非常にまれなケースですが、BMBF には Mod を適切な場所にコピーする権限が与えられていないことがあります。 SideQuest にチェックインして、BMBFにファイルのアクセス許可があることを確認してください。

---

### Beat Saber がクラッシュした
Modをひとつひとつ無効にしてチェックしてください。それでも問題が解決しない場合はDiscordのサポートチャンネルにお問い合わせください。

### BMBFを開くと白い画面が表示されます
不明なソースからBMBFを開いたときに白い画面が表示された場合は、Questを再起動する必要があります。

### 起動すると読み込み画面から動きません！
起動したときに読み込み画面から動かない場合は以下のことを確認してください。

1. Modを入れる前にゲームを一度起動し、曲を最低一曲はプレイした
2. 海賊版のゲームを使用していない
3. 最新バージョンのBMBFを使用している
