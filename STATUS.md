# Projektstatus – Videos für Facebook und Instagram

**Stand:** 12. Oktober 2026

## Ziel
Die 31 bereits fertig produzierten Videos auf dem Rechner des Projektinhabers vollautomatisch nach festem Zeitplan auf Facebook und Instagram veröffentlichen. Eine manuelle Freigabe vor jedem Beitrag ist nicht vorgesehen.

## Bisher erledigt
- GitHub-Repository vorhanden: https://github.com/Fex66/Videos-f-r-Facebook-und-Insta
- Arbeitsbranch angelegt: `setup/31-video-publishing-plan`
- Veröffentlichungsplan `veroeffentlichungsplan.csv` mit 31 vorbereiteten Zeilen erstellt
- `README.md` um Projektziel, Voraussetzungen und Ablauf ergänzt
- `.gitignore` ergänzt, um lokale Videodateien und Geheimnisse nicht versehentlich einzuchecken
- `.env.example` als Platzhalter-Konfiguration angelegt; sie enthält keine echten Zugangsdaten
- `META-EINRICHTUNG.md` mit einer Checkliste für Meta-Entwicklerzugang, Berechtigungen, IDs, Token und Videospeicher erstellt
- Pull Request Nr. 1 eröffnet: https://github.com/Fex66/Videos-f-r-Facebook-und-Insta/pull/1

## Bekannte Voraussetzungen / Entscheidungen
- Facebook-Seite und Instagram-Konto sind laut Projektinhaber bereits miteinander verbunden.
- Veröffentlichung soll vollautomatisch nach Zeitplan erfolgen, auf beiden Plattformen.
- Die 31 Videodateien befinden sich derzeit auf dem lokalen Rechner und wurden nicht ins Repository hochgeladen.

## Noch offen
1. Pull Request Nr. 1 prüfen und in `main` übernehmen.
2. Meta-Entwickler-App und den passenden Veröffentlichungsweg einrichten.
3. Prüfen, dass das Instagram-Konto professionell (Business oder Creator) ist.
4. Facebook-Seiten-ID und Instagram-Professional-Account-ID ermitteln.
5. Benötigte Berechtigungen und Token sicher konfigurieren. Keine Tokens, App-Geheimnisse oder Passwörter in Quellcode, CSV oder README speichern; später GitHub Actions Secrets verwenden.
6. Geeigneten Videospeicher/Upload-Weg auswählen, damit die Automatisierung auf die Videodateien zugreifen kann. Ein lokaler Dateipfad funktioniert nicht für einen Cloud-Job, wenn der Rechner nicht erreichbar ist.
7. Dateinamen, Veröffentlichungstermine, Uhrzeiten, Begleittexte und Hashtags in der CSV eintragen.
8. Veröffentlichungsworkflow entwickeln und mit einem Testbeitrag prüfen.
9. Erst nach erfolgreichem Test die automatische Veröffentlichung aktivieren.

## Sicherheits- und Betriebsstatus
**Automatische Veröffentlichung ist noch nicht eingerichtet und derzeit nicht aktiv.** Es wurden keine Beiträge veröffentlicht. Zugangsdaten wurden noch nicht eingetragen.

## Nächster Schritt
Im Meta-Entwicklerportal anmelden und prüfen, ob bereits eine App vorhanden ist oder eine neue App erstellt werden muss. Danach die offizielle Meta-Konfiguration anhand von `META-EINRICHTUNG.md` fortsetzen.
