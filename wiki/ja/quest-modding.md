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
現在、カスタム曲やMODをインストールする唯一の推奨方法は、[パソコンでSideQuestから](#installing-bmbf-with-sidequest)BMBFをロードすることです。

PCを使えない場合は、 [Android端末でModを導入する](/support/modding-with-android.md) を参照してください。 iPhoneやiPadなどのChromebookやiOSデバイスはサポートされていません。

:::warning 警告 BMBFをインストールすると公式のマルチプレイモードや公式のリーダーボードへのスコアの送信、リプレイの記録ができなくなります。 もしModが導入された状態でマルチプレイを行いたい場合は`Beat Together`が必要になります。これはPCとQuestのクロスプレイを可能にします。また、両方とものカスタムソングで遊ぶことができます。 ディスコードの[Beat Saber Modding Group](discord.gg/beatsabermods)の`#quest-mods`チャンネルもしくは[Questboard](https://questmodding.com)のサイトで入手できます。

ランク付けされた曲からパフォーマンスポイント(PP)を得るためには、 [ScoreSaber](https://new.scoresaber.com/quest) modが必要です。 [このリンク](https://new.scoresaber.com/quest) では、 ScoreSaberページに移動して設定する方法が書いてあります。 Scoresaberは公式のリーダーボードを置き換えるものではなく、カスタム曲のリーダーボードだけが追加されます。

**注意** [ScoreSaber Discord](https://discord.gg/WpuDMwU)のサーバーでModが現在のゲームバージョンで使えるかチェックしてください。 :::

### SideQuestでBMBFをインストールする
SideQuestをまだ設定していない場合は、 [SideQuest](https://sidequestvr.com/#/setup-howto) をダウンロードしてセットアップしてください。

**注意:** iOSをお使いの場合は、 `ステップ4:開発者モードを有効にして再起動` の代わりに次の手順に従ってください。

![iOSHowTo](~@images/beginners-guide/EnableDevModeIOS.png)

BMBFを取得するには3つの方法があります。

* [PC上のSideQuestストア](#download-from-the-sidequest-store)
* [BMBFのウェブサイト](#download-the-from-the-bmbf-website)
* PCをお持ちでない場合は、 [AndroidのSideQuestストア](/support/modding-with-android.md) を使用できます。
  * iPhoneやiPadなどのChromebookやiOSデバイスはサポートされていません。 :::tip 以前にModが導入されたBeat Saberやスコアがあれば、 [あらかじめデータをバックアップしてください!](#backup-save-data-using-sidequest) :::

#### SideQuest Storeからダウンロード

1. QuestをPCに接続して、[SideQuestからBMBF](https://sidequestvr.com/app/747)へアクセスします。
2. `Install To Headset` ボタンをクリックします。 (SideQuestを開くというポップが表示されたら開くを押してください。)
3. BMBFがヘッドセットにインストールされるのを待ちます。

インストールが完了したら、ガイドの [BMBFのセットアップ](#bmbf-setup) セクションに進んでください。

#### BMBFのウェブサイトからダウンロード
初めに[BMBF APK](https://bmbf.dev/stable)をパソコンにダウンロードします。

SideQuestを開き、QuestをPCに接続します。

Modが入っている状態なら一度アンインストールする必要があります。上部のワッフルアイコンからSideQuestのアプリタブを開き、BeatSaberの横にある歯車マークから`UNINSTALL APP`ボタンを押します。 Beat Saberをクエストストアからダウンロードすると、ゲームの最新バージョンでModがない状態になります。

`Install APK from folder`ボタンを選択して最新のBMBF apkをみつけダウンロードしてください。もしくはSideQuestにドラッグしてください。 どちらの方法でもBMBFをQuestにインストールできます。

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

ガイドの [BMBF セットアップ](#bmbf-setup) セクションに進んでください。

#### BMBFのセットアップ

BMBFのインストールが完了したら、BMBFがサポートしている最新のBeatSaberがインストールされていて、Modが入っていない事を確認してください。 BSMG Discordの `#modding-announcements` チャンネルや、[QuestBoard](https://www.questmodding.com/) で、対応バージョンやModを確認してください。

:::warning Modを入れる前に、ビートセイバーを一度起動して一つの曲をプレイしてください。そのあとすぐにゲームを終了しても大丈夫です。

現在、マルチユーザー機能を利用している場合、Modは動作しません。 Modを導入する前に一時的にサブアカウントをすべて取り除く必要があります。 希望のModをインストールし終えたらあとで元に戻すことができます。 :::

Beat Saberを一度実行した後、以下の画像のように、unknown sourcesからBMBFを開きます。 ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

開いたら、BMBFの各手順に沿ってModを導入してください。 完了後[QuestBoard](https://www.questmodding.com/)と[BeastSaber](https://www.bsaber.com)がBMBFにアプリとしてロードされます。 そこからすべてのカスタム曲をダウンロードすることができます。 また、BeatSaverボタンをクリックして曲をダウンロードすることもできます。

ゲームの改造に成功すると、 `アプリを復元する` ポップアップが表示されます。 `閉じる` をクリックして下さい

Modを入れた後にBeat Saberを起動しようとすると、アプリの復元を確認するポップアップが再び表示される可能性があります。 そこで アプリを開くを選択します (この時点で閉じるを押すと何も行われません)。 この警告は、海賊版のゲームに向けられているので、Modを導入しているだけの場合無視をしてもほとんど影響はありません。

![RestoreApp](~@images/beginners-guide/restoreapp.png)

引き続き[コアMods](#core-mods)のインストールステップに進んでください。

## 保存データの管理

### SideQuest を使用してセーブデータをバックアップ

SideQuestを開き、QuestをPCに接続します。

SideQuest ファイルエクスプローラを使用して、 `sdcard/Android/data/com.beatgames.beatsaber/files` に移動します。

![SideQuest Files](~@images/beginners-guide/sqfiles.png)

`AvatarData.dat`と`PlayerData.dat` と `settings.cfg` を PC 上のフォルダに保存します。 これらにはあなたのスコアやそのほかのセッティングが含まれているので保管してください。

### SideQuest を使用してセーブデータを復元

データを復元するにはSideQuestを開き、PCに接続します。  
SideQuestのファイルから[サイドクエストを利用したバックアップ](#backup-save-data-using-sidequest)で保存した3つのファイル`AvatarData.dat`、`PlayerData.dat`と`settings.cfg`を`sdcard/Android/data/com.beatgames.beatsaber/files`に入れます

## Modをインストール

### コアMod
追加のMODをインストールする前に、BMBFウェブインターフェースの右上に「`Sync to Beat Saber`」という赤いボタンが表示されています。 これをクリックして同期を完了させます。 BMBFの `mods` タブに移動します。 7つのコアModがあることを確認してください:

* Custom Types
* Codegen
* SongLoader
* Playlist Manager
* QuestUI
* SongDownloader
* PinkCore

:::danger 注意 これらのコアModが無いと他のModは動作しません！

もしリストにModがない場合はBMBFの`Tools`タブの`Reload Mods`と`Check Core Mod Updates`ボタンを押してください。 それでもModが表示されない、もしくは表示されるがゲーム内で動作しない場合はトラブルシューティングの[コアModが動かない場合](#core-mods-don-t-work)を参照してください。 :::

### Quest 内での操作
:::warning すべてのModがQuestBoardで使えるわけではありません!  
もしお探しのModがここで見当たらない場合は [PCを使った方法](#using-your-pc) を代わりにお試しください。 :::

クエストでBMBFを開き、`Browser` タブに移動します。 QuestBoard は自動的に開きます。  
そうでない場合は、`Choose Website` をクリックし、`QuestBoard` ボタンをクリックします。

![globequestboard](~@images/beginners-guide/globequestboard.png)

以下の [QuestBoard](https://www.questmodding.com/) ウェブサイトにアクセスしてください 次に、 `Get Mods` タブを選択します。

![questboardhome](~@images/beginners-guide/questboardhome.png)

ポインタをドラッグして下にスクロールします。 そのリストから任意のModを選択し、その隣のダウンロードボタンを押してダウンロードすることができます。 一部のダウンロードは、ウェブサイトまたはGitHubページにリダイレクトされる場合があります。 その場合は、画面上の指示に従うか、リリースリストで最新の `.qmod` をそれぞれ選択します。

![questboardmods](~@images/beginners-guide/questboardmods.png)

### PCを使った方法
[BSMG Discord](https://discord.com/invite/beatsabermods)の`#quest-mods`チャンネルで他のModを探してインストールすることができます。

:::warning
クエストとPCが同じネットワークに接続されていること、httpsではなくhttpであることを確認してください。
:::

QuestでBMBFを開き、 `Tools` タブに移動します そこにウェブアドレスとバージョン番号が表示されます

![ip](~@images/beginners-guide/ip.png)

お使いの PC でブラウザを開き、検索バーにアドレスを入力します。

以下の画面にアクセスできるはずです。

これがうまくいかない場合は、 [こちら](#bmbf-web-interface-not-loading) をクリックしてトラブルシューティングの手順にしたがってください。

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Quest互換のMODをアップロードボックスにドラッグしてください。 古いバージョン用のModとして作られていた場合、自動的に有効にはなりません。 古いMODを有効にするには、 `Mods` タブに移動し、そこから有効にします。

## 曲のインストール
::: tip
「すべての曲から」「レート」「ダウンロード数」「プレイ数」によってソートできます。 2019年後半から現在の間にリリースされた曲をダウンロードして、最高の
創作譜面を体験してみてください。
:::

### ゲーム内でダウンロードする方法
SongDownloader (コア mod) を使ってゲーム内で曲をダウンロードできるようになりました。 ゲーム内で曲をダウンロードするにはいくつかのステップがあります。

1. Beat Saberを開く
2. メインメニューの左側にある「Mods」パネルを見る
3. SongDownloader タブを開く
4. 曲を検索してダウンロードします。

ゲーム内で曲をダウンロードするときは、ゲームを再起動する必要はありません。 SongLoader を使用して自動的に曲をロードします。

![songdownloader](~@images/beginners-guide/songdownloader.png)

### BMBFからダウンロードする方法
ブラウザを使用してQuest内にカスタム曲を取得するには、2つの方法があります。

* キュレーションされたマップとプレイリストをお探しなら、 [BeastSaber](https://bsaber.com/) をご覧ください。
* BeastSaberのUIが気に入らない場合は、 [BeatSaver](https://beatsaver.com/)を試すこともできます。

どちらにもOneClick™ ボタンがあり、Questにその曲を簡単にインストールできます。 ブラウザウィンドウの右上にある地球儀アイコンを使用して、これらのウェブサイトを切り替えることができます。

`Syncsaber`を使うことで様々な種類の曲を簡単にダウンロードできます。QuestのBMBFから`Syncsaber`というタブをクリックしてください。 ここではボタンをクリックして曲をダウンロードすることができます。様々な設定から選ぶことができます。 例えば[Beatsaver's](https://beatsaver.com/)でのトップ20をダウンロードしたい場合は"hot"を選んでください。もしくは50の最も難しい曲を選ぶこともできます。

また別の方法としては[Beastsaber](https://bsaber.com/)の`Bookmark`という機能を使う方法です。 After creating an account, you can click a little bookmark icon on a song and if you later delete all your songs from the Quest you can redownload the ones that are bookmarked with OneClick™.

### PCを使った方法
Quest内に曲をインストールできない場合は、modのインストールと同様にPCを使用して楽曲をインストールできます。

1. お使いのコンピューターで [BeastSaber](https://bsaber.com/) または [BeatSaver](https://beatsaver.com/) にアクセスしてください。
2. zipファイルをダウンロード
3. [PC を使用して Mod をインストールする](#using-your-pc) の手順に従って、ファイルのアップロード画面を開きます。
4. マップのzipファイルをドラッグアンドドロップするとインストールされます！

これがうまくいかない場合は、 [こちら](#bmbf-web-interface-not-loading) をクリックしてトラブルシューティングの手順に従ってください 。

:::tip プレイリストも同様にダウンロードできます。 You can find various playlists on [BeastSaber](https://bsaber.com/category/playlists/) or various community discords. You can also make your own using [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) or [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

If you want to test a map you have created see the [Testing on a Quest](/mapping/#testing-on-a-quest) Section in the Mapping Wiki section for steps on packing it up for testing! :::

## モデルのインストール
Join the [Qosmetics Community](https://discord.gg/qosmetics) to change how your sabers, bloqs or walls look in-game!

## ダウングレード
[BSMG](https://www.discord.gg/beatsabermods)の`#modding-announcements`チャンネルで最新バージョンがModに対応しているかを確認してください。 If mods are not updated for the latest version, you will need to downgrade to be able to mod.

The easiest method to get to the right version, is to go to the [QuestModding](https://www.questmodding.com/) page, click on How To Downgrade tab, and follow the steps.

With these steps done, you can now start modding your game!

::: tip Something not working? Go to the [BSLG Discord](https://discord.gg/MrwMx5e) for help. :::

## 関連リンク

* [Qosmetics Community](https://discord.gg/qosmetics) - Quest用にセイバー、ノーツ、壁が保存されているサーバー。
* [Qosmetics Creation Guides](https://github.com/RedBrumbler/Qosmetics/wiki) - Quest用に独自のカスタムセイバー、ノーツ、壁を作成するためのガイド。
* [Beat Saber Quest Modding Guide](https://bsqmg.cal117.me/) - Guides on how to create your own mods for Quest.
* [QuestBoard website](https://questmodding.com) - A place to get Beat Saber related news and info along with the latest mods releases!
* [QuestBoard Discord server](https://discord.gg/P7sUKVnP) - A quest community to hangout and talk about Beat Saber related stuff, you can also get a role to get notified when a new mod gets released!
* [Fixing Out of Sync Audio](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber Mod](https://new.scoresaber.com/quest) - Get in-game leaderboards for custom songs
* [ScoreSaber](https://scoresaber.com) - The website to view custom song leaderboards outside of the game.

## トラブルシューティング
:::warning Youtubeのビデオチュートリアルを見たのですが、うまくいかず困っています。 どうすればいいですか？ BSMGは他のチュートリアルを使用しないことを**強く**お勧めします。 多くの場合、それらの情報は古いものであったり、不完全であったり、誤った情報であったりすることがあります。

代わりに、ここで書かれたガイドに従うか、 [BSMG Discord](https://discord.gg/beatsabermods) のヘルプを探してください。 :::

### 起動すると読み込み画面から動きません！
If your Beat Saber is getting 3 dots when launching make sure that:

1. You launched and played one song before modding the game
2. You're not using a pirated version of the game
3. Make sure you're using the latest version of BMBF
4. Make sure you hit done instead of open when installing modded BeatSaber.

> If you did not do these last two, reinstall Beat Saber, and redo the BMBF setup process.

5. Make sure you have allowed Beat Saber permissions, you can check this by pressing the three dots next to beatsaber in the apps section and going into permissions.
6. If you have, try pressing Quick Fix in the Tools tab of BMBF.
7. Make sure you have given it 10-15 seconds to load.

If none of the above work, restart your headset and redo the modding process.

### Adding mods from beatmods.com or models from modelsaber.com does not work
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model qmod use the [BMBF Web Interface](#using-your-pc) to install it.

### Sideloading BMBF failed
When sideloading BMBF and you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Core mods don't work

If you are having problems with core mods, please verify that you are not trying to use any outdated mods. Any mod made for a previous game version is considered outdated. Once you have removed them:

1. Go to `Tools`
2. Click `Delete Mods`
3. Click `Sync to Beat Saber`

If you had mods installed before this, turn them off then on again to reinstall them.

---

### BMBF web interface not loading
If your BMBF Web Interface is not loading, Make sure you are typing the ip from the tools tab in the quest into your browser. If it still does not load, make sure you are doing the following:

* BMBF is open in the headset
* There is http:// at the beginning of the link, not https://
* You have :50000 at the end of your link
* Your pc and your quest are on the same Wifi
* Your ip hasn't changed, as it changes from time to time
* Your ip is not 127.0.0.1 If none of these work restart your quest and try them all again

---

### BMBF not loading configuration after a few minutes
This is likely due to using BMBF on a game version it was not built for. Such as using BMBF for Beat Saber version `1.13.0` when the version of the game installed on the headset is `1.12.2`.  
If the game version matches what the BMBF release page says its built for, try restarting your headset. If it still does not work use the [BMBF Web Interface](#using-your-pc) and click `Quick Fix` in the Tools tab.

---

### セイバーとModが有効になりません！
This is most likely due to having an outdated BMBF App, grab the latest [BMBF Release](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* If your level doesn't load then try installing mapping extensions from #quest-mods. It may also require the mod Noodle Extensions which isn't on Quest yet.
* If your BMBF is on the latest version and mods wont be enabled in game, uninstall Beat Saber with the uninstall BS button in the BMBF Tools tab then reinstall and remod.
* In very very very rare cases, BMBF does not have file permissions to copy mods into the right location. Check in SideQuest to make sure BMBF has file permissions.

---

### Beat Saber がクラッシュした
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### BMBFを開くと白い画面が表示されます
If you only see a white screen when you open BMBF from unknown sources, try waiting a few seconds. If that does not work, restart your quest and try opening BMBF again.
