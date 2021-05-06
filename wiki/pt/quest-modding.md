---
sidebar: auto
---

# Quest Modding

## Prefácio

* Esse guia é para ambos Quest 1 e Quest 2.
* Ninguém ainda foi banido por modding.

::: danger AVISO Ao escolher usar mods, você entende que:

* Você deve experienciar problemas que não existem com o game vanilla. 99.9% dos bugs, crashes, e lag são pelos mods.
* Os mods estão sujeitos a falhas por causa de atualizações e isso é normal - sê paciente e respeitoso quando isso acontecer, porque os modders são voluntários com vidas reais.
* Os Beat games não estão propositadamente a tentar acabar com os mods. Eles querem trabalhar no código fonte e às vezes isso quebra os mods, mas não estão tentando matar os mods.

Não ataque os devs por problemas relacionados a mods, e vice versa - modders e devs são dois grupos separados. Só não seja um idiota ok. :::

:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Instalação
Currently the only recommended way to install custom songs and mods is BMBF sideloaded with SideQuest using a PC.

If you do not have access to a PC you can use an [Android Phone](#installing-bmbf-with-an-android-phone).

* [BMBF apk](https://bmbf.dev/stable) :::warning Instalar o BMBF e instalar mods ao seu jogo desativará o Multiplayer oficial, assim como ver e enviar scores para os placares base do jogo. If you would like to play modded multiplayer, you need the mod, `Beat Together`, which allows for cross-play between pc and quest and allows for custom songs to be used if all parties own said song. O mod pode ser encontrado no Beat Saber Modding Group em `#quest-mods` ou no site [Questboard](https://questmodding.com).

To get leaderboards on custom songs and to be able to get Performance Points (PP) from ranked songs you need the [ScoreSaber](https://new.scoresaber.com/quest) mod. [This link](https://new.scoresaber.com/quest) will take you to the ScoreSaber page to set it up. ScoreSaber does not replace the base game leaderboards, it only adds leaderboards for custom songs.

**Note:** Check the updates channel in the [ScoreSaber discord](https://discord.gg/WpuDMwU) to see if the mod is available for the current game version. :::

### Instalando o BMBF com o SideQuest
If you haven't already, download and setup [SideQuest](https://sidequestvr.com/#/setup-howto)

Open SideQuest and connect your Quest to your PC.

:::tip If you've previously modded Beat Saber or have scores you want to backup, [Backup your Save Data first!](#backup-save-data-using-sidequest) :::

If you have a modded game you also need to uninstall it by pressing the `UNINSTALL APP` button. You can later restore your save from the same menu, after modding.

Select the `Install APK from folder` button shown below and find the latest BMBF apk you downloaded and click on it, or simply drag the BMBF apk into SideQuest. Either method will install BMBF to your Quest.

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

Once it has been successfully installed, make sure you have the latest version of Beat Saber installed and unmodded.

:::warning Before modding, run Beat Saber once, play a level and immediately fail!

Modding currently does not work if the experimental multi-user feature is in use. You will need to temporarily remove all secondary accounts before modding the game. You can add them back later once you have installed your desired mods. :::

After running Beat Saber once, open BMBF from unknown sources as the picture below shows. ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

Follow each step exactly as you're told. Then, you should see [bsaber.com](https://www.bsaber.com). This is where you can download any custom songs available. You can also click on the globe icon in the top right and go to beatsaver to download songs too.

If at any point during the install process, you get the `Restore App` popup just click `Close`. This warning is more directed to pirated versions of the game so if you're just modding there will likely be no consequences for ignoring it.

![RestoreApp](~@images/beginners-guide/restoreapp.png)

Continue to the [Core Mods](#core-mods) step of the installation process.

### Instalando BMBF com um celular Android
This is **NOT** the recommended way to install BMBF and should only be used if you do not have access to a PC.

* [Requisitos](#requirements)
* [Configurando o seu Celular](#setup-your-phone)
* [Instalando BMBF com seu celular Android](#installing-bmbf-with-your-phone)
* [Configurando o Beat Saber](#setup-beat-saber)

#### Requisitos

* An Android Phone or Android Tablet (IPhones or IPads are not supported)
* A **paid** Version of Beat Saber on the Oculus Quest Store
* A Cable to connect your Quest to your Phone (If your phone charges over USB C the charger that was included with your Quest should work)

#### Setup your Phone

1. Download the [bugjaeger app from the Google Play store](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)
2. Download the newest [BMBF APK from bmbf.dev/stable](https://bmbf.dev/stable)
3. Follow [this written guide](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ) to Enable Developer Mode on your Quest.
4. Enable Developer mode on your Phone
    1. Go into your Android settings
    2. Scroll to "About phone" and open it
    3. Tap "Software information"
    4. Tap the "Build number" field until it says Developer mode enabled. This should take about 7 taps.
5. Enable USB debugging on your Phone
    1. Go back to settings
    2. Tap "Developer options"
    3. Activate USB debugging

#### Installing BMBF with your Phone
:::warning Before modding, run Beat Saber once, play a level and immediately fail! :::

Open bugjaeger on your Phone and connect your Quest. You should get a USB debugging pop-up in your Quest and on your phone. Select allow on both devices and if you prefer, select always allow. Once bugjaeger picks your Quest up, install the BMBF APK by doing following:

![installAPKusingPhone.png](~@images/beginners-guide/InstallAPK.png)

After you pressed ok, allow file access and select the download APK file which should be labeled `com.weloveoculus.BMBF.apk`. The apk file should now install to your Quest.

#### Setup Beat Saber
After successfully installing BMBF onto your Quest you should be able to find it in your Quests library under unknown sources.

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

Open it and allow file access after starting it if prompted. Now follow the on-screen instructions carefully. After you finished you should see [BeastSaber](https://bsaber.com).

If at any point during the install process, you get the Restore App popup just click Close. This warning is directed to pirated versions of the game so there will likely be no consequences for ignoring it if you have a legitimate copy.

Now you can continue to the [Core Mods](#core-mods) step of the installation process.

## Gerenciar Dados Salvos

### Fazer backup de seus dados salvos usando o SideQuest

Open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber.

Navigate to `sdcard/Android/data/com.beatgames.beatsaber/files` using the SideQuest file explorer.

Save the files: `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` into a folder on your PC. Do not lose these, as they contain your scores and other settings!

### Restaurando seus dados salvos usando o SideQuest

To restore your data, open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber. Using the SideQuest file explorer take the 3 files you saved from the [Backup Save Data using SideQuest](#backup-save-data-using-sidequest) steps `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` and put them in the `sdcard/Android/data/com.beatgames.beatsaber/files` folder.

Go back to the menu and press the circular arrows located beside your latest backup. Your scores and settings should now be restored.

## Instalando mods

### Core Mods
Before installing any additional mods look in the top right of the BMBF web interface, you should see a red button that says, `Sync to Beat Saber`. Click this and let it finish syncing. Then go to your `mods` tab in BMBF. Make sure that you have the 5 core mods:

* Codegen
* Goodbye bug
* PinkCore
* QuestUI
* Custom Types

:::danger All other mods will not work if these core mods are not listed and enabled.

If one of the core mods does not enable, delete that mod and click `Sync to Beat Saber` again to redownload it. Double check to see if it has been downloaded and enabled. If it still doesn't work, or mods are appear to be enabled, but not working in-game see [Core Mods don't work](#core-mods-don-t-work) for troubleshooting steps. :::

### Dentro de seu Quest
:::warning Not all mods are available on QuestBoard!  
If a mod is not seen in here, you should follow the [Using Your PC](#using-your-pc) method instead. :::

Open BMBF in your Quest and go to the `Browser` tab, there you should see a globe icon similar to what's shown below. Click it, then click the `QuestBoard` button.

![globequestboard](~@images/beginners-guide/globequestboard.png)

You should be greeted with the [QuestBoard](https://www.questmodding.com/) website below. Next, select the `DOWNLOAD MODS` tab.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Scroll down with your thumbsticks. You can now select any mod from the list, seen below, and download it by hitting the download button next to it. Some downloads may redirect you to a website or GitHub page. If so, follow the instructions onscreen, or select the latest `.zip` in the Releases list, respectively.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Usando seu PC
You can find and download other Quest mods from the [BSMG Discord](https://discord.com/invite/beatsabermods) in the `#quest-mods` channel.

:::warning Make sure your Quest and PC are on the same network and that you are using http and not https! :::

Open BMBF in your Quest and go to the `Tools` tab, there you should see a web address and a version number similar to what's shown below.

![ip](~@images/beginners-guide/ip.png)

On your PC, open your browser and type the address into the search bar.

You should be greeted with this screen below.

If this doesn't work [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Now just drag any Quest compatible mods into the upload box and sync. If the mod was originally made for an older version, then it won't automatically enable. To enable an old mod, go to the `Mods` tab and enable it from there.

## Instalando músicas
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

### Inside your Quest
There are 2 sources to getting custom maps inside your Quest using the browser window.

* Se você estiver procurando por mapas curated e playlists visite o [BeastSaber](https://bsaber.com/)
* Se você não gosta da UI do BeastSaber, você também pode tentar o [BeatSaver](https://beatsaver.com/)

Both have a OneClick™ button that easily installs that song onto your Quest. You can switch between these websites using the globe icon in the top right of the browser window.

An easy way to download different kinds of songs is to use `Syncsaber` you can access it by going into BMBF on your quest and clicking the tab called `Syncsaber`. Here you can download songs with a click of a button, you can choose from different "settings". For example you can download the top 20 songs in [Beatsaver's](https://beatsaver.com/) "hot" section or the 50 hardest ranked songs.

Another method is using the `Bookmark` feature on [Beastsaber](https://bsaber.com/). After creating an account you can click a little bookmark icon on a song and if you later delete all your songs from the Quest you can redownload the ones that are bookmarked with OneClick™.

### Usando seu PC
If you are unable to install songs inside your Quest, you can install maps using your computer similar to installing mods.

1. Visite o [BeastSaber](https://bsaber.com/) ou o [BeatSaver](https://beatsaver.com/) no seu computador
2. Baixe o zip
3. Siga os pasos do [Instalando mods](#using-your-pc) em cima da tela de envio de arquivos.
4. Arraste e solte o arquivo zip do mapa aqui e ele deve ser instalado!

If the web interface doesn't load [click here](#bmbf-web-interface-not-loading) for some troubleshooting steps.

:::tip You can also download playlists in the same way. You can find various playlists on [Beastsaber](https://bsaber.com/category/playlists/) or various community discords. You can also make your own using [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) or [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

If you want to test a map you have created see the [Testing on a Quest](/mapping/#testing-on-a-quest) Section in the Mapping Wiki section for steps on packing it up for testing! :::

## Instalando modelos
Join the [Qosmetics Community](https://discord.gg/qosmetics) to change how your menu title, sabers, bloqs or walls look in-game!

## Links Úteis

* [Qosmetics Community](https://discord.gg/qosmetics) - Servidor dedicado à criação e uso de sabres, blocos e paredes para o Quest.
* [Qosmetics Creation Guides](https://github.com/RedBrumbler/Qosmetics/wiki) - Guias para criar seus próprios custom sabers, blocos, e paredes para Quest.
* [Questboard website](https://questmodding.com) - A place to get Beat Saber related news and info along with the latest mods releases!
* [Questboard discord server](https://discord.gg/P7sUKVnP) - A quest community to hangout and talk about Beat Saber related stuff, you can also get a role to get notified when a new mod gets released!
* [Corrigindo o Áudio Fora de Sincronia](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - Placares in-game para músicas custom

## Solução de problemas
:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

### Adicionar mods do beatmods.com ou modelos do modelsaber.com não funciona
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model zip use the [BMBF Web Interface](#using-your-pc) to install it.

### Fazer o sideload do BMBF falhou
When sideloading BMBF you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Core mods não funcionam

If you are having problems with core mods, please verify that you are not trying to use any outdated mods. Any mod made for a previous game version is considered outdated. Once you have removed them:

1. Vá para `Tools`
2. Clique em `exit BMBF`
3. Abra o BMBF novamente
4. Vá para `Tools` novamente
5. Clique em `Quick fix`
6. Vá para a seção `Browser` do aplicativo BMBF.
7. Clique no ícone do pequeno globo no canto superior direito
8. Clique em `QuestBoard`
9. Clique em `Downloads Mods`
10. Role para baixo e clique em `Download All Core Mods`
11. Clique em `Sync to Beat Saber`

---

### A interface web do BMBF não está carregando
If your BMBF Web Interface is not loading, be sure that you're typing the IP from the tools tab into your browser on your computer that's on the same network. Make sure that:

1. Seu IP não é `127.0.0.1`, se isso aparecer tente reiniciar seu headset e/ou roteador.
2. BMBF está aberto em seu headset
3. Há `http://` no início do link, e não `https://`
4. Você tem `:50000` no final do seu link
5. Seu PC e Quest estão na mesma rede wifi
6. Seu IP ainda é o mesmo que pode mudar de vez em quando

If none of these work, restart your Quest and go through the list again.

---

### BMBF não carregando as configurações depois de alguns minutos
This is likely due to using BMBF on a game version it was not built for. Such as using BMBF for Beat Saber version `1.13.0` when the version of the game installed on the headset is `1.12.2`.  
If the game version matches what the BMBF release page says its built for, try restarting your headset. If it still does not work use the [BMBF Web Interface](#using-your-pc) and click `Quick Fix` in the Tools tab.

### Beat Saber está preto quando abro
Open the library on your Quest. Click the three dots next to Beat Saber and then click `Permissions`. In the menu that pops up, enable storage permissions and try launching the game again.

---

### Meus sabres e mods não ativam/funcionam
This is most likely due to having an outdated BMBF App, grab the latest [BMBF Release](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* Se o seu mod é suposto ser compativel com a sua versão do BMBF, em seguida, verifique se não há nenhuma pasta que separe o conteúdo do arquivo .zip.
* Se seu level não carregar, tente instalar o mapping extensions do #quest-mods. Eles também podem precisar do mod Noodle Extensions no qual não está no Quest ainda.
* Se o seu BMBF estiver na versão mais recente e os mods não forem ativados no jogo, desinstale o Beat Saber com o botão de uninstall BS na aba Tools do BMBF então reinstale e instale os mods novamente.
* Em casos muito muito raros, o BMBF não tem permissão de copiar mods no local certo. Verifique no SideQuest para certificar-se que o BMBF tenha permissões de arquivo.

---

### Beat Saber is crashing
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### I only see a white screen when i open BMBF
If you only see a white screen when you open BMBF from unknown sources, restart your quest and then it should be fixed

### Meu Beat Saber tem 3 pontos quando eu abro
If your Beat Saber is getting 3 dots when launching make sure that:

1. Você abriu e jogou uma música antes de modificar o jogo
2. Você não está usando uma versão pirata do jogo
3. Certifique-se de estar usando a versão mais recente do BMBF
