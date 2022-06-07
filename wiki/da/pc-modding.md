---
sidebar: auto
---

# PC Modding

## Forord

::: danger DISCLAIMER Når du vælger at benytte mods, forstår du at:

* Du kan opleve problemer, der ikke findes i vanilla-spillet. 99,9% af bugs, crashes og lag skyldes mods.
* Mods er underlagt af at blive ødelagt af opdateringer, og det er normalt - vær tålmodig og respektfuld når dette sker, eftersom modders er frivillige med et liv ved siden af.
* Beat Games forsøger ikke med vilje at ødelægge mods. De ønsker kun at arbejde med programmeringen og nogle gange vil dette ødelægge mods, men det er ikke med vilje.

Angrib ikke udviklerne for problemer relateret til mods eller omvendt - modders og udviklere er to separate grupper. Bare lad være med at være en idiot. :::

:::warning FORBLIV SIKKER NÅR DU INSTALLERER MODS Beat Saber vil **ALDRIG** bede dig om at køre den som administrator.

Hvis du har downloadet og installeret en mod og hvis du får User Account Control prompten, så **LAD VÆR** med at clicke accepter, og vær sød at rapportere det. Det du har installeret er en fjendtlig mod!

Den eneste godkendte sag er, når du aktiverer/deaktiverer OneClick™ Installer i Mod Assistant. Administrator adgang er påkrævet for at registrere programmet med din computer OneClick™ Installerings links.

Hvis du er usikker på om noget, du har installeret, er malware eller ej, ***så spørg venligst nogen i vores discord***. :::

Beat Saber understøtter allerede brugerskabte sange, så hvis det er alt du leder efter, behøver du ikke flere mods! Det er en god idé at installere `SongCore` alligevel, da denne mod udvider spillets grundfunktion til at forbedre indlæsningstiden og levere funktionalitet til andre mods såsom download af sange inde i spillet, ranglister til brugerskabte baner, playlister osv.

::: warning This guide is for PC-modding on Windows.  
If you have a Quest, see the [Quest Modding page](/quest-modding.md).  
If you're on Linux, check out the [Linux page](./linux-modding.md) or [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

If you run into problems at any point, please head to the [support page](./support/) and see if you can identify what went wrong before asking in the Discord server. Der er gode muligheder for, at svaret er på den side!

::: warning ADVARSEL Jeg fulgte en tutorial på YouTube, men jeg sidder fast/det virkede ikke. Hvad skyldes det? Vi her i BSMG anbefaler **kraftigt** imod at bruge nogen tutorials fra YouTube. Ofte finder vi, at de er forældede eller indeholder en ufuldstændig, fejlagtig eller direkte ukorrekt information.

