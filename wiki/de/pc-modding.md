---
sidebar: auto
---

# PC Modding

## Vorwort

::: danger BITTE BEACHTE Wenn du Mods verwendest, verstehst du das:

* Du möglicherweise Probleme bekommst, die im normalen Spiel nicht existieren. 99,9% aller Fehler, Abstürzen und Verzögerungen passieren aufgrund von Mods.
* Mods werden durch Updates oft unbrauchbar und das ist normal - Bitte sei geduldig und respektvoll wenn dies passiert. Modder sind Freiwillige mit einem richtigen Leben.
* Beat Games versucht nicht mit Absicht Mods kaputt zu machen. Sie versuchen an der Code-Grundlage zu arbeiten welches manchmal Mods unbrauchbar macht. Dies geschieht aber nicht mit Absicht.

Bitte greife die Entwickler im Bezug mit Problemen bei Mods nicht an. Modder und Entwickler sind zwei verschiedene Gruppen. Sei einfach kein Trottel, ok? :::

:::warning BEI DER INSTALLATION VON MODS SICHER BLEIBEN Beat Saber wird **NIEMALS** fragen als Administrator zu starten.

Wenn du eine  Mod heruntergeladen und installiert hast und die Benutzerkontensteuerung erhältst, **klicke NICHT** auf "Akzeptieren" und melde dies bitte. Was du installiert hast, ist eine bösartige Mod!

Wenn du dir nicht sicher bist, ob du dir gerade Malware installiert hast, ***frage bitte jemanden in unserem Discord***. :::

Beat Saber ünterstützt von Haus aus Custom Songs. Wenn du also nur das haben willst, brauchst du keine Mods! Es ist empfehlenswert `SongCore` zu installieren, da diese Mod das Basisspiel mit einigen Funktionalitäten erweitert, wie verbesserte Ladezeiten. Es fügt Funktionalitäten für andere Mods ein, wie der In-Game Downloader, eigene Bestenlisten, Playlisten, usw.

