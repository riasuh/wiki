---
sidebar: auto
---

# Quest Modding mit Android

:::warning Wenn du BMBF installierst und dein Spiel modifizierst, wird der offizielle Mehrspielermodus sowie die Anzeige und das Hochladen von Spielständen in den Bestenlisten des Basisspiels deaktiviert. Wenn du einen modifizierten Mehrspielermodus spielen möchtest, benötigst du die Mod `Beat Together`, die Cross-Play zwischen PC und Quest ermöglicht und die Verwendung von Custom Songs erlaubt. Die Mod kann im [Beat Saber Modding Group](discord.gg/beatsabermods) Discord unter `#quest-mods` oder auf der [Questboard](https://questmodding.com) Seite gefunden werden.

Um Ranglisten für Custom Songs zu erhalten und um Performance-Punkte (PP) für Ranked Songs zu bekommen, benötigst du die [ScoreSaber](https://new.scoresaber.com/quest) Mod. [Dieser Link](https://new.scoresaber.com/quest) führt dich zur ScoreSaber-Seite, um das Programm einzurichten. ScoreSaber ersetzt nicht die Bestenlisten des Basisspiels, sondern fügt nur Bestenlisten für Custom Songs hinzu.

**Hinweis:** Überprüfe den Update-Kanal im [ScoreSaber Discord](https://discord.gg/WpuDMwU), um zu sehen, ob die Mod für die aktuelle Spielversion verfügbar ist. :::

::: tip HINWEIS Die empfohlene Art, BMBF zu installieren, ist mit [SideQuest auf einem PC](/quest-modding.md#installing-bmbf-with-sidequest). Diese Methode sollte nur verwendet werden, wenn du keinen Zugriff auf einen PC hast. :::

* [Voraussetzungen](#requirements)
* [Entwicklermodus auf deiner Quest aktivieren](#how-to-enable-developer-mode-on-the-oculus-quest)
* [Telefon einrichten](#setup-your-phone)
* [BMBF auf deinem Telefon installieren](#installing-bmbf-with-your-phone)
* [Beat Saber einrichten](#setup-beat-saber)

## Voraussetzungen

* Ein Android Phone oder Android Tablet
  * iPhones oder iPads werden **NICHT** unterstützt
* Eine **bezahlte** Version von Beat Saber im Oculus Quest Store
* Ein Kabel um deine Quest mit deinem Telefon zu verbinden (wenn dein Telefon über USB C geladen wird, sollte das Ladegerät, das mit deiner Quest mitgeliefert wurde, funktionieren)

## Wie man den Entwicklermodus auf der Oculus Quest aktiviert
Es gibt zwei Methoden, die erste erfordert eine Kreditkarte. Wenn du keine hast, kannst du [Ich habe keine Kreditkarten](#i-have-no-credit-card) Schritte folgen.

### Mit Kreditkarte verifizieren
Gehe zum [Oculus Dashboard](https://dashboard.oculus.com/) und melde dich mit deinem Facebook-Konto an.

Nachdem du dich erfolgreich angemeldet und verifiziert hast, kannst du eine neue Organisation erstellen.

![DevModeDashboard](~@images/beginners-guide/DevModeDashboard.png)

![DevModeCreateOrg](~@images/beginners-guide/DevModeCreateOrg.png)

Nachdem du diese erstellt hast, kannst du den Entwicklermodus in der Oculus-App auf deinem Smartphone aktivieren.

#### Aktivieren des Entwicklermodus in der Oculus App

![EnableDevMode](~@images/beginners-guide/EnableDevMode.png)

Du kannst nun zu [Telefon einrichten](#setup-your-phone) wechseln

### Ich habe keine Kreditkarte
[Originalquelle](https://www.reddit.com/r/sidequest/comments/jaxy4u/cant_verify_oculus_developer_account/?utm_source=amp&utm_medium=&utm_content=post_body).

Bitte beachte, dass du ein zweites Konto (Oculus-Entwicklerkonto) erstellst und dann dein Facebook-Profil zu der erstellten Organisation hinzufügen musst. Das ist etwas schwieriger.

:::tip Wenn du einen Freund hast, der eine Organisation hat, kannst du ihn bitten dichhinzuzufügen, damit du kein neues Konto erstellen musst. Wenn ja, sag deinem Freund, dass er stattdessen die Schritte unter [Sich selbst zur Organisation hinzufügen](#add-yourself-to-the-organization) mit deinem Facebook Konto ausführen soll. :::

#### Erstelle ein neues Developer Konto

1. Rufe die [Anmeldeseite für Oculus-Entwickler](https://developer.oculus.com/sign-up/) auf und klicke auf `Erstelle ein unverbundenes Oculus Entwicklerkonto`.
2. Fülle die erforderlichen Informationen aus.
3. Überprüfe die E-Mail, die du erhalten hast, und melde dich erneut mit dem erstellten Konto an.
4. Rufe die [Überprüfungsseite](https://developer.oculus.com/manage/verify/) auf und richte die Zwei-Faktor Authentifizierung ein.

![2fa](~@images/beginners-guide/2fa.png)

#### Neue Organisation erstellen
Gehe danach zum [Oculus Dashboard](https://dashboard.oculus.com/) und erstelle eine Organisation mit *fast* jedem beliebigen Namen, den du möchtest.

![DevModeDashboard](~@images/beginners-guide/DevModeDashboard.png)

![DevModeCreateOrg](~@images/beginners-guide/DevModeCreateOrg.png)

#### Füge dich zur Organisation hinzu
After you created your Organization you have to add your Facebook profile to your Organization by Selecting your Organization in the drop down and then clicking on Members. There you add a new Member with the Role Admin and put in the Username of your Facebook profile. After that, click add and the user should be added.

![DevModeCreateOrg](~@images/beginners-guide/addmember.png)

#### Enable Developer Mode in the Oculus App
You should now be able to enable the developer mode in the Oculus app on your smartphone.

![EnableDevMode](~@images/beginners-guide/EnableDevMode.png)

You can now continue to [Setup your Phone](#setup-your-phone)

## Setup your Phone

1. Download the [SideQuest app from the Google Play store](https://play.google.com/store/apps/details?id=side.quest.mobile)
2. Enable Developer mode on your Phone
    1. Go into your Android settings
    2. Scroll to "About phone" and open it
    3. Tap "Software information"
    4. Tap the "Build number" field until it says Developer mode enabled. This should take about 7 taps.
3. Enable USB debugging on your Phone
    1. Go back to settings
    2. Tap "Developer options"
    3. Activate USB debugging

### Installing BMBF with your Phone
:::warning Before modding, run Beat Saber once, play a level and immediately fail! :::

Open Sidequest on your Phone connect and your Quest with your phone via the USB Cord. You should get a USB debugging pop-up in your Quest and on your phone. Select allow on both devices and if you prefer, select always allow.

Now if SideQuest picked your Quest up you should see the SideQuest logo with a green dot next to it at the bottom of your Screen.

Then install BMBF by clicking the search icon at the top of SideQuest and search for `BMBF`. You should see an app with an unicorn as symbol. Tap on that and click `INSTALL TO HEADSET`.

Afterwards you should have BMBF installed on your Quest and are ready to mod Beat Saber.

## Setup Beat Saber
After successfully installing BMBF onto your Quest you should be able to find it in your Quests library under unknown sources.

![UnknownMenu](~@images/beginners-guide/quest_home-menu.jpg)

Open it and allow file access after starting it if prompted. Now follow the on-screen instructions carefully. After you finished you should see [BeastSaber](https://bsaber.com).

If at any point during the install process, you get the Restore App popup just click Close. This warning is directed to pirated versions of the game so there will likely be no consequences for ignoring it if you have a legitimate copy.

Now you can continue with the [Core Mods](/quest-modding.md#core-mods) step of the installation process as if you were modding with your PC.
