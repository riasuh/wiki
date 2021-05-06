---
sidebar: auto
---

# Modding su Quest

## Prefazione

* Questa guida è sia per Quest 1 e Quest 2.
* Nessuno è mai stato bandito per il modding.

::: DISCLAIMER di pericolo Scegliendo di usare le mod, comprendi che:

* Potresti sperimentare problemi inesistenti nel gioco vanilla. 99,9% di bug, arresti anomali e lag sono dovuti alle mod.
* Le mod sono soggette alla corruzione da aggiornamenti e ciò è normale; sii paziente e rispettoso quando succede, poiché i modder sono volontari con una vita reale.
* Beat Games non cerca intenzionalmente di corrompere le mod. Desiderano lavorare sul loro codice e talvolta questo corrompe le mod, ma non vanno in giro a ucciderle.

Non attaccare gli sviluppatori del gioco per problemi relativi alle mod, e viceversa; i modder e gli sviluppatori del gioco sono due gruppi separati. Semplicemente, non fare l'idiota, ok. :::

:::attenzione Ho guardato un tutorial video su YouTube, ma mi ci sono bloccato/non ha funzionato. Che succede? Noi a BSMG sconsigliamo **fortemente** l'uso di tutorial video per il modding. Spesso, troviamo che siano obsoleti o contengano informazioni incomplete, erronee, o direttamente errate.