I stedet bør du følge de skriftlige vejledninger her på wikisiden eller søge hjælp i [BSMG Discord](https://discord.gg/beatsabermods). :::

## Installatører

### Mod Assistant
> **DETTE ER NUVÆRENDE DET ANBEFALEDE INSTALLATIONSPROGRAM TIL MODS.**

__**Kør spillet mindst én gang**** før du forsøger at modde spillet! Dette gælder også for geninstallering af dit spil.

Det er et simpelt Beat Saber Mod Installationsprogram som ligner mod manager, men med yderligere funktioner såsom mod-fjernelse og kontrol af din version! Få den fra [Assistentens GitHub](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Sådan får du flere sange
De fleste maps i sorteringsfiltrene "Top All", "Rating", "Downloads" eller "Plays" blev oprettet før god mappingspraksis blev etableret. Prøv at downloade sange udgivet mellem slutnignen af 2019 og nu for at få den bedste oplevelse. :::

::: advarsel Det er en god idé at sikkerhedskopiere din `CustomLevels` mappe periodevis, da der er en lille chance for at den vil blive nulstillet hvis spillet opdateres!

Denne mappe er placeret i din spil installation: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### Downloader inde i spillet
Plugin'et `BeatSaver Downloader` giver dig mulighed for at downloade baner inde i spillet ved hjælp af menuknappen `MORE SONGS` på menuskærmen `MODS`. Dette trækker baner direkte fra [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) er hovedarkivet for brugerskabte baner fra fællesskabet. Mange andre værktøjer og websteder forbedrer oplevelsen af at downloade brugerskabte baner, men dette er stedet, hvor de er opbevaret. For at installere sange, downloadet fra BeatSaver, skal du udpakke zip-filen i en mappe og placere mappen i `Beat Saber/Beat Saber_Data/CustomLevels`. Du kan også bruge in-game downloader modden, eller Mod Assistants OneClick™ Installerings funktion.

For at aktivere og bruge Mod Assistants OneClick™ Installatør, så se billedet nedenfor: ![Mod Assistant](~@images/beginners-guide/modassistant-oneclick.png)

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) er en hjemmeside, der forsøger at hjælpe med at gøre det nemmere at finde fantastiske baner. Det gør den ved at kategorisere de tusindvis af sange fra beatsaver og lader dig sortere efter en sangs genre og mange andre karaktertræk. Den har også en social funktion, hvor spillerne kan gennemgå sange og kommentere dem. En af de mest anvendte funktioner er "Curator Recommended" funktionen, hvor et hold gennemspiller de fleste sange udgivet hver dag og anbefaler dem, der skiller sig ud, og lader dig [automatisk downloade disse sange inde i spillet](https://bsaber.com/beatsync/).

### Apps til sanghåndtering

Der er ingen fungerende sang management apps tilgængelige på nuværende tidspunkt.

### Playlister
Du skal installere [PlaylistManager](https://github. com/rithik-b/PlaylistManager/releases/latest) modden.

Så kan du enten:

* Brug værktøjet `Install Playlist` i fanen Indstillinger i Mod Assistant.
* Placer playlistfilen i `Beat Saber/Playlists`, vælg playlisten inde i spillet, og tryk derefter på "download all songs".

Du burde se playlisten ved siden af Custom Levels albummet inde i spillet. Modden understøtter også håndtering af playlister inde i spillet.

## Installationsmappe
_Hvor er Beat Saber installeret?_

### Standardplacering
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Andre Placeringer
**Hvis du har flyttet din installationsmappe til et andet drev, kan det være på placeringerne nedenfor.** Erstat drevbogstavet `F` med det drev, dit spil er installeret på.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Manuel installering
Et mod-installationsprogram er den anbefalede måde at installere mods. Se afsnittet [ovenfor](#installering). Hvis du har opdateret spillet og bare har brug for at installere mods der ikke er tillgængelige i installationsprogrammet, skal du springe til trin 4.

::: warning FORBLIV SIKKER NÅR DU INSTALLERER MODS Modding af dit spil med ubekræftede mods, såsom mods fundet i `#pc-mods` kanalen, kommer med ricisi, herunder muligheden for fjendtlig software, der fungerer som en regelmæssig mod.

Beat Saber vil **ALDRIG** bede dig om at den som administrator.

Hvis du har downloadet og installeret en mod og hvis du får User Account Control prompten, så **LAD VÆR** med at clicke accepter, og vær sød at rapportere det. Hvis du er usikker på om noget, du har installeret, er malware eller ej, ***så spørg venligst nogen i vores discord***. :::

**Kør spillet mindst én gang** før du forsøger at modde spillet! Dette gælder også for geninstallering af dit spil.

### Installer BSIPA

1. Download [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Gå til din [installationsmappe.](#install-folder) og udpak indholdet af BSIPA-zipfilen ind i den mappe. ![Direktions Fjernelse](~@images/beginners-guide/directory-clean.png "Direktions Fjernelse") ![Direktions Ipa](~@images/beginners-guide/directory-ipa.png "Direktions Ipa")
3. Dobbeltklik på IPA.exe for at modde spillet. Alle mods i mappen `Plugins` vil nu blive indlæst, når spillet startes. Hvis der er fejl, har du sandsynligvis ikke fulgt trin 2 korrekt. ![Direktions Modded](~@images/beginners-guide/directory-patched.png "Direktions Modded")

### Installer Mods

4. Download den mod eller de mods du ønsker at installere, uanset om det er fra GitHub, [BSMG Discorden](https://discord.com/invite/beatsabermods) i `#pc-mods` kanalen, [BeatMods](https://beatmods.com/#/mods) eller andre kilder. **Sørg for at downloade eventuelle afhængigheder, som bruges af mod'en.** ![Direktions Plugins](~@images/beginners-guide/directory-plugins.png "Direktions Plugins")
5. Nogle mods har installationsvejledninger, og nogle har ikke. Generelt kan du bare trække og slippe zip-indholdet ind i din Beat Saber installationsmappe, og filerne bør selv komme ind i de korrekte mapper.

## Downgrading

Check `#modding-announcements` in [BSMG](https://www.discord.gg/beatsabermods) to see if the latest version is moddable. If it is not, you can follow these tutorials to downgrade to a moddable version.

Click on these links corresponding to where you own the game to see the tutorials.

* [Oculus Store](https://computerelite.github.io/tools/Oculus/OculusDowngraderGuide.html)
* For Steam you have a few options to be able to downgrade. These two are supported by [BSLG](https://discord.gg/MrwMx5e).
  * [BSLegacyLauncher](https://www.youtube.com/watch?v=qjNU5aENHRU)
  * [LegacyInstaller](https://github.com/Goobwabber/LegacyInstaller#readme)

## How to uninstall mods
Either remove the dll from the `Plugins` folder, or click the `Uninstall` button in Mod Assistant.

## Where to go from here

* [Grips and Tricks](./grips-and-tricks.md)
* [Making Beatmaps](/mapping/)
* [Custom Sabers](/models/custom-sabers.md)
* [Custom Avatars](/models/custom-avatars.md)
* [Custom Platforms](/models/custom-platforms.md)
* [Play Customs in Multiplayer](https://discord.com/invite/gezGrFG4tz)
* [Making Mods](/modding/)

## Have questions?
Visit the support channels in the [BSMG Discord](https://discord.gg/beatsabermods)!
