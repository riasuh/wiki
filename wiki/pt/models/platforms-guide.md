---
sidebar: auto
prev: ./avatars-guide.md
next: ./notes-guide.md
description: Guia de Emma para criar Custom Platforms!
---

# Guia de Custom Platforms
_Guia de Emma para criar Custom Platforms._

## Projeto
Open the current [Custom Platforms Project](https://github.com/affederaffe/CustomPlatformsUnityProject/releases/) with [Unity 2018.1.6f1](https://download.unity3d.com/download_unity/57cc34175ccf/Windows64EditorInstaller/UnitySetup64-2018.1.6f1.exe).

## Primeiros passos
![Custom Platform Script](~@images/models/platforms/CustomPlatformScript.png)

Crie um `Empty GameObject` clicando com o botão direito na janela de Hierarchy e selecionando `Create Empty`. Certifique-se de definir sua posição no Inspector para a origem (0,0,0). Procure no inspector pelo script de </code>Custom Platform` e aplique-o a este GameObject. Tudo dentro deste Objeto será exportado quando o botão no script de <code>Custom Platform` for pressionado. No script existem também opções de Exporting. Eles desabilitam partes da plataforma original (Para quando você deseja substituir algo parcialmente).

## Adicionando modelos
![Objects](~@images/models/platforms/Objects.png)

Drag all models you want in your Platform into the GameObject created in the second step and position them to your liking. Para os materiais dos modelos, certifique-se de usar shaders compatíveis com o Beat Saber ou os que você pode encontrar no Projeto chamado `_dark_replace` e `_glow_replace`. Estes são materiais personalizados que atuam como os materiais no Beat Saber, ou seja, reagem às luzes de tube e mist.

### Track Rings
O script `Track Rings` faz track rings como são vistos no jogo. Para conseguir isso, o script precisa de um prefab. Currently I haven't been able to figure out how to use a prefab in it, so I used a gameObject, that is part of the platform hierarchy, that I later moved off to `y = -1000`. For the ring-preview to show correctly, move this gameObject to (0,0,0) and adjust your settings and before importing move it off to somewhere offscreen.

Ativando o rotating effect, faz com que os rings gire de acordo com o evento especificado, dependendo das variáveis que ele é dado. (Eu ainda não testei eles, então experimente).

Ativando o step effect altera o espaçamento dos rings quando o evento especificado é chamado entre 2 variáveis.

![Track Rings Script](~@images/models/platforms/TrackRingsScript.png)

### Tube Light
![Tube Light](~@images/models/platforms/TubeLightScript.png)

Este script ativar blinking lights. Putting this on an empty gameObject changes the background and adds a bit of color to that space, according to the light ID's. When there's also a mesh renderer on it, it'll change the meshes color according to the light ID's. When using this no color adding is needed, so I change the size on the script to 0.

### Song Events
![Song Event Handler](~@images/models/platforms/SongEventHandler.png)

The event manager is the most useful script. With it you can trigger an action on any beat saber event (even unused ones). Para adicionar um evento, pressione o botão `+` abaixo do botão `On Trigger ()`. Drag in the object you want to manipulate into the box that just got created. Press the dropdown menu to the right and choose what that object should do, by first selecting what component, then what action. Make sure that you only use 1 event Handler per gameObject, as only 1 will work per gameObject.

### Spectrogram
![Spectrogram](~@images/models/platforms/Spectrogram.png)

The spectrogram script works like the track rings script and also requires a prefab or gameObject. This will get stretched and shrunk according to the sound of the game and the variables provided. (Haven't played with this either).

## Exporting

![Saving](~@images/models/platforms/Save.png)

Export the platform trough the script that you previously added to the gameObject to the location of your choosing. Preferably the game's directory `Beat Saber/CustomPlatforms`.

::: tip NOTE **Once you've got your new platform working**, [upload them to ModelSaber](https://modelsaber.com) if you want to share them with the world. :::

![Cat](~@images/models/platforms/Cat.png)
