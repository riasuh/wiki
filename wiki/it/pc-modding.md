---
sidebar: auto
---

# Modding su PC

## Prefazione

::: DISCLAIMER di pericolo Scegliendo di usare le mod, comprendi che:

* Potresti sperimentare problemi inesistenti nel gioco vanilla. 99,9% di bug, arresti anomali e lag sono dovuti alle mod.
* Le mod sono soggette alla corruzione da aggiornamenti e ciò è normale; sii paziente e rispettoso quando succede, poiché i modder sono volontari con una vita reale.
* Beat Games non cerca intenzionalmente di corrompere le mod. Desiderano lavorare sul loro codice e talvolta questo corrompe le mod, ma non vanno in giro a ucciderle.

Non attaccare gli sviluppatori del gioco per problemi relativi alle mod, e viceversa; i modder e gli sviluppatori del gioco sono due gruppi separati. Semplicemente, non fare l'idiota, ok? :::

::: avviso RIMANI AL SICURO INSTALLANDO LE MOD Beat Saber non ti chiederà **MAI** di eseguirlo come Amministratore.

Se hai scaricato e installato una mod e ottieni il prompt di Controllo del Profilo Utente, **NON** cliccare accetta, e sei pregato di segnalarlo. Ciò che hai installato è una mod dannosa!

Se non sei sicuro che qualcosa che hai installato sia o meno un malware, ***sei pregato di chiedere a qualcuno nel nostro discord***. :::

Beat Saber supporta nativamente le canzoni personalizzate, quindi se è tutto ciò che stai cercando, non richiedere altre mod! È saggio installare invece `SongCore`, poiché questa mod si espande sulla funzionalità del gioco di base per migliorare i tempi di caricamento e fornire funzionalità per altre mod come il download integrato, le classifiche personalizzate, le playlist, etc.

::: attenzione Questa guida è per il modding PC su Windows.  
Se hai un Quest, vedi la [pagina di Modding su Quest](/quest-modding.md).  
Se sei su Linux, dai un'occhiata alla [pagina di Linux](/modding/linux.md) o a [Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) :::

Se incontri problemi in qualsiasi momento, sei pregato di andare alla [pagina del supporto](./support) e vedere se puoi identificare cosa è andato storto prima di chiedere nel server di Discord. Ci sono possibilità, che la risposta sia su quella pagina!

::: attenzione Ho guardato un tutorial video su YouTube, ma mi ci sono bloccato/non ha funzionato. Che succede? Noi a BSMG sconsigliamo **fortemente** l'uso di tutorial video per il modding. Spesso, troviamo che siano obsoleti o contengano informazioni incomplete, erronee, o direttamente errate.

