# Vanliga Frågor

## Jag fick precis Beat Saber, hur kommer jag igång?
Kolla in vår [nybörjarguide](/beginners-guide.md)!

## Hur får jag fler låtar?
> [BeatSaver](https://beatsaver.com) är huvudarkivet för låtar gjorda av gemenskapen. Många andra verktyg och webbplatser förbättrar upplevelsen av att ladda ner anpassade låtar, men på denna plats är dem lagrade.

Om du laddar ner banor manuellt från BeatSaver, extrahera dem till en mapp och placera filerna i `Beat Saber/Beat Saber_Data/CustomLevels`. Detta är den directory som spelet läser nedladdade banor ifrån.

### BeastSaber
[Beast Saber](https://www.bsaber.com) är en recensionssida som syftar till att kurera alla låtar på BeatSaver. Du kan också ladda ner spellistor, följa mappare, hitta låtar med hjälp av avancerade sorteringsmetoder och mycket mer.

### Verktyg för låthantering
Följande är program som kan användas för att hjälpa dig att ladda ner banor, med några andra medföljande funktioner.

* [Beat Saber Downloader](https://drive.google.com/file/d/1QWedF77hWYbqcigIWa2UcpXlhqGTjwR1/view), ett nedladdningsprogram av Sturdyfool0.
* [BeatList](https://github.com/Alaanor/beatlist) är en app som hanterar spellistor och beatmaps, av Alaanor.

## Hur installerar jag spellistor?

### PC
Du behöver installera moddet [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest).

Sen kan du antingen:

* Använda verktyget `Install Playlist` som finns i ModAssistants Options-flik.
* Placera spellistefilen i `Beat Saber/Playlists`, välja den i spelet och tryck på Download all.

Du bör nu se spellistan bredvid Custom Levels albumet i spelet. Moddet stöder också hantering av spellistor i spelet.

### Quest
Du kan använda [Playlist Editor Pro](https://beatsaberquest.com/bmbf/my-tools/playlist-editor-pro/) för att hantera spellistorna på din Quest. Notera att en nedladdad bana endast kan visas en gång i spelet på grund av en begränsning hos BMBF.

::::warning VARNING för Quest-användare Omladdning av mappen Custom Songs återställer alla spellistors organisering. :::

## Hur skapar jag mina egna banor?
Se [mappning](/mapping/)!

## Hur laddar jag in plugins som inte finns i ModAssistant?
Se [denna sektion](/pc-modding.md#manual-installation) i nybörjarguiden.

## Har multiplayer crossplay?
Officiellt är multiplayer begränsad till att spela med andra människor i den butiksversion (Oculus eller Steam) du köpt. Dessutom inaktiveras den officiella multiplayern när man modifierar spelet på Quest.

Moddet BeatTogether är den nuvarande lösningen för cross-platform mellan de olika moddade spelversionerna. Gå med i deras [Discord-server](https://discord.com/invite/gezGrFG4tz) och se kanalen `#install-instructions` för mer information.

## My game updated and now none of my mods are working
Each time the game updates it is possible *(and very likely)* that your existing mods will stop working and need to be updated. The game developers realized this, so when the game updates and you run it for the first time, everything in the `Plugins` folder is moved into a new folder called `Old 1.xx.x Plugins`. **Leave those plugins in there!**

To get mods back, simply **run the installer again.**  
The BeatMods repository only includes mods that have been confirmed to work on the latest version of the game!

If you're confused by any of this, visit [Beginners Guide](/beginners-guide.md).

## Hur fungerar poängsystemet i Beat Saber? Hur fungerar den globala rankningen?
We have sections on the [grips and tricks](/grips-and-tricks.md) page dedicated to the scoring and ranking systems, check them out!

## My menus are blank and I have nothing to click on
If the main window in your game is blank, your save file likely got corrupted.

To fix it, navigate to: `%AppData%\..\LocalLow\Hyperbolic Magnetism`

Delete or rename the Beat Saber folder to something else. When you re-enter the game, it'll recreate the save file and should load the main menu properly.
