---
sidebar: auto
---

# Модификация PC версии

## Вступление

::: danger ДИСКЛЕЙМЕР Если вы хотите использовать моды, вы должны понимать, что:

* Вы можете столкнуться с проблемами, которых нет в версии игры без модификаций. В 99.9% случаев, баги, ошибки и плохая производительность игры связаны с модификациями.
* Модификации могут быть сломаны в результате обновления игры и это нормально. Будьте терпеливы, когда это происходит, потому что создатели модов - это добровольцы с реальной жизнью.
* Beat Games не пытаются целенаправленно ломать работу модификаций. Они просто работают над своей игрой и иногда это приводит к поломке модификаций. Beat Games не ставит перед собой цели специально вредить модификациям.

Не атакуйте разработчиков игры по вопросам, связанных с модификациями, и наоборот. Создатели модификаций и разработчики игры - разные команды. Просто ведите себя достойно, ок. :::

:::warning СОБЛЮДАЙТЕ ПРАВИЛА БЕЗОПАСНОСТИ, КОГДА УСТАНАВЛИВАЕТЕ МОДИФИКАЦИИ Beat Saber **НИКОГДА** не должен запускаться от имени администратора.

Если вы скачали и установили модификацию, которая просит дать доступ к вашей учетной записи, **НЕ** делайте этого. Сообщите нам об этом. То, что вы установили, является вредоносной модификацией!

The only approved case is when activating/deactivating OneClick™ Install in Mod Assistant. Administrator access is required to register the program with your computer to handle OneClick™ Install links.

If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

Beat Saber natively supports custom songs, so if that's all you're looking for, you don't require more mods! It's a wise idea to install `SongCore` though, as this mod expands upon the base game functionality to improve loading times and provide functionality for other mods like the in-game downloader, custom leaderboards, playlists, etc.

::: warning This guide is for PC-modding on Windows.  
If you have a Quest, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux page](/modding/linux.md) or [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

If you run into problems at any point, please head to the [support page](./support) and see if you can identify what went wrong before asking in the Discord server. Chances are, your answer is on that page!

::: warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** suggest against using video tutorials for modding. Often, we find they are outdated or contain a incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

## Установщики модификаций

### Mod Assistant
> **ЭТО РЕКОМЕНДОВАННЫЙ УСТАНОВЩИК МОДОВ.**

__**Run the game at least once**** before trying to mod the game! This applies to reinstalling your game too.

A simple Beat Saber Mod Installer similar to the mod manager, but with additional features such as mod removal and version checking! Get it on [Assistant's GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Как получить больше песен
::: tip Most maps in the "Top All", "Rating", "Downloads" or "Plays" sort filters were created before good mapping practices were established. Try downloading songs released between late 2019 and now to get the best custom levels experience. :::

::: warning It is a good idea to backup your `CustomLevels` folder periodically as there is a small chance it will be reset if the game updates!

This folder is located in your game install: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### Загрузка карт изнутри игры
The `BeatSaver Downloader` mod allows you to download maps in-game using the `MORE SONGS` menu button on the `MODS` menu screen. This pulls maps directly from [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) is the master repository of custom songs made by the community. Many other tools and sites enhance the experience of downloading custom songs, but this site is where they are stored. To install songs downloaded from the site, unzip them into a folder and place it into `Beat Saber/Beat Saber_Data/CustomLevels`. You can also use the in-game downloader mod, or Mod Assistant's OneClick™ Install feature.

To enable and use Mod Assistant's OneClick™ Install see the picture below: ![Mod Assistant](~@images/beginners-guide/modassistant-oneclick.png)

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) is a site that tries to help make finding fantastic maps to play easier. It does this by categorizing the thousands of songs on BeatSaver and lets you sort by a song's genre and many other attribute tags. It also has a full social feature where players can review songs and comment on them. One of the most used features is the "Curator Recommended" feature where a team plays through most songs released each day and recommends the ones that stand out, letting you [automatically download these in-game](https://bsaber.com/beatsync/).

### Внешние программы для загрузки и организации карт

There are no working song management apps available at this time.

### Плейлисты
You need to install the [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) mod.

Then you can either:

* Использовать функцию `Установить плейлист` во вкладке Настройки в Mod Assistant.
* Или поместите файл плейлиста в папку `Beat Saber/Playlists`, выберите в игре и нажмите кнопку "Скачать все песни".

You should see the playlist next to the Custom Levels album's in-game. The mod also supports managing playlists in-game.

## Папка установки
_Where is Beat Saber installed?_

### Расположение по умолчанию
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Другие возможные места расположения
**If you have moved your install folder to a different drive, it might be in the location below.** Replace the drive letter `F` with the drive your game is installed on.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Ручная установка
A mod installer is the recommended way to install mods. See the section [above](#installers). If you have patched the game and just need to install mods that are not available in the installer, skip to step 4.

::: warning STAY SAFE WHEN INSTALLING MODS Modding your game with unverified mods such as mods found in the `#pc-mods` channel comes with risks, including the possibility for malicious software that acts like a regular mod.

Beat Saber will **NEVER** ask you to run it as Administrator.

If you've downloaded and installed a mod and you get the User Account Control prompt, **DO NOT** click accept, and please report this. If you're unsure if something you installed is malware or not, ***please ask someone in our discord***. :::

**Run the game at least once** before trying to mod the game! This applies to reinstalling your game too.

### Установка BSIPA

1. Скачайте [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Перейдите в папку [установки](#install-folder) и распакуйте в нее содержимое BSIPA. ![Директория очищена](~@images/beginners-guide/directory-clean.png "Директория очищена") ![Директория Ipa](~@images/beginners-guide/directory-ipa.png "Директория Ipa")
3. Дважды нажмите на IPA.exe для модификации игры. Все моды из папки `Plugins` теперь будут загружены при запуске игры. Если вы видите какие-то ошибки, то вы, вероятно, не выполнили шаг 2 правильно. ![Папка изменена](~@images/beginners-guide/directory-patched.png "Папка изменена")

### Установка модификаций

4. Скачайте модификацию(и), который(ые) вы хотите установить, будь то с GitHub, [BSMG Discord](https://discord.com/invite/beatsabermods) `#pc-mods`,  [BeatMods](https://beatmods.com/#/mods) или из других источников. **Убедитесь, что вы скачали всё нужное, которое требуются для работы модификации.** ![Каталог плагинов](~@images/beginners-guide/directory-plugins.png "Каталог плагинов")
5. Некоторые модификации имеют инструкции по их установке, а некоторые нет. В общем случае, вы можете просто перетащить содержимое архива в папку Beat Saber, и тогда файлы сами попадут в правильные папки.

## Как удалить модификации
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## Что можно посмотреть ещё

* [Хваты и советы](./grips-and-tricks.md)
* [Создание карт](/ru/mapping/)
* [Пользовательские мечи](/ru/models/custom-sabers.md)
* [Пользовательские модели аватаров](/ru/models/custom-avatars.md)
* [Пользовательские платформы](/ru/models/custom-platforms.md)
* [Играть пользовательские песни в Мультиплеере](https://discord.com/invite/gezGrFG4tz)
* [Создание модификаций](/ru/modding/)

## Есть вопросы?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