Invece, dovresti seguire le guide scritte qui sulla wiki o cercare aiuto nel [Discord di BSMG](https://discord.gg/beatsabermods). :::

## Installatori

### Assistente Mod
> **QUESTO È L'INSTALLATORE DI MOD CORRENTEMENTE CONSIGLIATO.**

__**Esegui il gioco almeno una volta**** prima di provare a moddare il gioco! Questo si applica anche alla reinstallazione del tuo gioco.

Un semplice Installatore di Mod di Beat Saber simile al gestore delle mod, ma con funzionalità aggiuntive come la rimozione delle mod e il controllo della versione! Ottieni [Assistant](https://github.com/Assistant/ModAssistant/releases/latest) su GitHub

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Come ottenere altre canzoni
::: suggerimento Gran parte delle mappe nei filtri di ordinamento "Migliori", "Classifica", "Download" o "Riprodotte" sono state create prima che fossero stabilite buone pratiche di mappatura. Prova a scaricare le canzoni rilasciate tra il tardo 2019 e ora per una migliore esperienza con i livelli personalizzati. :::

::: attenzione È una bella idea fare il backup della tua cartella `CustomLevels` periodicamente poiché esiste la piccola posibilità che sarà ripristinata se il gioco si aggiorna!

Questa cartella si trova nell'installazione del tuo gioco: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### Downloader Integrato
La mod `BeatSaver Downloader` ti consente di scaricare mappe nel gioco usando il pulsante del menu `ALTRE CANZONI` sulla schermata del menu `MOD`. Questo estrae le mappe direttamente da [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) è la repository principale delle canzoni personalizzate create dalla community. Molti altri strumenti e siti migliorano l'esperienza di scaricare canzoni personalizzate, ma questo sito è dove sono memorizzate. Per installare le canzoni scaricate dal sito, decomprimile in una cartella e posizionale in `Beat Saber/Beat Saber_Data/CustomLevels`. Puoi anche usare la mod del downloader integrato, o la funzionalità OneClick™ di Mod Assistant.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) è un sito che prova ad aiutare a trovare fantastiche mappe per giocare più facilmente. It does this by categorizing the thousands of songs on BeatSaver and lets you sort by a song's genre and many other attribute tags. Ha anche una funzionalità social completa in cui i giocatori possono recensire le canzoni e commentarle. Una delle funzionalità più usate è "Curatore Consigliato" in cui una squadra gioca gran parte delle canzoni rilasciate ogni giorno e consiglia quelle che spiccano, facendotele [scaricare automaticamente nel gioco](https://bsaber.com/beatsync/).

### App di Gestione della Canzone

Non ci sono app di gestione delle canzoni funzionanti al momento disponibili.

### Playlist
Devi installare la mod [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest).

Poi puoi:

* Usare lo strumento `Install Playlist` nella scheda delle Opzioni del Mod Assistant.
* Posizionare il file della playlist in `Beat Saber/Playlists`, selezionarlo nel gioco, poi cliccare scarica tutte le canzoni.

Dovresti vedere la playlist vicino all'album dei Livelli Personalizzati nel gioco. La mod supporta anche la gestione delle playlist nel gioco.

## Cartella d'Installazione
_Dov'è installato Beat Saber?_

### Posizione Predefinita
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Altre Posizioni
**Se hai spostato la tua cartella di installazione a un'unità differente, potrebbe trovarsi nella posizione sotto.** Sostituisci la lettera dell'unità `F` con l'unità in cui è installato il tuo gioco.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Installazione Manuale
Un installer di mod è il modo consigliato per installare le mod. Vedi la sezione [sopra](#installers). Se hai aggiustato il gioco e devi solo installare le mod non disponibili nell'installer, salta al passaggio 4.

::: avviso RIMANI AL SICURO INSTALLANDO LE MOD Moddare il tuo gioco con mod non verificati come quelle trovate nel canale `#pc-mods` presenta dei rischi, inclusa la possibilità di software dannosi che agiscono come una mod regolare.

Beat Saber non ti chiederà **MAI** di eseguirlo come Amministratore.

Se hai scaricato e installato una mod e ottieni il prompt di Controllo del Profilo Utente, **NON** cliccare accetta, e sei pregato di segnalarlo. Se non sei sicuro che qualcosa che hai installato sia o meno un malware, ***sei pregato di chiedere a qualcuno nel nostro Discord***. :::

**Esegui il gioco almeno una volta** prima di provare a moddare il gioco! Questo si applica anche alla reinstillazione del tuo gioco.

### Installa BSIPA

1. Scarica [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases).
2. Naviga alla tua [cartella d'installazione](#install-folder) ed estrai i contenuti di BSIPA in essa. ![Cartella Vuota](~@images/beginners-guide/directory-clean.png "Cartella Vuota") ![Cartella Ipa](~@images/beginners-guide/directory-ipa.png "Cartella Ipa")
3. Clicca due volte IPA.exe per patchare il gioco. Ogni mod nella cartella `Plugins` non sarà caricata all'avvio del gioco. Se ci sono errori, probabilmente non hai eseguito correttamente il passaggio 2. ![Cartella Patchata](~@images/beginners-guide/directory-patched.png "Cartella Patchata")

### Installare le Mod

4. Scarica le mod che vuoi installare, che siano da GitHub, il [Discord BSMG](https://discord.com/invite/beatsabermods), il canale `#pc-mods`, [BeatMods](https://beatmods.com/#/mods) o altre fonti. **Assicurati di scaricare ogni dipendenza richiesta dalla mod.** ![Plugin della Cartella](~@images/beginners-guide/directory-plugins.png "Plugin della Cartella")
5. Alcune mod hanno istruzioni d'installazione, altre no. Generalmente puoi solo trascinare e rilasciare i contenuti zip nella tua cartella d'installazione di Beat Saber, e i file dovrebbero andare nelle cartelle corrispondenti.

## Come disinstallare le mod
Rimuovi il dll dalla cartella `Plugins`, o clicca il pulsante `Disinstalla` nel Mod Assistant.

## Dove andare da qui

* [Impugnature e Trucchi](./grips-and-tricks.md)
* [Creare Beatmap](/mapping/)
* [Sciabole Personalizzate](/models/custom-sabers.md)
* [Avatar Personalizzati](/models/custom-avatars.md)
* [Piattaforme Personalizzate](/models/custom-platforms.md)
* [Giocare Personalizzate in Multigiocatore](https://discord.com/invite/gezGrFG4tz)
* [Creare Mod](/modding/)

## Hai domande?
Visita i canali di supporto nel [Discord BSMG](https://discord.gg/beatsabermods)!
