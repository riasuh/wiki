---
sidebar: auto
---

# PC Modding

## Prefácio

::: danger AVISO Ao escolher usar mods, tu entendes que:

* Tu podes ter problemas que não existem no jogo vanilla. 99,9% dos bugs, travamentos e lag devem-se aos mods.
* Os mods estão sujeitos a falhas por causa de atualizações e isso é normal - sê paciente e respeitoso quando isso acontecer, porque os modders são voluntários com vidas reais.
* A Beat Games não está a tentar quebrar os mods intencionalmente. Eles querem trabalhar no código fonte e às vezes isso quebra os mods, mas não estão tentando matar os mods.

Não ataque os devs por problemas relacionados a mods, e vice versa - modders e devs são dois grupos separados. Não sejas um idiota ok. :::

O Beat Saber suporta originalmente músicas personalizadas, então se isso é tudo o que tu estás à procura, não precisas de mais mods! Entretanto, é uma boa ideia instalar o `SongCore` porque este mod se expande na funcionalidade base do jogo para melhorar o tempo de carregamento e fornecer a funcionalidade para outros mods como o baixador dentro do jogo, classificações personalizadas, listas de reprodução, etc.

::: warning Este guia é para PC-modding no Windows.  
Se você tem um Quest, veja a [página de Modding do Quest](/pt/quest-modding.md).  
Se você estiver no Linux, confira a [página do Linux](/pt/modding/linux.md) ou [QBeat](https://github.com/geefr/beatsaber-linux-goodies/blob/master/README.md) :::

Se a qualquer momento tiveres problemas, por favor, acessa a [página de suporte](./support) e verifica se consegues identificar o problema antes de perguntar no servidor do Discord. É provavel que a tua resposta esteja nessa página!

::: warning Eu assisti este vídeo pelo Elite Eric, mas fiquei preso e/ou não funcionou. Por que isso? Nós do BSMG **fortemente** sugerimos não usar qualquer tutorial do Elite Eric. Após revisar grande parte do conteúdo dele, ele contêm uma grande quantidade de informações incompletas, erróneas, ou diretamente informações incorretas. Tentativas de chegar nele para corrigir esses erros, infelizmente foram recebidos com silêncio e novos tutoriais (também incorretos).

Em vez disso, você deve seguir os guias escritos aqui na wiki ou procurar ajuda no [Discord do BSMG](https://discord.gg/beatsabermods). :::

## Instaladores

### Mod Assistant
> **ESTE É ATUALMENTE O MOD INSTALLER RECOMENDADO.**

__**Execute o jogo pelo menos uma vez**** antes de tentar instalar mods nele! Isto também se aplica a reinstalar o jogo.

Um simples Beat Saber Mod Installer similar ao gerenciador de mods, mas com recursos adicionais como remoção de mods e verificação de versão! Podes obtê-lo no [GitHub do Assistente](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Como obter mais músicas
::: tip A maioria dos mapas "Top Todos", "Rating", "Downloads" ou "Plays" foram criados antes das boas práticas de mapeamento serem estabelecidas. Experimente baixar músicas liberadas no final de 2019 e agora obtenha a melhor experiência de custom levels. :::

### In-game Downloader
The `BeatSaver Downloader` mod allows you to download maps in-game using the `MORE SONGS` menu button on the `MODS` menu screen. Isto instala mapas diretamente do [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) é o repositório principal de custom songs feitas pela comunidade. Muitas outras ferramentas e sites melhoram a experiência de download de músicas personalizadas, mas este lugar é onde elas estão hospedadas. Para instalar músicas baixadas do site, descompacta-as numa pasta e coloca-a no `Beat Saber/Beat Saber_Data/CustomLevels`. You can also use the in-game downloader mod, or Mod Assistant's OneClick™ Install feature.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) é um site que tenta ajudar a tornar mais fácil encontrar mapas fantásticos para jogar. Ele faz isso categorizando milhares de músicas do beatsaver e te permite classificar por um gênero de música e muitas outras tags de atributo. Tem também uma característica social completa onde os jogadores podem avaliar músicas e comentar nelas. Uma das características mais usadas é o recurso "Curator Recommended" onde uma equipe joga a maioria das músicas liberadas a cada dia e recomenda as que se destacam, Deixando você [baixar automaticamente elas dentro do jogo](https://bsaber.com/beatsync/).

### Programas de gerenciamento de músicas

There are no working song management apps available at this time.

### Playlists
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* Use the `Install Playlist` tool in the Options tab of Mod Assistant.
* Place the playlist file into `Beat Saber/Playlists`, select it in-game, then hit download all songs.

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

## Pasta De Instalação
_Where is Beat Saber installed?_

### Localização Padrão
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Outras Localizações
**If you have moved your install folder to a different drive, it might be in the location below.** Replace the drive letter `F` with the drive your game is installed on.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Instalação Manual
A mod installer is the recommended way to install mods. See the section [above](#installers). If you have patched the game and just need to install mods that are not available in the installer, skip to step 4.

**Run the game at least once** before trying to mod the game! This applies to reinstalling your game too.

### Instale o BSIPA

1. Baixe o [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Navegue para a sua [pasta de instalação](#install-folder) e extraia o conteúdo do BSPIA nela. ![Directory Clean](~@images/beginners-guide/directory-clean.png "Directory Clean") ![Directory Ipa](~@images/beginners-guide/directory-ipa.png "Directory Ipa")
3. Clique duas vezes no IPA.exe para instalar os mods no jogo. Todos os mods na pasta `Plugins` agora serão carregados ao iniciar o jogo. Se houver erros, você provavelmente não seguiu corretamente a etapa 2. ![Directory Patched](~@images/beginners-guide/directory-patched.png "Directory Patched")

### Instale os mods

4. Baixe o mod (s) que você deseja instalar, seja do GitHub, [Canal do Discord BSMG](https://discord.com/invite/beatsabermods) `#pc-mods` ,  [BeatMods](https://beatmods.com/#/mods) ou outras fontes. **Certifique-se de baixar quaisquer dependências necessárias pelo mod.** ![Directory Plugins](~@images/beginners-guide/directory-plugins.png "Directory Plugins")
5. Alguns mods têm instruções de instalação, outros não. Normalmente, você pode apenas arrastar e soltar o conteúdo zip na pasta de instalação do Beat Saber e os arquivos devem ir para as pastas correspondentes.

## Como desinstalar mods
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## Para onde ir daqui

* [Grips and Tricks](./grips-and-tricks.md)
* [Making Beatmaps](/mapping/)
* [Custom Sabers](/models/custom-sabers.md)
* [Custom Avatars](/models/custom-avatars.md)
* [Custom Platforms](/models/custom-platforms.md)
* [Setup Multiplayer](https://bs.assistant.moe/Multiplayer/)
* [Making Mods](/modding/)

## Tem alguma pergunta?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
