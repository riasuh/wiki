---
sidebar: auto
---

# Supporto

## Tabella dei Contenuti

0. [Aggiornamenti](#_0-updates)
1. [Nessuna mod?](#_1-no-mods)
2. [Problemi di Gioco Dopo il Modding](#_2-game-issues-post-modding)
3. [Domande Comuni](#_3-common-questions)
4. [Risoluzione di Problemi Vari](#_4-miscellaneous-troubleshooting)
5. [Riscontri Ancora Problemi](#_5-still-having-issues)

## 0. Aggiornamenti
Dopo un aggiornamento, il canale `#modding-announcements` del Discord di BSMG dovrebbe avere le informazioni più aggiornate sullo stato delle mod. Seguono altre istruzioni dettagliate della procedura più comune.

### L'aggiornamento ha corrotto le mie mod
**Esegui il gioco una volta** al nuovo aggiornamento. Poi, reinstalla le tue mod usando un installatore collegato nella [guida per principianti](/beginners-guide), come Mod Assistant.

## 1. Nessuna mod?

### Domande Varie

#### 1.1 Nessuna mod compare su una nuova copia del gioco
Prima, assicurati che quanto segue sia corretto:

* **Hai eseguito il gioco una volta prima di installare le mod**. BSIPA rimuove tutte le mod alla prima esecuzione di un nuovo aggiornamento per prevenire che le vecchie mod corrotte carichino su una nuova versione. Reinstalla le mod se questo è il caso.
* Steam/Oculus sta lanciando Beat Saber dalla **stessa installazione** in cui si trovano le mod. *es. le mod sono sull'unità D ma Steam si sta avviando dall'unità C.* Imposta la posizione d'installazione corretta nell'installatore di tua scelta.
* Se hai installato le mod manualmente, assicurati di aver incluso tutti i file dal download e inseriscile nelle cartelle corrette, nonché nelle proprie dipendenze.

#### 1.2 Avevo installato delle mod su una vecchia versione, ma dopo un aggiornamento non carica nulla
Se i dettagli nella suddetta sezione 1.1 sono corretti, prova le seguenti soluzioni, in ordine decrescente.

##### Soluzione 1

* Aggiorna BSIPA all'ultima versione (su Mod Assistant o manualmente)
* Vai alla tua cartella di Beat Saber
* Esegui `IPA.exe`

##### Soluzione 2 (Solo Steam)

* [Verifica i tuoi file di gioco](#verify-game-files-for-steam)
* Aggiorna BSIPA all'ultima versione
* Vai alla tua cartella di Beat Saber
* Esegui `IPA.exe`

##### Soluzione 3

* Vai alla tua cartella di Beat Saber
* Crea un backup della cartella `UserData` (facoltativo)
* Elimina UserData

::: attenzione Questo ripristinerà le impostazioni di tutte le mod! :::

##### Soluzione 4

* Esegui un'[Installazione Pulita](#clean-installation)

#### 1.2 Mod Assistant non sembra installare alcuna mod
L'installatore scarica le mod in `Beat Saber/IPA/Pending`, BSIPA sposta questi file alla cartella di root quando avvii il gioco. Se la cartella Plugins del tuo gioco è ancora vuota in seguito, esegui nuovamente `IPA.exe` e assicurati che nulla ne stia impedendo l'esecuzione, es. `Antivirus, permessi d'amministratore, etc.`

## 2. Problemi di Gioco Dopo il Modding

### Il Gioco Non Si Avvia

#### 2.1 Errore GetThreadContext Fallito
Se una finestra appare dicendo `GetThreadContext Fallito` e/o senti un suono d'errore di Windows, potresti avere dei software sul tuo PC che corrompe le mod di Beat Saber. Molti software antitruffa di terze parti come ESEA e FaceIt interrompono BSIPA dall'applicare mod a Beat Saber, anche quando non è in esecuzione. Alcuni software di antivirus esibiscono anch'essi un comportamento simile.

Per risolvere questo problema:

1. Disinstalla il software di anticheat.
2. Riavvia il tuo PC.
3. Controlla se c'è ancora qualche residuo del software nelle tue cartelle di `AppData`.
4. Esegui il gioco. Se i problemi persistono, allora prova quanto segue: `Nota Aggiuntiva: Il problema può continuare a persistere a causa della mancanza di permessi o eccezioni, qualsiasi programma che può bloccare BSIPA, o programmi contrassegnati come sospetti possono far persistere questo problema` Steam: [Verifica i File di Gioco di Steam](#verify-game-files-for-steam) Oculus: Esegui un'[Installazione Pulita](#clean-installation)

Questo dovrebbe risolvere il problema.

#### 2.2 Congelato all'Avvio
Se il gioco è congelato alla schermata Salute e Sicurezza, o si vede un avatar in posa a T senza controllo del gioco, [verifica i tuoi file](#verify-game-files-for-steam) se hai il gioco su Steam, o reinstalla il gioco su Oculus Home. Fai riferimento all'[Installazione Pulita](#clean-installation)

Questo sembra succedere aggiornando Beat Saber, avendo precedentemente installato delle mod.

### Problemi di Framerate

#### 2.3 Il gioco va a tratti in modo insopportabile dopo aver installato le mod
Se il gioco lagga così tanto da poter a malapena cliccare il pulsante `Continua` sulla schermata Salute e Sicurezza, verifica i file se hai il gioco su Steam o reinstalla il gioco su Oculus Home. Fa lo stesso se non si avvia affatto e non mostra alcun messaggio d'errore provando ad avviare il gioco.

If that didn't solve the issue, then check section [2.4 Improving framerate](#_2-4-improving-framerate)

#### 2.4 Migliorare il Framerate
Se [2.3](#2-3-the-game-stutters-unbearably-after-installing-mods) non ha migliorato i tuoi fps, il tuo PC potrebbe semplicemente star facendo fatica a tenersi al passo con lo stress causato dalle mod. Ecco alcune cose che puoi fare per migliorare il framerate, in nessun ordine particolare:

* Verifica se NVIDIA GEFORCE EXPERIENCE ha impostato la scala di rendering per Beat Saber oltre il predefinito di 1.0. Potrebbe averlo impostato a un numero maggiore a 1,4 o 1,8, il che aumenta significativamente il carico della GPU.
* Usa un avatar personalizzato meno complesso.
* La sciabola personalizzata **Plasma Katanas** contiene tonnellate di eventi personalizzati, noti per introdurre lag se perdi.
* Camera2 e CameraPlus possono esser molto pesanti, specialmente se hai molte telecamere o aumenti il FOV.
* Disattiva la Scala di Rendering, l'Anti-Aliasing, specchio, nebbia, etc. nelle impostazioni di base del gioco.
* Per i giocatori con Oculus Rift (CV1): considera di usare 2 sensori invece che oltre 3.
* Riduci il conteggio totale delle tue mod e canzoni.
* Esegui un'[Installazione Pulita](#clean-installation) dei file di gioco.
* Il basso framerate può anche esser causato da qualcosa che va storto nella cartella dei dati della tua applicazione, fai riferimento all'[Eliminazione della Cartella di BeatSaber Nel Tuo AppData](#deleting-your-save-in-appdata)
* Disabilita i contatori di Counters+ come contatori di punteggio e la velocità d'oscillazione, poiché possono esser pesanti.
* HTTPStatus and DataPuller can cause lag spikes. Prova senza questa mod a vedere se i picchi di lag spariscono.

Il VR usa molto intensivamente la CPU, specialmente se aggiungi le mod. Se non riesci a eseguire il gioco con le mod che vuoi, considera di aggiornare il tuo hardware. Nota che Beat Saber non utilizza molto la GPU, essendo un gioco visivamente abbastanza semplice.

## 3. Domande Comuni

### Varie

#### 3.1 Menu Vuoto, Nessun Pulsante
Se la tua finestra principale di gioco è vuota, il tuo file di salvataggio potrebbe essersi corrotto. Per risolverlo, fai riferimento all'[Eliminazione della Cartella di BeatSaber Nel Tuo AppData](#deleting-your-save-in-appdata)

::: attenzione Questo eliminerà tutti i tuoi punteggi e statistiche locali. :::

#### 3.2 Come posso usare la mod `x`?
Se stai usando Mod Assistant, clicca la mod e premi il pulsante "Info Mod". [BeatMods](http://beatmods.com) include anche un pulsante "Altre Info" per ogni mod.

#### 3.3 Problemi di Vibrazione
Gameplay Modifiers Plus aveva un interruttore per abilitare/disabilitare la vibrazione del controller. Se lo hai disabilitato e poi hai rimosso la mod, dovrai modificare il file dei dati di salvataggio che scrive manualmente. Apri `%appdata%\..\LocalLow\Hyperbolic Magnetism\Beat Saber\settings.cfg` e imposta `controllersRumbleEnabled` a `true`.

Se questa non è la causa dei tuoi problemi di vibrazione e quanto segue è vero relativamente le tue sensazioni tattili:

* le tattili sono minuscole
* non c'è alcuna vibrazione colpendo più blocchi
* c'è un lieve ritardo facendo toccare le sciabole
* stai usando i controller touch di Oculus

Poi c'è una buona probabilità che Beat Saber stia sovraccaricando il controller USB della tua scheda madre. Oculus divora la larghezza di banda del tuo controller USB e gran parte delle schede madri hanno un controller molto economico. Beat Saber le spinge molto più di qualsiasi altro gioco, ecco perché gli altri giochi e menu potrebbero andare bene. Non esiste una soluzione chiara, quindi prova quanto segue:

* Mischia il sensore e i cavi USB HMD su diverse porte
* Scollega i dispositivi USB non necessari
* Acquista un hub PCI-E USB
* Usa `-vrmode oculus` se stai usando SteamVR per bypassarlo e usa invece la SDK di Oculus

### Avatar Personalizzati

#### 3.4 Avatar Personalizzati (Non) Mostrati In Gioco
Clicca il pulsante **Home** sulla tua tastiera con il gioco a fuoco per attivare la visibilità nell'auricolare.

#### 3.5 I Miei Avatar Sono Corrotti
Assicurati che la tua mod degli avatar personalizzati sia propriamente installata e aggiornata, assicurati che anche le tue dipendenze lo siano. Potresti avere un avatar corrotto/rotto, il che potrebbe rompere tutti i tuoi avatar allo stesso modo, con canzoni e sciabole.

### Canzoni Personalizzate

#### 3.6 Le Mie Canzoni Sono Mancanti
Assicurati che le tue canzoni siano nella tua cartella `CustomLevels`, situata in `Beat Saber/Beat Saber_Data/`. È da qui che il gioco legge nativamente le canzoni personalizzate.

**Non** posizionare canzoni nella vecchia cartella `Beat Saber/CustomSongs`. Questa posizione è obsoleta, poiché il formato per le canzoni personalizzate è cambiato. Se hai mappe nel vecchio formato (file `.json` e `.ogg` invece di `.dat` e `.egg`), lasciali nella vecchia cartella `Beat Saber/CustomSongs`. Dovrai riscaricarli da BeatSaver.

Altrimenti, puoi convertirli manualmente usando [Song Converter](https://github.com/lolPants/songe-converter), tuttavia, non riceverai alcun aiuto con questo metodo e dovrai compilare da solo il programma.

#### 3.7 Pulsante di Gioco Ingrigito
Clicca il pulsante del punto interrogativo blu lucido (?) in alto a destra. Questo dovrebbe dirti che mod sono necessarie per riprodurre la canzone, quali sono mancanti e dovresti installare. Se ancora non funziona, prova a reinstallare la mod necessaria. Altrimenti, prova un'[Installazione Pulita](#clean-installation).

#### 3.8 I dettagli della mappa caricano all'infinito
Se questo si verifica solo su certe mappe, potresti mancare delle mod necessarie o quei file di canzoni sono corrotti. Se si verifica su tutte le tue mappe, elimina la tua cartella dei `Plugins` e reinstallali.

### CameraPlus

#### 3.9 CameraPlus Non Funziona/Supera la Schermata di Salute
Assicurati che l'impostazione di gioco per "Smooth Camera" sia disattivata nelle tue impostazioni di gioco. Se non funziona, prova a reinstallarlo con le dipendenze associate.

#### 3.10 La mia vista desktop occupa solo una piccola sezione del mio schermo
La tua schermata di CameraPlus non sta riempendo il tuo schermo. Trascina l'angolo per adattarlo allo schermo, o clicca con il destro sulla finestra e clicca "Adatta alla Tela".

### Downloader di BeatSaver

#### 3.11 Pulsante Altre Canzoni del Downloader di BeatSaver
**Il pulsante Altre Canzoni si trova nel menu principale a sinistra, sotto al testo Mods.** Se il pulsante per Altre Canzoni è ingrigito, assicurati prima che tutte le tue canzoni siano caricate, come visto nella barra di progresso arcobaleno nel menu principale. Se il tuo menu Mods non c'è, assicurati che le tue mod e dipendenze stiano funzionando e siano propriamente installate, fai riferimento alla sezione [Nessuna Mod?](#_1-no-mods).

#### 3.12 Nel Menu Altre Canzoni Non Compare Nulla
Le probabili cause per cui il Downloader di BeatSaber non stia funzionando sono:

1. Prima, assicurati che tutte le tue canzoni siano state caricate, altrimenti il pulsante Altre Canzoni sarà ingrigito.
2. Il tuo antivirus o firewall sta bloccando l'accesso a BeatSaver.
3. Hai superato il limite di utilizzo di BeatSaber e dovrai attendere prima di riprovare.

### Codici d'Errore del Multigiocatore
Ecco un elenco dei codici d'errore noti, cosa significano e cosa puoi fare per risolverli.

<!-- Disable line length rule because of table -->
<!-- markdownlint-disable MD013 -->
| Code&nbsp; | Descrizione                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
|:---------- |:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| CFR-1      | Errore Sconosciuto. Prova a riavviare il gioco.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| CFR-2      | La connessione multigiocatore è stata annullata.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| CFR-3      | Il server è irraggiungibile. Potrebbe esserci un problema con la tua connessione a internet o con i server relè di Beat Saber. Ricontrolla di non essere offline e che il tuo firewall consenta a Beat Saber di connettersi a internet. <details><summary>**Informazioni di Background**</summary>Beat Saber Multiplayer è in pari, connettendoti direttamente con ogni giocatore nella lobby. Quando ciò è impossibile, Beat Saber avvia un server di "relè" per inviare i dati. Questo errore significa che entrambi questi metodi sono falliti.</details> &nbsp; Questo può anch'esser causato dall'uso di emoji o caratteri speciali nella tua username. |
| CFR-4      | Il server esiste già.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| CFR-5      | Il server non esiste. La lobby a cui ti stavi connettendo potrebbe aver chiuso mentre ti univi.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| CFR-6      | Il server è pieno. Scegli una lobby differente.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| CFR-7      | Sei su una versione del gioco non supportata dai server.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| CFR-8      | La password della lobby è errata. Ricontrolla di star inserendo quella corretta.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |
| CFR-9      | I server di matchmaking eseguiti da Beat Saber, che tengono traccia delle lobby pubbliche aperte e private, sono offline. Riprova più tardi.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| CFR-10     | La chiave della tua sessione da Steam od Oculus non è valida. Se stai giocando su Quest e hai moddato il tuo gioco, dai un'occhiata a questa [risposta della FAQ](/faq/README.md#does-multiplayer-have-crossplay) per risolvere. Altrimenti, stai usando una copia piratata del gioco, che non è supportata.                                                                                                                                                                                                                                                                                                                         |
| CFR-11     | La tua connessione a internet è offline.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
<!-- markdownlint-enable MD013 -->

## 4. Risoluzione di Problemi Vari

### Comprendere i Registri
Se sei su Steam puoi andare a
> Beat Saber > Proprietà > Generali > Aggiungi `--verbose` al campo delle opzioni d'avvio

Se sei su Oculus, dovrai allora cliccare con il Destro su Beat Saber.exe e creare una scorciatoia. Modifica l'obiettivo per aggiungere "--verbose" alla fine di esso. es. `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\Beat Saber.exe" --verbose`

Dopo aver aggiunto verbose al tuo gioco, si spera che mostrerà ogni errore relativo ai tuoi avatar, sciabole e canzoni

* Questo potrebbe non mostrare il 100% delle volte gli avatar e le sciabole e potresti dover rimuovere tutti i tuoi avatar/sciabole e provarli a uno a uno, per scoprire quale corrompe il gioco.

Questi messaggi sono scritti anche a `Beat Saber/Logs`.

Un elenco di eccezioni comuni si può trovare [qui](./exceptions.md).

### Verifica i File di Gioco Per Steam
Per verificare l'integrità dei file di gioco, segui questi passaggi:

1. Assicurati che SteamVR sia chiuso poiché, altrimenti, non ti permetterebbe di verificare i tuoi giochi.
2. Vai alla tua libreria di Steam e trova Beat Saber
3. Clicca con il destro su Beat Saber e clicca su Proprietà
4. Vai alla scheda dei "File Locali" nelle proprietà
5. Seleziona l'opzione "Verifica Integrità dei File di Gioco.
6. Fagli concludere la verifica e il download di qualsiasi file mancante e dovresti aver risolto.

Ecco una [Videoguida](https://www.youtube.com/watch?v=EBFfT4-ZiIc), sebbene sia sulla vecchia UI di Steam, i passaggi sono ancora gli stessi.

### Installazione Pulita

1. (Facoltativo) Esegui il backup dei tuoi contenuti personalizzati scaricati creando una copia delle seguenti cartelle:

* `Beat Saber\Beat Saber_Data\CustomLevels`
* `Beat Saber\CustomSabers`
* `Beat Saber\CustomPlatforms`
* `Beat Saber\CustomNotes`
* `Beat Saber\CustomAvatars`

2. **Elimina l'INTERA Cartella di Beat Saber.** Questo è diverso dalla disinstallazione del gioco su Steam, poiché questi metodi non rimuoveranno i file che non erano parte del gioco.

> Steam: ``\steamapps\common\Beat Saber\`
  Oculus:``\hyperbolic-magnetism-beat-saber\`

3. Reinstalla il gioco tramite il negozio di Steam o di Oculus
4. **Prima di moddare, avvia il gioco una volta**
5. Esegui Mod Assistant, installa le tue mod e avvia il gioco.

(Facoltativo) Se vuoi effettuare un ulteriore passaggio, fai riferimento all'[Eliminazione della Cartella di BeatSaber Nel Tuo AppData](#deleting-your-save-in-appdata)

### Eliminare il Tuo Salvataggio in AppData
Questo eliminerà i tuoi punteggi e dati locali, ma non le statistiche della tua classifica/ScoreSaber personalizzata. Puoi trovare la cartella a
> `%appdata%/../locallow/hyperbolic magnetism/beat saber`

Copia e incolla tutto dall'interno della barra superiore e incollalo nella tua barra degli indirizzi in esplora file ed eliminala.

Puoi anche arrivare a questa cartella mostrando gli elementi nascosti e navigando nella tua
> Utenti > "USER" > AppData > LocalLow > Hyperbolic Magnetism > beat saber

<YouTube url='https://youtu.be/ONxJcD3Ir3Q' />

::: attenzione Eliminare questa cartella in AppData, eliminerà anche i tuoi punteggi e statistiche locali. :::

#### Misure Disperate
::: attenzione Disabilitare il tuo antivirus comporta rischi per la sicurezza, assicurati di sapere cosa stai facendo (es. non scaricare o aprire file sospetti quando è disattivato) e non dimenticarti di riabilitarlo non appena terminati questi passaggi. :::

* Assicurati che il tuo utente corrente **sia un amministratore**
* **Disattiva** il tuo antivirus (almeno per ora)
* Assicurati di avere i permessi per creare cartelle e modificare file nell'unità disco/nel tuo pc (da ciò che ho sentito, un aggiornamento di Windows ha recentemente causato problemi alle persone)
* Assicurati che i tuoi driver siano aggiornati
* Controlla che il problema non si trovi nel tuo auricolare o sistema operativo o hardware/software
* Controlla la tua connessione a internet e che nulla stia bloccando qualsiasi cosa sia correlata al modding di BeatSaber e Steam, etc.

## 5. Riscontri Ancora Problemi
Se questa pagina non copre le basi, sentiti libero di fare una domanda su Discord! Per aumentare le possibilità che tu riceva risposte alle tue domande, considera quanto segue:

* Sei pregato di usare i canali corretti, `#pc-help` per il supporto mod per pc e `#quest-help` per il supporto mod per Quest. Usa `#pc-3d-modeling` e `#quest-3d-modeling` per le domande sulla **creazione di avatar, piattaforme, note o sciabole proprie**, e `#mapping-discussion` per le domande sulla **creazione di mappe.**
* Sii educato e rispettoso
* Descrivi il tuo problema in dettaglio. "Non ha funzionato" è tanto descrittivo quanto dire al tuo medico che non ti senti bene. Cosa non funziona e cosa hai provato? Ci sono dei messaggi che compaiono su schermo? Il tuo intero schermo è diventato viola luminoso?

::: tip NOTA Coloro che hanno il ruolo `Supporto` sono volontari che potrebbero scegliere di dare una mano nel loro tempo libero. Il ruolo di supporto consiste nel riconoscimento delle conoscenze e gli sforzi da loro messi in atto, ma non significa necessariamente che saranno lì ad aiutare solo perché sono online. :::

Crediti a Saber-Chan per il loro duro lavoro su questa pagina.
