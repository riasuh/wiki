---
sidebar: auto
---

# Quest Modding

## はじめに

* refer to the [original English version](../quest-modding.md),
* wait for a translation to be done,

::: danger Sorry, this page has not been translated yet, you can either:

* 初期設定（バニラ）には存在しない問題が発生する可能性があります。 99.9％のバグ、クラッシュや遅延はModによるものです。
* Modはゲームのアップデートによって動かなくなる可能性がありますが、普通のことです。このようなことが起きた場合は忍耐強く、敬意をもって待ちましょう。Mod作成者はボランティアです。
* Beat Gamesは、意図的にMODを破壊しようとはしていません。 コードベースで動作することを想定しているので、Modを壊すこともありますが、Modを排除しようとはしません。

Modに関連する問題でゲーム開発者を非難しないでください。 ただのクレーマーになってはいけません。 :::

:::warning Elite Ericのビデオを見ましたが、動かなくなりました。 いったい何が起こったのでしょうか。 BSMGはElite Ericによるチュートリアルを使用しないことを**強く**お勧めします。 多くの場合、それらは 時代遅れであるか、不完全で誤った、正しくない情報が含まれていることがわかります。

代わりに、ここで書かれたガイドに従うか、 [BSMG Discord](https://discord.gg/beatsabermods) のヘルプを探してください。（いくつかの日本語サイトも古い情報を含んでいるので注意してください） :::

## インストール
現在、カスタム曲やMODをインストールする唯一の推奨方法は、SideQuestでBMBFをロードすることです。

PCにアクセスできない場合は、 [Android Phone](#installing-bmbf-with-an-android-phone) を使用できます。

* [BMBF apk](https://bmbf.dev/stable) :::warning BMBFをインストールしModを導入するとゲーム公式のマルチプレイ、リプレイの視聴、公式のリーダーボードへの更新ができなくなります。 もしModが導入された状態でマルチプレイを行いたい場合は`Beat Together`が必要になります。これはPCとQuestのクロスプレイを可能にします。また、両方とものカスタムソングで遊ぶことができます。 Modは、 #quest-mods `または` Questboard [サイトの Beat Saber](https://questmodding.com) Modding Group にあります。

ランク付けされた曲からパフォーマンスポイント(PP)を得るためには、 [ScoreSaber](https://new.scoresaber.com/quest) modが必要です。 [このリンク](https://new.scoresaber.com/quest) では、 ScoreSaberページに移動して設定する方法が書いてあります。 Scoresaberはベースのゲームのリーダーボードを置き換えるものではなく、カスタム曲のリーダーボードだけが追加されます。

**注意** [ScoreSaber Discord](https://discord.gg/WpuDMwU)のサーバーでModが現在のゲームバージョンで使えるかチェックしてください。 :::

### SideQuestでBMBFをインストールする
まだ設定していない場合は、 [SideQuest](https://sidequestvr.com/#/setup-howto) をダウンロードしてセットアップしてください。

SideQuestを開き、QuestをPCに接続します。

:::tip 以前にModが導入されたBeat Saberやスコアがあれば、バックアップしたいスコアがあれば、 [最初にデータの保存をバックアップしてください!](#backup-save-data-using-sidequest) :::

Modが導入されているのであればそれらも`UNINSTALL APP`ボタンからアンインストールする必要があります。 Mod導入後、同じメニューから復元できます。

Select the 以下に示す`Install APK from folder`ボタンを選択して最新のBMBF apkをみつけダウンロードしてください。もしくはSideQuestにドラッグしてください。 そのどちらの方法でもBMBFをクエストにインストールできます。

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

正常にインストールされたら、最新バージョンの Beat Saber がインストールされており、Modがないことを確認してください。

:::warning Modを入れる前に、ビートセイバーを一度起動して一つの曲をプレイしてください。すぐに失敗しても大丈夫です。

現在実験的なマルチユーザー機能が搭載されている場合じゃModを導入できません。 Modを導入する前に一時的にサブアカウントをすべて取り除く必要があります。 希望のModをインストールし終えたらあとで元に戻すことができます。 :::

Beat Saberを一度実行した後、以下の写真のように、unknown sourcesからBMBFを開きます。 ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

言われたとおりにそれぞれのステップを実行してください。 それから、 [bsaber.com](https://www.bsaber.com) を見つけてください。 そこで利用可能な任意のカスタム曲をダウンロードすることができます。 右上にある地球儀アイコンをクリックして、ビートセーバーに曲をダウンロードすることもできます。

インストールプロセス中に `Restore App` ポップアップが表示されることがありますが、そのときは `Close` をクリックしてください。 この警告は、海賊版のゲームに向けられているので、Modを導入しているだけの場合無視をしてもほとんど影響はありません。

![RestoreApp](~@images/beginners-guide/restoreapp.png)

引き続き[コアMod](#core-mods)のインストールステップに進んでください。

### Android端末でBMBFをインストールする
これは BMBFをインストールする**推奨方法でありません**、PCにアクセスできない場合にのみ使用してください。

* [準備するもの](#requirements)
* [携帯電話のセットアップ](#setup-your-phone)
* [Android端末でBMBFをインストールする](#installing-bmbf-with-your-phone)
* [Beat Saberのセットアップ](#setup-beat-saber)

#### 準備するもの

* アンドロイド携帯もしくはタブレット（iPhoneやiPadはサポートされていません）
* Oculus Quest Storeで**支払いが完了**したBeat Saber
* クエストを携帯につなげるケーブル（もし携帯がタイプCの充電方式であればクエストでも機能するでしょう）

#### 携帯電話のセットアップ

1. [bugjaeger app](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)をGoogleストアからダウンロードします。
2. 最新の[BMBF APK from bmbf.dev/stable](https://bmbf.dev/stable)をダウンロードします。
3. この[ガイド](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ)を参考にクエストで開発者モードを実行できるようにしてください。
4. 開発者モードを有効にする。
    1. アンドロイドの設定をひらく
    2. 機器の設定を開く
    3. ソフトウエアの情報をタップ
    4. ビルド番号をタップして開発者モードを有効にします 7回タップします
5. USBであなたの携帯に接続します。
    1. 設定に戻ります
    2. 開発者オプションをタップ
    3. USBのデバッグを有効にします

#### Android端末でBMBFをインストールする
:::warning Modを入れる前に、ビートセイバーを一度起動して一つの曲をプレイしてください。すぐに失敗しても大丈夫です。 :::

bugjaegerを携帯で起動します。その後クエストと接続します。 クエストと携帯でUSBのデバッグのポップが表示されます 両方のデバイスで許可を選択してください。 クエストがbugjaegerを認識したら、以下のようにBMBFをインストールしてください。

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

「OK」を選択して`com.weloveoculus.BMBF.apk`とラベルが付いたダウンロードされたAPKへのアクセスを許可します。 apkファイルがクエストにインストールされます。

#### Beat Saberのセットアップ
BMBFを正常にインストールし終えたらクエスト内のライブラリ内に未知のソースとしてファイルを見つけることができます。

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

それを起動するとファイルへのアクセス許可を促すポップが表示されます 画面上の指示に従ってください。 終わったら、 [BeastSaber](https://bsaber.com) を見てください

インストールプロセス中に Restore App ポップアップが表示されることがありますが、そのときは Close をクリックしてください。 この警告は海賊版を防止するために表示されるものなので、正規版を購入している場合は無視をしてもかまいません。

引き続き[Core Mods](#core-mods)のインストールステップに進んでください。

## 保存データの管理

### SideQuest を使用して保存データをバックアップ

SideQuestを開き、QuestをPCに接続します。 ウィンドウの上部バーにある `My App` に移動し、Beat Saberを探します。

SideQuest ファイルエクスプローラを使用して、 `sdcard/Android/data/com.beatgames.beatsaber/files` に移動します。

`AvatarData.dat`と`PlayerData.dat` と `settings.cfg` を PC 上のフォルダに保存します。 これらにはあなたのスコアやそのほかのセッティングが含まれているのでなくさないでください。

### SideQuest を使用して保存データをバックアップ

データを復元するには、SideQuestを開き、クエストをPCに接続します。 ウィンドウの上部バーにある `My App` に移動し、Beat Saberを探します。 SideQuestのファイルエクスプローラーを使用して、[SideQuest を使用して保存データをバックアップ](#backup-save-data-using-sidequest)で保存した`AvatarData.dat`と`PlayerData.dat`、 `settings.cfg`の3つのファイルを`sdcard/Android/data/com.beatgames.beatsaber/files`に保存してください。

その後、メニューに戻り、最新のバックアップの横にある円形の矢印を押します。 スコアと設定が復元されます。

## Modをインストール

### Core mod
追加のMODをインストールする前に、BMBFウェブインターフェースの右上を見てください 。`Beat Saberと同期`と書かれた赤いボタンが表示されます。 これをクリックして同期を完了させます。 BMBFの `mods` タブに移動します。 5つのコアModがあることを確認してください:

* Codegen
* Goodbye bug
* PinkCore
* QuestUI
* Custom Types

:::danger これらのコアModがインストールされていなかったり有効になっていない場合、他のModは動作しません。

コアMODのいずれかが有効になっていない場合は、そのModを削除し、再度 `Sync to Beat Saber` をクリックして再度ダウンロードしてください。 ダウンロードして有効になっているかどうかを再確認してください。 それでも動かない場合（Modが有効になっているにもかかわらず）トラブルシューティングの[コアModが動かない場合](#core-mods-don-t-work)を参照してください。 :::

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

:::warning クエストとPCが同じネットワークに接続されていること、httpsではなくhttpであることを確認してください。 :::

QuestでBMBFを開き、 `Tools` タブに移動します そこにウェブアドレスとバージョン番号が表示されます

![ip](~@images/beginners-guide/ip.png)

お使いの PC でブラウザを開き、検索バーにアドレスを入力します。

以下の画面にアクセスできるはずです。

これがうまくいかない場合は、 [こちら](#bmbf-web-interface-not-loading) をクリックしてトラブルシューティングの手順にしたがってください。

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Quest互換のMODをアップロードボックスにドラッグしてください。 古いバージョン用のModとして作られていた場合、自動的に有効にはなりません。 古いMODを有効にするには、 `Mods` タブに移動し、そこから有効にします。

## 曲のインストール
::: tip 「すべての曲から」「レート」「ダウンロード数」「プレイ数」によってソートできます。 2019年後半から今の間にリリースされた曲をダウンロードして、最高の 創作譜面を体験してみてください。 :::

### Quest 内での操作
ブラウザーウィンドウを使用してQuest内にカスタムマップを取得するには、2つのソースがあります。

* キュレーションされたマップとプレイリストをお探しなら、 [BeastSaber](https://bsaber.com/) をご覧ください。
* BeastSaberのUIが気に入らない場合は、 [BeatSaver](https://beatsaver.com/)を試すこともできます。

どちらにもOneClick™ ボタンがあり、Questにその曲を簡単にインストールできます。 ブラウザウィンドウの右上にある地球儀アイコンを使用して、これらのウェブサイトを切り替えることができます。

様々な種類の曲を簡単にダウンロードする方法は`Syncsaber`を使うことです。クエストのBMBFにアクセスして`Syncsaber`というタブをクリックしてください。 ここではボタンをクリックして曲をダウンロードすることができます。様々な設定から選ぶことができます。 例えば[Beatsaver's](https://beatsaver.com/)でのトップ20をダウンロードしたい場合は"hot"を選んでください。もしくは50の最も難しい曲を選ぶこともできます。

また別の方法としては[Beastsaber](https://bsaber.com/)の`Bookmark`という機能を使う方法です。 アカウントの作成後、曲についている小さいブックマークをクリックすると、もしのちにクエストからすべての曲を削除した後ブックマークからOneClick™で再ダウンロードすることもできます。

### PCを使った方法
Quest内で曲をインストールできない場合は、modのインストールと同様にコンピュータを使用してマップをインストールできます。

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
* [Fixing Out of Sync Audio](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - カスタム曲のゲーム内ランキング

## トラブルシューティング
:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

### Adding mods from beatmods.com or models from modelsaber.com does not work
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model zip use the [BMBF Web Interface](#using-your-pc) to install it.

### Sideloading BMBF failed
When sideloading BMBF you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Core Mod が起動しません

Core Mod に問題がある場合は、古いModを使用していないかを確認してください。 以前のバージョンで作成されたModはすべて古いModとして認識されます。 一度それらを削除した後に

1. `Tools`に移動します。
2. `exit BMBF`をクリックします
3. BMBFをもう一度開きます
4. `Tools`に移動します。
5. `Quick fix`をクリックします
6. BMBF アプリの `ブラウザー` セクションに移動します。
7. 右上隅の小さな地球儀アイコンをクリックします
8. `QuestBoard`をクリックします
9. `Modのダウンロード` をクリックします。
10. 下にスクロールし、 `すべてのコア Modをダウンロード` をクリックします
11. `Sync to Beat Saberをクリック`

---

### BMBF Web インターフェイスが読み込まれていません
If your BMBF Web Interface is not loading, be sure that you're typing the IP from the tools tab into your browser on your computer that's on the same network. Make sure that:

1. Your IP is not `127.0.0.1`, if that shows up try rebooting your headset and/or router.
2. BMBF is open in the headset
3. There is `http://` at the beginning of the link, not `https://`
4. You have `:50000` at the end of your link
5. Your PC and Quest are on the same wifi network
6. Your IP is hasn't changed as it changes from time to time

If none of these work, restart your Quest and go through the list again.

---

### BMBF not loading configuration after a few minutes
This is likely due to using BMBF on a game version it was not built for. Such as using BMBF for Beat Saber version `1.13.0` when the version of the game installed on the headset is `1.12.2`.  
If the game version matches what the BMBF release page says its built for, try restarting your headset. If it still does not work use the [BMBF Web Interface](#using-your-pc) and click `Quick Fix` in the Tools tab.

### Beat Saber is black when I launch it
Open the library on your Quest. Click the three dots next to Beat Saber and then click `Permissions`. In the menu that pops up, enable storage permissions and try launching the game again.

---

### My Sabers and Mods wont enable/work
This is most likely due to having an outdated BMBF App, grab the latest [BMBF Release](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* If your mod is supposed to be compatible with your version of BMBF, then make sure there is no folder separating the contents of the .zip file.
* If your level doesn't load then try installing mapping extensions from #quest-mods. It may also require the mod Noodle Extensions which isn't on Quest yet.
* If your BMBF is on the latest version and mods wont be enabled in game, uninstall Beat Saber with the uninstall BS button in the BMBF Tools tab then reinstall and remod.
* In very very very rare cases, BMBF does not have file permissions to copy mods into the right location. Check in SideQuest to make sure BMBF has file permissions.

---

### Beat Saber is crashing
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### I only see a white screen when i open BMBF
If you only see a white screen when you open BMBF from unknown sources, restart your quest and then it should be fixed

### 起動すると読み込み画面から動きません！
起動したときに読み込み画面から動かない場合は以下のことを確認してください。

1. Modを入れる前にゲームを一度起動し、曲を最低一曲はプレイした
2. 海賊版のゲームを使用していない
3. 最新バージョンのBMBFを使用している