::: warning Diese Anleitung ist für das PC-Modding in Windows.  
Hast du eine Quest, schau dir die[Quest Modding Seite](/quest-modding.md) an.  
Benutzt du Linux, schau auf der [Linux Seite](/modding/linux.md) oder[Beataroni](https://github.com/geefr/beatsaber-linux-goodies/#readme) nach. :::

Wenn du auf irgendwelche Probleme stoßen solltest, schaue bitte auf der [Support Seite](./support) nach und prüfe was falsch gelaufen ist, bevor du auf dem Discord Server nachfragst. Es kann gut sein, dass deine Frage dort beantwortet wird!

::: warning Ich habe ein Video Tutorial angeschaut, aber es hängt/hat nicht funktioniert. Was bedeutet das? Wir von BSMG raten **stark** davon ab, Video-Tutorials für Modding zu verwenden. Meistens ist es so, dass diese veraltet, unvollständig, irrtümlich oder einfach falsch sind.

Stattdessen solltest du den schriftlichen Anleitungen hier im Wiki folgen oder im [BSMG Discord](https://discord.gg/beatsabermods) nach Hilfe suchen. :::

## Installationsprogramme

### Mod Assistant
> **DIES IST AKTUELL DER EMPFOHLENE MOD INSTALLER.**

__**Starte das Spiel mindestens ein mal**** bevor du versuchst das Spiel zu modden! Das gilt auch, wenn du das Spiel neu installiert hast.

Ein einfacher Beat Saber Mod Installer, ähnlich dem Mod Manager, aber mit zusätzlichen Funktionen wie Mod-Entfernung und Versionskontrolle! Hol ihn dir auf [Assistant's GitHub Seite.](https://github.com/Assistant/ModAssistant/releases/latest)

![Mod Assistant](~@images/beginners-guide/modassistant.png)

## Wie bekomme ich mehr Songs
::: tip Die meisten Maps in den "Top All", "Rating", "Downloads" oder "Plays" Sortierfiltern wurden erstellt, bevor gute Mapping Praktiken eingerichtet wurden. Versuche Songs herunterzuladen, welche Ende 2019 und jetzt veröffentlicht wurden um die beste Erfahrung zu haben. :::

::: warning Es ist eine gute Idee den `CustomLevels` Ordner periodisch zu sichern, da eine kleine Chance besteht, dass dieser zurück gesetzt wird, wenn das Spiel ein Update hat!

Dieser Ordner befindet sich dort, wo dein Spiel installiert ist: `Beat Saber/Beat Saber_Data/CustomLevels` :::

### InGame Downloader
Die `BeatSaver Downloader` Mod erlaubt es dir Lieder im Spiel über den `MORE SONGS` Menü Knopf in dem `MODS` Menü Bildschirm herunterzuladen. Dieser lädt die Maps direkt von [BeatSaver](https://beatsaver.com)

### BeatSaver
[BeatSaver](https://beatsaver.com) ist die Haupt Datenbank an Custom Songs, welche von der Community erstellt wurden. Viele andere Tools und Webseiten verbessern die Erfahrung beim Herunterladen von Custom Songs. BeatSaver ist aber die Seite, auf der sie zur Verfügung gestellt werden. Um gedownloadete Songs von der Seite zu installieren, entpacke und platziere diese in `Beat Saber/Beat Saber_Data/CustomLevels`. Du kannst auch das eingebaute Downloader Plugin, BeatList oder das OneClick™ Install-Feature von Mod Assistant verwenden.

### Beast Saber
[Beast Saber](https://www.bsaber.com) (bsaber.com) ist eine Seite, die versucht, euch die Suche nach guten Maps zum Spielen zu erleichtern. Dies geschieht durch Kategorisierung der Tausenden von Songs auf BeatSaver und lässt diese nach dem Genre eines Songs und vielen anderen Attributen sortieren. Es besitzt auch ein soziales Feature, in der Spieler Songs bewerten und kommentieren können. Eines der meistgenutzten Funktionen ist die "Curator Recommended"-Funktion, bei der ein Team die meisten täglich veröffentlichten Songs durchspielen und die herausstechenden empfiehlt, so dass sie diese [automatisch im Spiel herunterladen können](https://bsaber.com/beatsync/).

### Song Management Apps

Zurzeit gibt es keine funktionierende Mod zum managen von Songs.

### Playlists
Du musst den [PlaylistManager](https://github.com/rithik-b/PlaylistManager/releases/latest) installieren.

Dann kannst du entweder:

* Das `Install Playlist` Tool in den Optionen des Mod Assistant verwenden.
* Platziere die Playlist-Datei in `Beat Saber/Playlists` und wähle diese im Spiel aus. Klicke dann auf Download.

Du solltest die Playlist jetzt neben den eigenen Songs im Spiel sehen. Der Mod unterstützt auch die Verwaltung von Playlisten im Spiel.

## Installationspfad
_Wo ist Beat Saber installiert?_

### Standard Installations-Ordner
|        |                                                                                      |
| ------ | ------------------------------------------------------------------------------------ |
| Steam  | `C:\Program Files (x86)\Steam\steamapps\common\Beat Saber\`                  |
| Oculus | `C:\Program Files\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

### Andere Installationspfade
**Solltest du Beat Saber auf ein anderes Laufwerk verschoben haben, könnte es sich an der unten angegebenen Stelle befinden:** Ersetze den Laufwerksbuchstaben `F` mit dem Buchstaben, wo Beat Saber installiert ist.
|        |                                                                       |
| ------ | --------------------------------------------------------------------- |
| Steam  | `F:\SteamLibrary\steamapps\common\Beat Saber\`                 |
| Oculus | `F:\Oculus\Software\Software\hyperbolic-magnetism-beat-saber\` |

## Manuelle Installation
Ein Mod-Installer ist die empfohlene Methode, um Mods zu installieren. Siehe den Abschnitt [oben](#installationsprogramme). Solltest du das Spiel geupdated haben und Plugins installiert werden müssen, die nicht im Mod Installer sind, springe zu Schritt 4.

::: Warnung, BLEIG SICHER, WENN DU MODS INSTALLIERST Das Modding des Spiels mit ungeprüften Mods, wie welche im `#pc-mods` Kanal birgen Risiken, einschließlich der Möglichkeit für böswillige Software, die wie eine reguläre Mod agiert.

Beat Saber wird dich **NIEMALS** bitten als Administrator zu starten.

Wenn du einen Mod heruntergeladen und installiert hast und diese nach der Benutzerkontensteuerung fragt, **klicke NICHT** auf "Akzeptieren" und melde dies bitte. Wenn du dir nicht sicher bist, ob das, was du installiert hast Malware ist, ***frag bitte in unserem Discord nach***. :::

**Starte das Spiel mindestens einmal** bevor du versuchst Mods zu installieren! Dies gilt auch für die Neuinstallation des Spiels.

### BSIPA installieren

1. Lade [BSIPA](https://github.com/bsmg/BeatSaber-IPA-Reloaded/releases) herunter.
2. Begib dich zu deinem [Installationsordner.](#installationspfad) und entpacke den Inhalt des Archivs in diesen Ordner. ![Directory Clean](~@images/beginner-guide/directory-clean.png "Directory Clean") ![Directory Ipa](~@images/beginner-guide/directory-ipa.png "Directory Ipa")
3. Doppelklicke auf IPA.exe um das Spiel zu patchen. Alle Mods im Ordner `Plugins` werden ab sofort geladen, wenn das Spiel gestartet wird. Sollte es Fehler geben, hast du etwas in Schritt 2 nicht richtig gemacht. ![Directory Patched](~@images/beginners-guide/directory-patched.png "Directory Patched")

### Mods installieren

4. Lade die Mod(s) herunter die du installieren möchtest. Sei es von GitHub, dem [BSMG Discord](https://discord.com/invite/beatsabermods) `#pc-mods` Kanal, [BeatMods](https://beatmods.com/#/mods) oder anderen Quellen. **Stell sicher, dass du alle Dependncies herunterlädst, die vom Mod benötigt werden.** ![Directory Plugins](~@images/beginner-guide/directory-plugins.png "Directory Plugins")
5. Einige Mods haben Installationsanweisungen, andere nicht. In der Regel kann man einfach die ZIP-Datei im Beat Saber Installationsordner ziehen und entpacken. Die Dateien werden dann in die entsprechenden Ordner entpackt.

## Wie man Mods deinstalliert
Entferne entweder die dll vom `Plugins` Ordner oder klicke auf den `Entfernen` Knopf im Mod Assistant.

## Hilfe von der Community

* [Griffe und Tricks](./grips-and-tricks.md)
* [Erstelle Beatmaps](/de/mapping/)
* [Custom Sabers](/de/models/custom-sabers.md)
* [Custom Avatars](/de/models/custom-avatars.md)
* [Custom Platforms](/de/models/custom-platforms.md)
* [Custom Songs im Multiplayer](https://discord.com/invite/gezGrFG4tz)
* [Mods erstellen](/de/modding/)

## Hast Du Fragen?
Besuche die Support-Kanäle im [BSMG Discord](https://discord.gg/beatsabermods)!
