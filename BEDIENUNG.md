# Purple Alarm: Bedienung

Kurzanleitung für Tester. Was die App sonst noch kann, zeigt *Optionen → Überblick → Hilfe*
(kurze Antworten auf „Wie mache ich …?“, durchsuchbar, mit Knopf, der dich zur Stelle führt).

## Aufbau

Fünf Bereiche unten: **Heute**, **Wecker**, **Kalender**, **Gruppen**, **Optionen**.

- **Heute:** der nächste Wecker mit Countdown, Warnungen (zum Beispiel fehlende Berechtigung), Meldungen, Überspringen.
- **Wecker:** alle Wecker als Karten. Tippen öffnet den Editor, der Schalter schaltet ein oder aus. Oben und am Ende der Liste: Wecker hinzufügen.
- **Kalender:** Monat und Liste. Tippe einen Tag, dann siehst du für jeden Wecker, ob und warum er klingelt oder nicht.
- **Gruppen:** Wecker bündeln (Arbeit, Frühschicht, Sport …) und alle auf einmal ein- oder ausschalten, pausieren oder mit Regeln versehen.
- **Optionen:** Aussehen, Feiertage, Gerät, Hilfe, Feedback.

## Erste Schritte

1. Beim ersten Start führt die Einrichtung durch Sprache, Berechtigungen, Akku und Feiertage.
   Erlaube **Benachrichtigungen** und **Wecker und Erinnerungen**. Stelle die Akku-Nutzung auf **Unbeschränkt**.
2. Optionen → Gerät → Erweitert → Berechtigungen zeigt, ob alles bereit ist. *Heute* warnt, wenn etwas fehlt.
3. Wecker → **+** → Vorlage (zum Beispiel „Werktags 6:30“) oder Uhrzeit und Wochentage wählen → Speichern.
   Ein neuer Wecker ist standardmäßig einmalig und wird beim Speichern eingeschaltet.

## Häufige Aufgaben

| Ich möchte … | So geht es |
|---|---|
| Nur den nächsten Klingelton auslassen | Heute → Karte → *Überspringen*, oder Wecker nach rechts wischen |
| Morgen zu einer anderen Zeit wecken | Heute → *Andere Zeit für diesen Wecker* |
| Alle Arbeitswecker im Urlaub still stellen | Gruppen → Gruppe → *Pausieren …* mit von und bis; oder ein Modus „Urlaub“ |
| Pause rückgängig machen | Gruppenkarte → *Geplante Pause entfernen* oder *Fortsetzen* |
| An Feiertagen nicht klingeln | Optionen → Feiertage → Land und Region hinzufügen; am Wecker oder an der Gruppe *An Feiertagen still* |
| Schichten abbilden | Gruppe → *Regeln und Schichtplan* |
| Einen Wecker kopieren oder löschen | Karte nach links wischen; Löschen fragt noch einmal nach, danach gibt es *Rückgängig* |
| Wissen, warum ein Wecker nicht klingelt | Kalender → Tag; dort steht der Grund |
| Timer oder Stoppuhr | *Timer & Stoppuhr* im Wecker-Bereich |
| Sichern und wiederherstellen | Optionen → Gerät → Import und Export |

Jede Wischgeste hat auch einen Knopf. Fast jede Änderung lässt sich mit *Rückgängig* im Kopf der Seite zurücknehmen.

## Beim Klingeln

- Der Klingel-Bildschirm erscheint auch über der Sperre. **Stoppen** beendet, **Schlummern** wiederholt nach der eingestellten Zeit.
- Wecker lassen sich mit Aufgabe (rechnen, schütteln), Weckton-Anstieg, Aufwachlicht und höchstens so vielen Schlummern einstellen: Editor → *Weitere Optionen beim Klingeln*.
- Eine Benachrichtigung bietet ebenfalls Stoppen und Schlummern an. Die Lautstärke folgt der Alarm-Lautstärke des Telefons; die App ändert sie nie.
- Nach der eingestellten Zeit (Standard 10 Minuten) endet das Klingeln von selbst und gilt als verpasst (*Heute → Meldungen*).
- Zum Testen: Optionen → Gerät → *Alarm-Test*.

## Wenn ein Wecker nicht klingelt

1. *Heute* öffnen und die Warnungen lesen; *Alles bereit?* zeigt den Stand.
2. Alarm-Lautstärke des Telefons prüfen, Nicht stören und Akku-Einstellungen der App (Unbeschränkt).
3. Kalender → Tag: steht dort ein Grund (Pause, Feiertag, Regel)?
4. Optionen → Gerät → Fehlerprotokoll und Ereignisse ansehen, dann melden (siehe [TESTING.md](TESTING.md)).

## Daten und Netz

Alles liegt auf deinem Telefon. Das Netz braucht die App nur, wenn du Feiertage importierst oder
aktualisierst, und für das Feedback-Formular im Browser. Klingeln braucht nie Netz. Details:
Optionen → Gerät → Erweitert → Über (Impressum, Daten, Dienste, Version).