Invece, dovresti seguire le guide scritte qui sulla wiki o cercare aiuto nel [Discord di BSMG](https://discord.gg/beatsabermods). :::

## Installazione
Correntemente l'unico modo consigliato per installare canzoni personalizzate e mod è BMBF sideloaded con SideQuest usando un PC.

Se non hai accesso a un PC puoi usare uno [Smartphone Android](#installing-bmbf-with-an-android-phone).

* [BMBF apk](https://bmbf.dev/stable) :::attenzione Installare BMBF e moddare il tuo gioco disabiliterà il Multigiocatore Ufficiale nonché la visualizzazione e il caricamento di punteggi sulle classifiche di base del gioco. Se vorresti giocare al multigiocatore moddato, ti serve la mod `Beat Together`, che consente il gioco incrociato tra pc e quest e consente l'uso di canzoni personalizzate se tutte le parti posseggono detta canzone. La mod si può trovare nel Gruppo di Modding di Beat Saber in `#quest-mods` o sul sito di [Questboard](https://questmodding.com).

Per ottenere le classifiche sulle canzoni personalizzate e poter ottenere Punti Prestazioni (PP) dalle canzoni classificate, ti serve la mod [ScoreSaber](https://new.scoresaber.com/quest). [Questo link](https://new.scoresaber.com/quest) ti porterà alla pagina di ScoreSaber per configurarla. ScoreSaber non sostituisce le classifiche di base del gioco, aggiunge solo le classifiche per le canzoni personalizzate.

**Nota:** Controlla il canale degli aggiornamenti nel [Discord ScoreSaber](https://discord.gg/WpuDMwU) per vedere se la mod è disponibile per la versione corrente del gioco. :::

### Installare BMBF con SideQuest
Se non lo hai già fatto, scarica e configura [SideQuest](https://sidequestvr.com/#/setup-howto)

Apri SideQuest e connetti il tuo Quest al tuo PC.

:::tip Se precedentemente hai moddato Beat Saber o hai punteggi di cui vuoi fare il backup, [Esegui il Backup dei tuoi Dati di Salvataggio!](#backup-save-data-using-sidequest) :::

Se hai un gioco moddato devi anche disinstallarlo premendo il pulsante `DISINSTALLA APP`. Poi puoi ripristinare il tuo salvataggio dallo stesso menu, dopo il modding.

Seleziona il pulsante `Installa APK dalla cartella` mostrato sotto e trova l'ultimo apk di BMBF che hai scaricato e cliccaci, o semplicemente trascinalo in SideQuest. Entrambi i metodi installeranno BMBF al tuo Quest.

![InstallAPK](~@images/beginners-guide/apkfromfolder.png)

Una volta installato correttamente, assicurati di avere l'ultima versione di BeatSaber installata e non moddata.

:::attenzione Prima del modding, esegui una volta Beat Saber, gioca un livello e perdi immediatamente!

Il modding non funziona correntemente se la funzionalità sperimentale multiutente è in uso. Dovrai rimuovere temporaneamente tutti i profili secondari prima di moddare il gioco. Puoi riaggiungerli dopo una volta installate le mod desiderate. :::

Dopo aver eseguito una volta BeatSaber, apri BMBF da fonti sconosciute come mostra l'immagine sotto. ![UnknownSources](~@images/beginners-guide/quest_home-menu.jpg)

Segui ogni passaggio esattamente come ti viene detto. Poi, dovresti vedere [bsaber.com](https://www.bsaber.com). Qui è dove puoi scaricare ogni canzone personalizzata disponibile. Puoi anche cliccare sull'icona del globo in alto a destra e anche andare a beatsaver per scaricare le canzoni.

Se in qualsiasi momento durante il processo di installazione, ottieni il popup `Ripristina App` clicca semplicemente su `Chiudi`. Questo avviso è piuttosto diretto alle versioni piratate del gioco quindi se stai solo moddando probabilmente non ci saranno conseguenze per averlo ignorato.

![RestoreApp](~@images/beginners-guide/restoreapp.png)

Continua al passaggio [Mod Principali](#core-mods) del processo di installazione.

### Installare BMBF con uno Smartphone Android
Questo **NON** è il modo consigliato per installare BMBF e dovrebbe esser usato solo se non hai accesso a un PC.

* [Requisiti](#requirements)
* [Configura il tuo Telefono](#setup-your-phone)
* [Installare BMBF con il tuo Telefono](#installing-bmbf-with-your-phone)
* [Configura Beat Saber](#setup-beat-saber)

#### Requisiti

* Un Telefono o Tablet Android (iPhone o iPad non sono supportati)
* Una Versione **a pagamento** di Beat Saber sullo Store dell'Oculus Quest
* Un Cavo per connettere il tuo Quest al tuo Telefono (Se il tuo telefono carica su USB C, il caricabatterie incluso con il tuo Quest dovrebbe funzionare)

#### Configura il tuo Telefono

1. Scarica l'[app bugjaeger dallo store di Google Pay](https://play.google.com/store/apps/details?id=eu.sisik.hackendebug&hl=gsw&gl=US)
2. Scarica la più nuova [APK di BMBF da bmbf.dev/stable](https://bmbf.dev/stable)
3. Segui [questa guida scritta](https://github.com/ComputerElite/wiki/wiki/Enable-Developer-Mode-for-OQ) per Abilitare la Modalità Sviluppatore sul tuo Quest.
4. Abilita la modalità Sviluppatore sul tuo Telefono
    1. Vai alle tue impostazioni di Android
    2. Scorri a "Informazioni sul telefono" e aprile
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

## Manage Save Data

### Backup Save Data using SideQuest

Open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber.

Navigate to `sdcard/Android/data/com.beatgames.beatsaber/files` using the SideQuest file explorer.

Save the files: `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` into a folder on your PC. Do not lose these, as they contain your scores and other settings!

### Restoring Save Data using SideQuest

To restore your data, open SideQuest and connect your Quest to your PC. Go to `My Apps` located in the top bar of the window and find Beat Saber. Using the SideQuest file explorer take the 3 files you saved from the [Backup Save Data using SideQuest](#backup-save-data-using-sidequest) steps `AvatarData.dat`, `PlayerData.dat` and `settings.cfg` and put them in the `sdcard/Android/data/com.beatgames.beatsaber/files` folder.

Go back to the menu and press the circular arrows located beside your latest backup. Your scores and settings should now be restored.

## Installing Mods

### Core Mods
Before installing any additional mods look in the top right of the BMBF web interface, you should see a red button that says, `Sync to Beat Saber`. Click this and let it finish syncing. Then go to your `mods` tab in BMBF. Make sure that you have the 5 core mods:

* Codegen
* Goodbye bug
* PinkCore
* QuestUI
* Custom Types

:::danger All other mods will not work if these core mods are not listed and enabled.

Se una delle mod principali non si abilita, elimina quella mod e clicca di nuovo `Sincronizza a Beat Saber` per riscaricarlo. Ricontrolla per vedere se è stato scaricato e abilitato. Se ancora non funziona o le mod sembrano essere abilitate, ma non funzionanti nel gioco, vedi [Mod Principali non funzionano](#core-mods-don-t-work) per i passaggi di risoluzione dei problemi. :::

### Nel tuo Quest
:::attenzione Non tutte le mod sono disponibili su QuestBoard!  
Se una mod non si vede qui, dovresti seguire piuttosto il metodo [Usare il Tuo PC](#using-your-pc). :::

Apri BMBF nel tuo Quest e vai alla scheda `Browser`, lì dovresti vedere un'icona a globo simile a quella mostrata sotto. Cliccala, poi clicca il pulsante `QuestBoard`.

![globequestboard](~@images/beginners-guide/globequestboard.png)

Dovresti essere accolto dal sito web sotto [QuestBoard](https://www.questmodding.com/). Poi, seleziona la scheda `SCARICA MOD`.

![questboardhome](~@images/beginners-guide/questboardhome.png)

Scorri in già con le tue levette. Ora puoi selezionare ogni mod dalla lista, vista sotto, e scaricarla cliccando il pulsante di download vicino a essa. Alcuni download potrebbero reindirizzarti a un sito web o una pagina di GitHub. In tal caso, segui le istruzioni a schermo o seleziona l'ultima `.zip` nell'elenco Rilasci, rispettivamente.

![questboardmods](~@images/beginners-guide/questboardmods.png)

### Usare il tuo PC
Puoi trovare e scaricare altre mod di Quest dal [Discord di BSMG](https://discord.com/invite/beatsabermods) nel canale `#quest-mods`.

:::attenzione Assicurati che il tuo Quest e PC siano sulla stessa rete e che tu stia usando http e non https! :::

Apri BMBF nel tuo Quest e vai alla scheda `Strumenti`, lì dovresti vedere un indirizzo web e un numero di versione simile a quello mostrato sotto.

![ip](~@images/beginners-guide/ip.png)

Sul tuo PC, apri il tuo browser e digita l'indirizzo nella barra di ricerca.

Dovresti esser accolto dalla schermata sotto.

Se non funziona, [clicca qui](#bmbf-web-interface-not-loading) per alcuni passaggi di risoluzione dei problemi.

![bmbfweb](~@images/beginners-guide/bmbfweb.png)

Ora basta trascinare ogni mod compatibile con Quest nella casella di caricamento e sincronizzare. Se la mod è stata originariamente fatta per una versione più vecchia, allora non si abiliterà automaticamente. Per abilitare una mod vecchia, vai alla scheda `Mod` e abilitala da lì.

## Installare le Canzoni
::: tip Gran parte delle mappe nei filtri di ordinamento "Migliori", "Classifica", "Download" o "Riprodotte" sono state create prima che le buone pratiche di mappatura fossero stabilite. Prova a scaricare le canzoni rilasciate tra il tardo 2019 e ora per una migliore esperienza con i livelli personalizzati. :::

### Nel tuo Quest
Ci sono 2 fonti per ottenere mappe personalizzate nel tuo Quest usando la finestra del browser.

* Se cerchi mappe curate e playlist visita [BeastSaber](https://bsaber.com/)
* Se non ti piace l'UI di BeastSaber potresti anche provare [BeatSaver](https://beatsaver.com/)

Entrambe hanno un pulsante OneClick™ che installa facilmente quella canzone sul tuo Quest. Puoi passare tra questi siti web usando l'icona del globo in alto a destra alla finestra del browser.

Un modo facile per scaricare diversi tipi di canzoni è usare `Syncsaber`, puoi accedervi andando in BMBF sul tuo Quest e cliccando la scheda chiamata `Syncsaber`. Qui puoi scaricare le canzoni con il click di un pulsante, puoi scegliere tra diverse "impostazioni". Per esempio puoi scaricare le 20 canzoni migliori nella sezione "hot" di [Beatsaver](https://beatsaver.com/) o le 50 canzoni classificate più difficili.

Un altro metodo è usare la funzionalità `Segnalibro` su [Beastsaber](https://bsaber.com/). Dopo aver creato un profilo puoi cliccare su una piccola icona del segnalibro su una canzone e se poi elimini tutte le canzoni dal Quest puoi riscaricare quelle col segnalibro con OneClick™.

### Usare il tuo PC
Se non puoi installare le canzoni nel tuo Quest, puoi installare le mappe usando il tuo computer similmente all'installazione delle mod.

1. Visita [BeastSaber](https://bsaber.com/) o [BeatSaver](https://beatsaver.com/) sul tuo computer
2. Scarica la zip
3. Segui i passaggi di [Installazione di mod usando il tuo PC](#using-your-pc) fino alla schermata di caricamento dei file.
4. Trascina e rilascia la zip della mappa e dovrebbe esser installata!

Se l'interfaccia web non carica, [clicca qui](#bmbf-web-interface-not-loading) per alcuni passaggi di risoluzione dei problemi.

:::tip Puoi scaricare anche le playlist allo stesso modo. You can find various playlists on [Beastsaber](https://bsaber.com/category/playlists/) or various community discords. You can also make your own using [BMBF Manager](https://github.com/ComputerElite/BM#bmbf-manager) or [Playlist Editor Pro](https://beatsaberquest.com/playlisteditor-pro/).

If you want to test a map you have created see the [Testing on a Quest](/mapping/#testing-on-a-quest) Section in the Mapping Wiki section for steps on packing it up for testing! :::

## Installing Models
Join the [Qosmetics Community](https://discord.gg/qosmetics) to change how your menu title, sabers, bloqs or walls look in-game!

## Useful Links

* [Qosmetics Community](https://discord.gg/qosmetics) - Server dedicated to making and using sabers, bloqs, and walls for Quest.
* [Qosmetics Creation Guides](https://github.com/RedBrumbler/Qosmetics/wiki) - Guides to create your own custom sabers, bloqs, and walls for Quest.
* [Questboard website](https://questmodding.com) - A place to get Beat Saber related news and info along with the latest mods releases!
* [Questboard discord server](https://discord.gg/P7sUKVnP) - A quest community to hangout and talk about Beat Saber related stuff, you can also get a role to get notified when a new mod gets released!
* [Fixing Out of Sync Audio](https://bsaber.com/quest-out-of-sync/)
* [ScoreSaber](https://new.scoresaber.com/quest) - In-game leaderboards for custom songs

## Troubleshooting
:::warning I watched a video tutorial on YouTube, but I got stuck/it didn't work. What gives? We at BSMG **strongly** advise against using any video tutorials for modding. Often, we find that they are either outdated or contain incomplete, erroneous, or straight up incorrect information.

Instead, you should follow the written guides here on the wiki or seek out help in the [BSMG Discord](https://discord.gg/beatsabermods). :::

### Adding mods from beatmods.com or models from modelsaber.com does not work
The reason adding mods from [BeatMods](https://beatmods.com/) or models from [ModelSaber](https://modelsaber.com/) doesn't work is because those mods and models are for PC Only.

Get Quest compatible Mods from [QuestBoard](https://www.questmodding.com/) or `#quest-mods` in the Beat Saber Modding Group Discord, with Quest compatible sabers, bloqs, and walls in the [Qosmetics Community](https://discord.gg/qosmetics). Once you have your mod or model zip use the [BMBF Web Interface](#using-your-pc) to install it.

### Sideloading BMBF failed
When sideloading BMBF you get the error `INSTALL_FAILED_UPDATE_INCOMPATIBLE: Package com.weloveoculus.BMBF
signatures do not match the previously installed version; ignoring!`

You will need to uninstall the BMBF version on your Quest. You can do this from SideQuest's `My Apps` menu.

### Core mods don't work

If you are having problems with core mods, please verify that you are not trying to use any outdated mods. Any mod made for a previous game version is considered outdated. Once you have removed them:

1. Go to `Tools`
2. Click `exit BMBF`
3. Open BMBF again
4. Go to `Tools` again
5. Click `Quick fix`
6. Go to the `Browser` section of the BMBF app.
7. Click the small globe icon in the top right-hand corner
8. Click `QuestBoard`
9. Click `Download Mods`
10. Scroll down and click `Download All Core Mods`
11. Click `Sync to Beat Saber`

---

### BMBF web interface not loading
If your BMBF Web Interface is not loading, be sure that you're typing the IP from the tools tab into your browser on your computer that's on the same network. Make sure that:

1. Your IP is not `127.0.0.1`, if that shows up try rebooting your headset and/or router.
2. BMBF is open in the headset
3. There is `http://` at the beginning of the link, not `https://`
4. You have `:50000` at the end of your link
5. Your PC and Quest are on the same wifi network
6. Your IP is hasn't changed as it changes from time to time

Se niente di tutto ciò funziona, riavvia il tuo Quest e riesamina l'elenco.

---

### BMBF non carica la configurazione dopo alcuni minuti
Questo potrebbe dipendere dall'uso di BMBF su una versione di gioco per cui non è stato creato. Come usare BMBF per la versione `1.13.0` di Beat Saber, quando la versione di gioco installata sull'headset è la `1.12.2`.  
Se la versione di gioco corrisponde a quella per cui la pagina di rilascio di BMBF dica sia stato creato, prova a riavviare il tuo headset. Se ancora non funziona usa l'[Interfaccia Web di BMBF](#using-your-pc) e clicca `Soluzione Rapida` nella scheda degli Strumenti.

### Beat Saber è nero all'avvio
Apri la libreria sul tuo Quest. Clicca i tre puntini vicini a Beat Saber e poi clicca `Autorizzazioni`. Nel menu che compare, abilita i permessi di archiviazione e prova a riavviare il gioco.

---

### Le Mie Sciabole e le Mie Mod non si abilitano/non funzionano
Questo potrebbe dipendere dall'avere un'App BMBF obsoleta, scarica l'ultima [Release di BMBF](https://bmbf.dev/stable). If the BMBF version for your Beat Saber is not there then please wait a while for the unicorns to update BMBF.

* If your mod is supposed to be compatible with your version of BMBF, then make sure there is no folder separating the contents of the .zip file.
* If your level doesn't load then try installing mapping extensions from #quest-mods. It may also require the mod Noodle Extensions which isn't on Quest yet.
* If your BMBF is on the latest version and mods wont be enabled in game, uninstall Beat Saber with the uninstall BS button in the BMBF Tools tab then reinstall and remod.
* In very very very rare cases, BMBF does not have file permissions to copy mods into the right location. Check in SideQuest to make sure BMBF has file permissions.

---

### Beat Saber is crashing
If your game is crashing when doing something, disable your mods one by one, running your game each time to see if the issue is fixed before asking for help in a support channel.

### I only see a white screen when i open BMBF
If you only see a white screen when you open BMBF from unknown sources, restart your quest and then it should be fixed

### My Beat Saber gets 3 dots when I launch
If your Beat Saber is getting 3 dots when launching make sure that:

1. You launched and played one song before modding the game
2. You're not using a pirated version of the game
3. Make sure you're using the latest version of BMBF
