# Modding Einführung
_Lerne, wie du deine eigenen Mods für den Pc schreiben kannst._

## Erste Schritte
::: warning Diese Anleitung dient zum Erstellen von Mods für die **PC** Version von Beat Saber!

Stelle sicher, dass dein Spiel modifiziert ist, bevor du versuchst, eine Mod zu erstellen.  
Siehe die Anleitung für [Modde Beat Saber auf PC.](/pc-modding.md)

Dieser Leitfaden setzt ein grundlegendes bis mittleres Verständnis von C# und Unity voraus.  
Wenn Du nicht über diese Grundlagen verfügst, wirst du möglicherweise Schwierigkeiten haben, das hier Behandelte zu verstehen. :::

Beat Saber wurde in Unity 2019.3 mit C# und .NET Framework 4.6 entwickelt  
Du musst die neueste Version von [Visual Studio Community](https://visualstudio.microsoft.com/) herunterladen.

## Modding Tools einrichten
Wir werden in diesem Tutorial die Erweiterung BeatSaberModdingTools verwenden, da sie mit Modding Vorlagen und nützlichen Funktionen ausgestattet ist.   
BeatSaberModdingTools wird von Zingabopp gepflegt. Wenn du die Tools für nützlich hältst, solltest du sie unterstützen.

Du kannst es auf Ihrem [GitHub](https://github.com/Zingabopp/BeatSaberTemplates/releases/latest) herunterladen.  
Du musst `BeatSaberModdingTools.vsix` herunterladen. (Erweitere das Dropdown-Menü Assets, wenn du es nicht finden kannst)

Öffne nach dem Download die `.vsix` und es installiert sich selbst als Visual Studio Plugin.  
Bei Problemen lies dir bitte die [README](https://github.com/Zingabopp/BeatSaberModdingTools#readme) und [WIKI](https://github.com/Zingabopp/BeatSaberModdingTools/wiki) des Projekts durch.

## Template Setup
Erstelle zunächst ein neues Projekt unter Verwendung der Vorlage.  
Wir werden die Vorlage `BSIPA4 Plugin (Core)` verwenden und unsere Mod `BSPlugin1` nennen. Du solltest den Namen so ändern, wie du deine Mod nennen willst.

![Modding-Vorlage auswählen](~@images/modding/modding-template-select.png "Modding-Vorlage auswählen")  
![Name der Modding-Vorlage](~@images/modding/modding-template-name.png "Name der Modding-Vorlage")

Du musst dann dein Beat Saber-Verzeichnis in Visual Studio festlegen. Folge den Anweisungen [in der ReadMe-Datei der Vorlage](https://github.com/Zingabopp/BeatSaberModdingTools#how-to-use), oder sieh dir den Screenshot unten an.

![Einrichtung Beat Saber Verzeichnis](~@images/modding/setup-bs-directory.png "Einrichtung Beat Saber Verzeichnis")

An diesem Punkt **versuche, das Projekt zu bauen.** Es sollte automatisch die Referenzen für dich finden und der Build sollte erfolgreich sein.

Wenn der Build nicht erfolgreich ist, überprüfe, ob du keine fehlenden Referenzen hast.

::: tip BeatSaberModdingTools wird automatisch mit Referenzen umgehen. Wenn deine Referenzen nicht gefunden werden konnten, [prüfe die Anweisungen noch einmal](https://github.com/Zingabopp/BeatSaberModdingTools#how-to-use).

Wenn du Referenzen manuell hinzufügen willst, klicke mit der rechten Maustaste auf `Referenzen` im Projektordner, dann auf `Beat Saber Reference Manager...`. Wähle deine Referenzen aus und klicke dann auf "Übernehmen".

Weitere Informationen über den Referenzmanager findest du [hier](https://github.com/Zingabopp/BeatSaberModdingTools/wiki/Adding-References). :::

## Den Code Untersuchen
Es sollten automatisch 5 Dateien mit der Vorlage geöffnet werden.

| Dateiname                | Über                                                                                                |
| ------------------------ | --------------------------------------------------------------------------------------------------- |
| `manifest.json`          | Informationen über deine Mod für BSIPA.                                                             |
| `Plugin.cs`              | Die Hauptdatei, die für deine Mod geladen wird.                                                     |
| `AssemblyInfo.cs`        | Datei-Informationen über deine Mod. Dies wird größtenteils von Modding Tools verwaltet.             |
| `PluginConfig.cs`        | Eine Vorlage zum Aktivieren der Konfiguration für deine Mod. Dies ist standardmäßig auskommentiert. |
| `BSPlugin1Controller.cs` | Ein allgemeines MonoBehaviour für deine Mod.                                                        |

### Bearbeite das Mod Manifest
Fülle die Datei `manifest.json` mit deinen Informationen aus.  
Der `name` und `id` Schlüssel werden verwendet, um deine Mod zu identifizieren. Die ID sollte mit der ID übereinstimmen, die du beim Hochladen deines Mods auf BeatMods verwendet hast.

::: warning Entferne **nicht** die Abhängigkeit von BSIPA. Ab BSIPA v4.1 ist dies erforderlich, damit deine Mod geladen werden kann. :::

## Kompilieren
Erstelle dein Plugin mit `Build -> Build Solution` oder <kbd>CTRL + SHIFT + B</kbd>  
Deine kompilierte DLL sollte automatisch im `Plugins` Ordner in deinem Beat Saber Verzeichnis kopiert werden! Dies wird für Debug- als auch für Release-Builds durchgeführt.

::: tip HINWEIS Wenn du bereit bist, deinen Mod zu veröffentlichen, wähle die Option `Release`, um einen Release-Build deines Mods zu erstellen.

Das Erstellen im Release Modus erzeugt eine gepackte `.zip`-Datei, die auf BeatMods hochgeladen werden kann. :::

## Testen deiner Mod im Spiel
Um zu testen, ob deine Mod im Spiel geladen ist, musst du Beat Saber mit aktivierter BSIPA Konsole starten. Füge `--verbose` als Startargument hinzu und starte das Spiel.  
Weitere Informationen über Startargumente findest du [hier](./#launch-args).

Wenn du das Spiel startest, solltest du sehen, dass BSIPA deine Mod im Konsolenfenster lädt.

![Screenshot der Konsole](~@images/modding/testing-console.png "Screenshot der Konsole")

## Nächste Schritte
Hier sind einige nützliche Ressourcen für die Fortsetzung deiner Modding Karriere.

* Wenn du Hilfe bei der Entwicklung von Mods brauchst, kannst du im [BSMG Discord](https://discord.gg/beatsabermods) unter `#pc-mod-dev` fragen.
* Wenn du Code dekompilieren möchtest, solltest du dir [dnSpy](https://github.com/dnSpy/dnSpy/releases) ansehen.
* Weitere Informationen über das [Konfigurationssystem](https://bsmg.github.io/BeatSaber-IPA-Reloaded/tags/4.1.3/articles/start-dev.html#configuring-your-plugin) findest du in der BSIPA-Dokumentation.
* Wenn du den Code des Spiels für deine Mod patchen musst, solltest du [Harmony](https://github.com/pardeike/Harmony#readme) verwenden. Die `0Harmony.dll` ist für modifizierte Spiele bereits installiert.
* Für erfahrene Entwickler könnte es interessant sein, mehr über Zenject zu erfahren, das Dependency Injection System von Beat Saber. [SiraUtil](https://github.com/Auros/SiraUtil#readme) ist eine Bibliothek, mit der du dich leicht in dieses System einklinken kannst.
