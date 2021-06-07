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

:::warning PROTEGE-TE ENQUANTO INSTALAS MODS O Beat Saber **NUNCA** te vai pedir para ser executado como Administrador.

Se transferiste e instalaste um mod e tens o pedido de Controlo de Conta de Utilizador, **NÃO** carregues em Aceitar, e reporta isto. O que tu instalaste é um mod malicioso!

Se não tens a certeza se alguma coisa que instalaste é malware ou não, ***por favor pergunta a alguém no nosso Discord.***. :::

O Beat Saber suporta nativamente músicas personalizadas, então se isso é tudo o que procuras, não precisas de mods! No entanto, é uma boa ideia instalar o `SongCore`, porque este mod extende a funcionalidade base do jogo para melhorar tempos de carregamento e fornece funcionalidades para outros mods, como transferir músicas dentro do jogo, classificações personalizadas, playlists, etc.

::: warning Este guia é para PC Modding no Windows.  
Se tens uns Quest, vê a [página de Modding nos Quest](/quest-modding.md).  
Se estás no Linux, vê a [página do Linux](/modding/linux.md) ou [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

Se a qualquer momento tiveres problemas, por favor, acessa a [página de suporte](./support) e verifica se consegues identificar o problema antes de perguntar no servidor do Discord. É provavel que a tua resposta esteja nessa página!

::: warning Eu assisti este vídeo no YouTube, mas fiquei preso e/ou não funcionou. Por que isso? Nós do BSMG **fortemente** sugerimos não usar qualquer tutorial do YouTube para modding. Muitas vezes, achamos que eles estão desatualizados ou contêm informações incompletas ou até mesmo completamente erradas.

Em vez disso, você deve seguir os guias escritos aqui na wiki ou procurar ajuda no [Discord do BSMG](https://discord.gg/beatsabermods). :::

## Instaladores

### Mod Assistant
> **ESTE É ATUALMENTE O MOD INSTALLER RECOMENDADO.**

__**Execute o jogo pelo menos uma vez**** antes de tentar instalar mods nele! Isto também se aplica a reinstalar o jogo.

Um simples Instalador de Mods para o Beat Saber similar ao gerenciador de mods, mas com recursos adicionais como remoção de mods e verificação de versão! Podes obtê-lo no [GitHub do Assistant](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Como obter mais músicas
::: tip A maioria dos mapas nos filtros "Top Todos", "Rating", "Downloads" ou "Plays" foram criados antes das boas práticas de mapeamento serem estabelecidas. Experimente baixar músicas lançadas entre o final de 2019 e agora para obter a melhor experiência de níveis personalizados. :::

::: warning É uma boa ideia fazer backup da tua pasta de `CustomLevels` periodicamente, pois há uma pequena chance desta ser perdida se o jogo atualizar!

Esta pasta está localizada na instalação do jogo: `Beat Saber/Beat Saber_Data/Custom Levels` :::

### In-game Downloader
O mod `BeatSaver Downloader` permite que tu baixes mapas dentro do jogo usando o botão do menu `MORE SONGS` no ecrã do menu `MODS`. Isto instala mapas diretamente do [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) é o repositório principal de músicas personalizadas feitas pela comunidade. Muitas outras ferramentas e sites melhoram a experiência de download de músicas personalizadas, mas este site é onde elas estão hospedadas. Para instalar músicas baixadas do site, descompacta-as numa pasta e coloca-a dentro da pasta `Beat Saber/Beat Saber_Data/CustomLevels`. Também podes usar o mod de download no jogo, ou o recurso OneClick™ Install do Mod Assistant.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) é um site que tenta ajudar a tornar mais fácil encontrar mapas fantásticos para jogar. Ele faz isso categorizando milhares de músicas do BeatSaver e permite-te classificar por um gênero de música e muitas outras tags de atributo. It also has a full social feature where players can review songs and comment on them. One of the most used features is the "Curator Recommended" feature where a team plays through most songs released each day and recommends the ones that stand out, letting you [automatically download these in-game](https://bsaber.com/beatsync/).

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

::: warning STAY SAFE WHEN INSTALLING MODS Modding your game with unverified mods such as mods found in the `#pc-mods` channel comes with risks, including the possibility for malicious software that acts like a regular mod.

Beat Saber will **NEVER** ask you to run it as Administrator.

If you've downloaded and installed a mod and you get the User Account Control prompt, **DO NOT** click accept, and please report this. If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

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
* [Play Customs in Multiplayer](https://discord.com/invite/gezGrFG4tz)
* [Making Mods](/modding/)

## Tem alguma pergunta?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
