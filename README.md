# Purple Alarm: Beta-Versionen / beta releases

**Purple Alarm** ist ein Wecker-Manager für Android: viele Wecker, geordnet in Gruppen, still gestellt
durch Pausen (Urlaub, Schichtarbeit) und Feiertage. Die App klingelt zuverlässig auch bei geschlossener App,
nach einem Neustart und im Ruhemodus. Deutsch zuerst, Englisch verfügbar. Kein Konto, keine Werbung,
keine Analyse, keine Cloud. Zum Klingeln braucht die App nie Internet.

*English: Purple Alarm is an Android alarm manager (many alarms, groups, pause windows, public holidays,
native alarm engine that rings with the app closed). This repository carries the beta APKs, their
checksums and guides; the source code is private. A short English install note is at the end.*

> **Beta.** Es gibt noch Ecken und Kanten. Das zuverlässige Klingeln ist bisher auf einem Telefon geprüft;
> genau dafür ist die Beta da. Verlass dich noch nicht als einziger Wecker darauf.

## Installation (Schritt für Schritt)

Du brauchst ein Android-Telefon (Android 8 oder neuer). Die App kommt nicht aus dem Play Store, sondern
als Datei von hier. Das ist normal und dauert fünf Minuten. Die Namen der Menüs unterscheiden sich je nach
Hersteller ein wenig; das Vorgehen ist überall gleich.

### 1. Datei herunterladen

1. Öffne auf dem **Telefon** diese Seite und tippe auf **Releases** (rechts oder unter dem Dateilisting).
   Oder öffne direkt: <https://github.com/forky-fish/purple-alarm-releases/releases/latest>
2. Suche die neueste Version ganz oben und scrolle zu **Assets**.
3. Tippe auf die Datei **`purple-alarm-….apk`**. Der Download startet. Bei der Frage
   „Diese Art von Datei kann Ihr Gerät beschädigen“ tippe auf **Trotzdem herunterladen** oder **OK**.
   Das ist die übliche Warnung für jede Datei dieser Art.

### 2. Installieren

1. Wenn der Download fertig ist, tippe unten auf **Öffnen**. Oder öffne die App **Dateien** (oder
   „Downloads“) und tippe dort auf die Datei.
2. Beim ersten Mal sagt Android, dass diese Quelle nicht erlaubt ist („Aus Sicherheitsgründen darf …“).
   Tippe auf **Einstellungen**, schalte **Aus dieser Quelle zulassen** ein und gehe mit der Zurück-Taste zurück.
   Die Quelle ist der Browser oder die Dateien-App, mit der du die Datei geöffnet hast. Du kannst die Erlaubnis später wieder ausschalten.
3. Tippe auf **Installieren**.
4. Zeigt Google Play Protect „App wird nicht oft heruntergeladen“ oder „Unbekannte App“, tippe auf
   **Weitere Details** und dann auf **Trotzdem installieren**. Das erscheint bei jeder App, die nicht aus dem Play Store kommt.
5. Tippe auf **Öffnen**.

### 3. Erster Start: damit der Wecker zuverlässig klingelt

Die Einrichtung in der App führt dich durch diese Schritte. Sie sind wichtig, sonst kann Android den Wecker verschlafen.

1. **Benachrichtigungen:** Tippe auf **Zulassen**.
2. **Wecker und Erinnerungen:** Android öffnet eine Einstellungsseite. Schalte **Zulassen** (Wecker und Erinnerungen) für Purple Alarm ein.
3. **Akku:** Öffne **Einstellungen → Apps → Purple Alarm → Akku** und wähle **Uneingeschränkt** (bei manchen Herstellern „Nicht optimieren“ oder „Keine Einschränkungen“).
   Die App zeigt dir unter *Optionen → Gerät → Erweitert → Berechtigungen* mit grünem Haken, ob alles bereit ist.
4. **Alarm-Lautstärke:** Stelle die Lautstärke für **Wecker** am Telefon (Einstellungen → Töne) nicht auf null. Die App ändert die Lautstärke nie von selbst.

Danach: **Wecker → +**, Uhrzeit wählen, **Speichern**. Mach zum Test einen Wecker für in zwei Minuten und sperre das Telefon.
Mehr zur Bedienung: [BEDIENUNG.md](BEDIENUNG.md).

### 4. Echt sein? Die Datei prüfen (optional)

Jede Version nennt auf ihrer Release-Seite zwei Prüfwerte. In der installierten App findest du dieselben unter
*Optionen → Gerät → Erweitert → Über → Version*: den Wert der **APK** und den des **Signaturzertifikats**.
Stimmen beide mit der Release-Seite überein, ist es die Original-Datei. Ein anderer Zertifikatswert heißt:
Das ist nicht unsere Datei, bitte deinstallieren. Auf einem Computer prüfst du die Datei mit
`sha256sum -c SHA256SUMS` (Windows: `certutil -hashfile purple-alarm-….apk SHA256`).

### Aktualisieren

Lade die neuere Datei wie oben herunter und installiere sie **über** die alte (Schritt 2). Deine Wecker und Einstellungen bleiben.
Die App aktualisiert sich nicht selbst; schau ab und zu auf der Releases-Seite nach.

### Wenn etwas nicht klappt

| Problem | Lösung |
|---|---|
| „App nicht installiert“ beim Aktualisieren | Eine frühere Test-Version mit anderer Signatur ist installiert. Sichere deine Wecker (*Optionen → Gerät → Import und Export*), deinstalliere die App, installiere die neue und stelle die Sicherung wieder her. |
| „Installation blockiert“ | Schritt 2.2: Erlaubnis für die Quelle (Browser oder Dateien-App) einschalten. |
| Die Datei lässt sich nicht öffnen | Download noch nicht fertig, oder die Datei ist beschädigt: erneut herunterladen. |
| Ein Wecker hat nicht geklingelt | In der App *Heute* öffnen und die Warnungen lesen; Akku auf *Uneingeschränkt* prüfen; dann bitte melden (siehe unten). Mehr auf [dontkillmyapp.com](https://dontkillmyapp.com). |
| Ich will die App wieder loswerden | Einstellungen → Apps → Purple Alarm → Deinstallieren. Alle Daten der App werden gelöscht. |

## Anleitungen

- [Bedienung](BEDIENUNG.md): was die App kann und wie es geht.
- [Beta testen](TESTING.md): was du ausprobieren kannst und wie du Probleme meldest.

## Feedback

Eröffne ein [Issue](../../issues) hier, oder nutze in der App *Optionen → Gerät → Feedback*. Bitte nenne Telefonmodell,
Android-Version und App-Version (*Über → Version*).

## Lizenz

Die App ist © ihr Autor, alle Rechte vorbehalten. Diese Beta wird ohne Gewähr zum Testen bereitgestellt.
Der Quellcode liegt in einem privaten Repository.

## English install note

Android 8 or newer. Download `purple-alarm-<version>.apk` from the newest
[release](../../releases) on your phone, open it, allow installs from that source when Android asks,
tap *Install* (on Play Protect's warning choose *More details → Install anyway*). On first start allow
notifications and *Alarms & reminders*, and set the app's battery use to *Unrestricted*. Update by installing
a newer APK over the old one. Verify with `sha256sum -c SHA256SUMS`; the app shows the APK and certificate
hashes under *Optionen → Gerät → Erweitert → Über → Version*. Report problems as an [issue](../../issues).
