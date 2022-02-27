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

:::warning Eu assisti este vídeo no YouTube, mas fiquei preso e/ou não funcionou. Por que isso? Nós do BSMG **fortemente** sugerimos não usar qualquer tutorial do YouTube para modding. Muitas vezes, achamos que eles estão desatualizados ou contêm informações incompletas ou até mesmo completamente erradas.

Em vez disso, você deve seguir os guias escritos aqui na wiki ou procurar ajuda no [Discord do BSMG](https://discord.gg/beatsabermods). :::

## Instalação
Atualmente a única maneira recomendada de instalar músicas customs e mods é pelo BMBF sideloaded com o [SideQuest usando um PC](#installing-bmbf-with-sidequest).

Se você não tem acesso a um PC você pode usar um [Celular Android](/support/modding-with-android.md). Chromebooks e dispositivos iOS como iPhones ou iPads não são suportados.

BMBF apk:::warning Instalar o BMBF e instalar mods ao seu jogo desativará o Multiplayer oficial, assim como ver e enviar scores para os placares base do jogo. Se você gostaria de jogar multiplayer modded, você precisa do mod, `Beat Together`, que permite cross-play entre pc e quest e permite que custom songs sejam usadas. O mod pode ser encontrado no [Beat Saber Modding Group](discord.gg/beatsabermods) em `#quest-mods` ou no site [Questboard](https://questmodding.com).

Para obter rankings em custom songs e ser capaz de obter Pontos de Performance (PP) de músicas ranqueadas você precisa do mod [ScoreSaber](https://new.scoresaber.com/quest). [Este link](https://new.scoresaber.com/quest) vai te levar à página de ScoreSaber para configurá-lo. O ScoreSaber não substitui o ranking base do jogo, apenas adiciona rankings para custom songs.

**Nota:** Confira o chat de atualizações do [Discord do ScoreSaber](https://discord.gg/WpuDMwU) para ver se o mod está disponível para a versão atual do jogo. :::

### Instalando o BMBF com o SideQuest
Se você ainda não fez, baixe e configure o [SideQuest](https://sidequestvr.com/#/setup-howto).

Existem três métodos disponíveis para obter o BMBF:

* [A Loja do SideQuest no PC](#download-from-the-sidequest-store)
* [O site do BMBF](#download-the-from-the-bmbf-website)
* Se você não tem um PC, você pode usar [a Loja do SideQuest no Android](/support/modding-with-android.md) como um último recurso
  * Chromebooks e dispositivos iOS como iPhones ou iPads não são suportados. :::tip Se você modificou anteriormente o Beat Saber ou tem pontuações que você quer fazer o backup, [faça backup dos seus dados salvos primeiro!](#backup-save-data-using-sidequest) :::

#### Baixando pela Loja do SideQuest

1. Conecte seu Quest em seu PC, então vá para o [BMBF No SideQuest](https://sidequestvr.com/app/747).
2. Clique o botão `Install To Headset`. (Aceite a solicitação para abrir o SideQuest quando aparecer.)
3. Espere até que o BMBF termine de instalar em seu headset.

Uma vez instalado, pule para a seção [BMBF Setup](#bmbf-setup) do guia.

#### Baixe o BMBF de seu site
Primeiro baixe o [APK DO BMBF](https://bmbf.dev/stable) no seu PC.

Abra o SideQuest e conecte seu Quest em seu PC.

Se você tem um jogo com mods, você também precisa desinstalá-lo pressionando o botão `UNINSTALL APP`. Você pode restaurar seu save do mesmo menu, depois de instalar os mods.

Selecione o botão `Install APK from folder` mostrado abaixo e encontre a versão mais recente do BMBF que você baixou e clique nele, ou simplesmente arraste o apk do BMBF para o SideQuest. Qualquer outro método irá instalar o BMBF em seu Quest.

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

Você pode continuar para a seção de [Setup do BMBF](#bmbf-setup) do guia.

#### Setup do BMBF

Once BMBF has been successfully installed, make sure you have the latest supported version of Beat Saber installed and unmodded. Check the BSMG `#modding-announcements` channel or [QuestBoard](https://www.questmodding.com/) to see which game version this is and for other modding news.

:::warning Antes de instalar os mods, abra o Beat Saber uma vez, jogue um level e falhe imediatamente!

O modding atualmente não funciona se o recurso experimental multi-user estiver em uso. Você precisará remover temporariamente todas as contas secundárias antes de instalar mods no jogo. Você pode adicioná-los de volta depois de ter instalado os mods desejados. :::

Depois de executar o Beat Saber uma vez, abra o BMBF do unknown sources como mostra a imagem abaixo. ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

Uma vez aberto, siga cada passo do BMBF exatamente como dito para instalar mods no seu jogo. Uma vez concluído, você deve ver o [QuestBoard](https://www.questmodding.com/) com [BeastSaber](https://www.bsaber.com) carregado dentro do aplicativo do BMBF. Aqui é onde você pode baixar qualquer custom song disponivel. Você também pode clicar no botão BeatSaver para baixar músicas também.

Se em algum momento durante o processo de instalação, você ver um pop-up com `Restore App` escrito, apenas clique em `Close`. Este aviso é mais direcionado para versões pirateadas do jogo, então se você está apenas instalando mods, provavelmente não terá consequências por ignorar.

![RestoreApp](~@images/beginners-guide/restoreapp.png)

Continue no passo [Core Mods](#core-mods) do processo de instalação.

## Gerenciar Dados Salvos

### Fazer backup de seus dados salvos usando o SideQuest

Abra o SideQuest e conecte seu Quest em seu PC.

Navegue até `sdcard/Android/data/com.beatgames.beatsaber/arquivos` usando o explorador de arquivo do SideQuest.

![SideQuest Files](~@images/beginners-guide/sqfiles.png)

Salve os arquivos: `AvatarData.dat`, `PlayerData.dat` e `settings.cfg` em uma pasta no seu PC. Não perca estas, pois eles contêm seus scores e outras configurações!

### Restaurando seus dados salvos usando o SideQuest

Para restaurar seus dados, abra SideQuest e conecte seu Quest ao seu PC.  
Usando o explorador de arquivo SideQuest, tire os 3 arquivos que você salvou dos passos [Dados de backup salvos usando o SideQuest](#backup-save-data-using-sidequest) selecione o `AvatarData.dat`, `PlayerData.dat` e `settings.cfg` e coloque-os na pasta `sdcard/Android/data/com.beatgames.beatsaber/files`.

## Instalando mods

### Core Mods
Antes de instalar qualquer modificação adicional no canto superior direito da interface web do BMBF, você deve ver um botão vermelho que diz: `Sync to Beat Saber`. Clique aqui e deixe terminar a sincronização. Então vá para a guia de `mods` no BMBF. Certifique-se de que você tem os 7 core mods:

* Custom Types
* Codegen
* SongLoader
* Playlist Manager
* QuestUI
* SongDownloader
* PinkCore

:::danger Outros mods não funcionarão sem estes Core Mods!

Se algum desses mods não estiver listado, tente o botão de reinstalação na aba `Tools` dentro do BMBF. Se ele ainda não aparecer, ou mods aparecerem mas não funcionarem dentro do jogo, veja [Core Mods não funcionam](#core-mods-don-t-work) para etapas de solução de problemas. :::

### Dentro de seu Quest
:::warning Nem todos os mods estão disponíveis no QuestBoard!  
Se um mod não estiver aqui, você deve seguir o método [Usando Seu PC](#using-your-pc) no lugar. :::

Abra o BMBF em seu Quest e vá para a aba `Browser`. O site do QuestBoard deve abrir automaticamente.  
Se não, clique em `Choose Website` no canto superior direito e, em seguida, clique no botão `QuestBoard`.

![globequestboard](~@images/beginners-guide/globequestboard.png)

Você deve ser cumprimentado com o site [QuestBoard](https://www.questmodding.com/) abaixo. Em seguida, selecione a aba `Get Mods`.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Role para baixo clicando e arrastando o ponteiro. Agora você pode selecionar qualquer mod da lista, visto abaixo, e baixá-lo pressionando o botão de download ao lado dele. Alguns downloads podem redirecionar você para um site ou página do GitHub. Se for o caso, siga as instruções na tela, ou selecione a versão do `.qmod` mais nova na lista de Releases, respectivamente.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Usando seu PC
Você pode encontrar e baixar outros mods de Quest no [Discord do BSMG](https://discord.com/invite/beatsabermods) no canal de `#quest-mods`.

:::warning Certifique-se de que seu Quest e PC estão na mesma rede e que você está usando http e não https! :::

Abra o BMBF em seu Quest e vá para a aba `Tools`, lá você deve ver um endereço web e um número de versão semelhante ao que é mostrado abaixo.

![ip](~@images/beginners-guide/ip.png)

Em seu PC, abra seu navegador e digite o endereço em sua barra de pesquisa.

Você deve ser cumprimentado com essa tela abaixo.

Se isso não funcionar [clique aqui](#bmbf-web-interface-not-loading) para alguns passos de solução de problemas.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Agora arraste todos os mods compatíveis com o Quest para a caixa de envio e sincronize. Se o mod foi feito originalmente para uma versão mais antiga, então ele não vai ser automaticamente ativado. Para habilitar um mod antigo, vá para a aba `Mods` e habilite-o a partir daí.

## Instalando músicas
::: tip A maioria dos mapas "Top Todos", "Rating", "Downloads" ou "Plays" foram criados antes das boas práticas de mapeamento serem estabelecidas. Experimente baixar músicas liberadas entre o final de 2019 e agora para obter a melhor experiência de custom levels. :::

### In-Game
Agora você pode baixar músicas no jogo usando o SongDownloader (core mod) Existem alguns passos para baixar músicas no jogo:

1. Abra o Beat Saber
2. On the main menu, look at the Mods screen, on the left.
3. Abra a aba do SongDownloader
4. Procure por uma música e baixe-a.

Ao baixar músicas no jogo, você não precisa reiniciar o jogo. Isso irá carregar a música automaticamente usando o SongLoader. ![songdownloader](~@images/beginners-guide/songdownloader.png)

### Dentro do BMBF
Existem 2 fontes para obter mapas custom dentro de seu Quest usando a janela do navegador.

* Se você estiver procurando por mapas curated e playlists visite o [BeastSaber](https://bsaber.com/)
* Se você não gosta da UI do BeastSaber, você também pode tentar o [BeatSaver](https://beatsaver.com/)

Ambos têm um botão 1click que facilmente instala músicas em seu Quest. Você pode alternar entre estes sites usando o ícone global no canto superior direito da janela do navegador.

Uma maneira fácil de baixar diferentes tipos de músicas é usar o `SyncSaber`, que você pode acessar indo no BMBF em seu Quest e clicando na aba chamada `SyncSaber`. Aqui, você pode baixar músicas com um clique de um botão escolhendo entre diferentes "configurações". Por exemplo, você pode baixar as top 20 músicas do [BeatSaver na seção "hot"](https://beatsaver.com/) ou as 50 músicas rankeadas mais difíceis.

Outro método é usar o recurso `Bookmark` no [BeastSaber](https://bsaber.com/). Depois de criar uma conta, você pode clicar no pequeno ícone de favorito em uma música e, se mais tarde você excluir todas as suas músicas do Quest, você pode baixar novamente os que estão marcados com o OneClick™.

### Usando seu PC
Se você não conseguir instalar músicas dentro de seu Quest, você pode instalar mapas usando seu computador similarmente a instalar mods.

1. Visite o [BeastSaber](https://bsaber.com/) ou o [BeatSaver](https://beatsaver.com/) no seu computador
2. Baixe o zip
3. Siga os pasos do [Instalando mods](#using-your-pc) em cima da tela de envio de arquivos.
4. Arraste e solte o arquivo zip do mapa aqui e ele deve ser instalado!

Se a interface web não funcionar [clique aqui](#bmbf-web-interface-not-loading) para alguns passos de solução de problemas.

:::tip Você também pode baixar as playlists da mesma maneira. Você pode encontrar várias playlists no [BeastSaber](https://bsaber.com/category/playlists/) ou várias comunidades do discord. Você pode cria sua própria usando o [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) ou [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

Se você deseja testar um mapa que criou veja na seção [Testando no Quest](/mapping/#testing-on-a-quest) na Wiki de Mapping para etapas para preparar-lo para ser testado! :::

## Instalando modelos
Junte-se à [Comunidade do Qosmetics](https://discord.gg/qosmetics) para mudar seu titulo do menu, sabres, blocos ou como suas paredes são no jogo!

## Links Úteis

* [Qosmetics Community](https://discord.gg/qosmetics) - Servidor dedicado à criação e uso de sabres, blocos e paredes para o Quest.
* [Qosmetics Creation Guides](https://github.com/RedBrumbler/Qosmetics/wiki) - Guias para criar seus próprios custom sabers, blocos, e paredes para Quest.
* [Site do QuestBoard](https://questmodding.com) - Um lugar para obter notícias e informações relacionadas à Beat Saber junto com as mais recentes versões de mods!
* [Servidor do Discord do QuestBoard](https://discord.gg/P7sUKVnP) - Uma comunidade de quest para relaxar e falar sobre coisas relacionadas a Beat Saber, você também pode receber um cargo para ser notificado quando um novo mod é lançado!
* [Corrigindo o Áudio Fora de Sincronia](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - Placares in-game para músicas custom
* [ScoreSaber](https://scoresaber.com) - O site para ver o placar de músicas personalizado fora do jogo.

## Solução de problemas
:::warning Eu assisti este vídeo no YouTube, mas fiquei preso e/ou não funcionou. Por que isso? Nós do BSMG **fortemente** sugerimos não usar qualquer tutorial do YouTube para modding. Muitas vezes, achamos que eles estão desatualizados ou contêm informações incompletas ou até mesmo completamente erradas.

Em vez disso, você deve seguir os guias escritos aqui na wiki ou procurar ajuda no [Discord do BSMG](https://discord.gg/beatsabermods). :::

### Adicionar mods do beatmods.com ou modelos do modelsaber.com não funciona
A razão pela qual adicionar mods do [BeatMods](https://beatmods.com/) ou modelos do [ModelSaber](https://modelsaber.com/) não funciona, é porque esses mods e sabres são somente para PC.

Obtenha Mods compatíveis com o Quest no [Questboard](https://www.questmodding.com/) ou `#quest-mods` no Discord do Beat Saber Modding Group, com sabres compativeis com o Quest, blocos, e paredes na [Comunidade do Qosmetics](https://discord.gg/qosmetics). Depois de ter seu mod zip use a [Interface Web do BMBF](#using-your-pc) para instalá-lo.

### Fazer o sideload do BMBF falhou
Quando estiver fazendo sideload do BMBF você pode ver o erro `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF signatures do not match the previously installed version; ignoring!`

Você precisará desinstalar a versão do BMBF de seu Quest. Você pode fazer isso no menu `My Apps` no SideQuest.

### Core mods não funcionam

Se você está tendo problemas com os core mods, verifique se você não está tentando usar nenhum mod desatualizado. Qualquer mod feito para uma versão anterior de jogo é considerado desatualizado. Depois de removê-los:

1. Vá para `Tools`
2. Clique em `Delete Mods`
3. Clique em `Sync to Beat Saber`

Se você tinha mods instalados antes disso, desative-os e instale novamente.

---

### A interface web do BMBF não está carregando
Se a sua Interface Web BMBF não estiver carregando, certifique-se de que você está digitando o IP da guia ferramentas no seu navegador no seu computador que está na mesma rede. Certifique-se de que:

1. Seu IP não é `127.0.0.1`, se isso aparecer tente reiniciar seu headset e/ou roteador.
2. BMBF está aberto em seu headset
3. Há `http://` no início do link, e não `https://`
4. Você tem `:50000` no final do seu link
5. Seu PC e Quest estão na mesma rede wifi
6. Seu IP ainda é o mesmo que pode mudar de vez em quando

Se nada disso funcionar, reinicie seu Quest e siga a lista novamente.

---

### BMBF não carregando as configurações depois de alguns minutos
Isso provavelmente deve ser por usar o BMBF em uma versão do jogo no qual ele não foi feito para. Tal como usar BMBF para o Beat Saber versão `1.13.0` quando a versão do jogo instalado no headset for `1.12.2`.  
Se a versão do jogo corresponde ao que a página de lançamentos do BMBF diz, tente reiniciar o seu headset. Se ela ainda não funciona, use a [Interface Web do BMBF](#using-your-pc) e clique em `Quick Fix` na aba Tools.

### Beat Saber está preto quando abro
Abra a biblioteca em seu Quest. Clique nos três pontos ao lado do Beat Saber e, em seguida, clique em `Permissões`. No menu que aparece, habilite as permissões de armazenamento e tente iniciar o jogo novamente.

---

### Meus sabres e mods não ativam/funcionam
Isso é muito provável que você tenha um cliente BMBF desatualizado, pegue a última versão do [BMBF](https://bmbf.dev/stable). Se a versão do BMBF do seu Beat Saber não estiver ali, por favor espere um pouco para que os unicórnios atualizem o BMBF.

* Se seu level não carregar, tente instalar o mapping extensions do #quest-mods. Eles também podem precisar do mod Noodle Extensions no qual não está no Quest ainda.
* Se o seu BMBF estiver na versão mais recente e os mods não forem ativados no jogo, desinstale o Beat Saber com o botão de uninstall BS na aba Tools do BMBF então reinstale e instale os mods novamente.
* Em casos muito muito raros, o BMBF não tem permissão de copiar mods no local certo. Verifique no SideQuest para certificar-se que o BMBF tenha permissões de arquivo.

---

### Beat Saber está crashando
Se seu jogo estiver falhando ao fazer algo, desabilite seus mods um por um. executando o seu jogo toda vez para ver se o problema é corrigido antes de pedir ajuda em um canal de suporte.

### Eu só vejo uma tela branca quando abro o BMBF
If you only see a white screen when you open BMBF from unknown sources, try waiting a few seconds. Se isso não funcionar, reinicie seu quest e tente abrir o BMBF novamente.

### Meu Beat Saber tem 3 pontos quando eu abro
Se o seu Beat Saber está recebendo 3 pontos ao iniciar, certifique-se de que:

1. Você abriu e jogou uma música antes de modificar o jogo
2. Você não está usando uma versão pirata do jogo
3. Certifique-se de estar usando a versão mais recente do BMBF
