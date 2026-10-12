# Videos für Facebook und Instagram

Ziel: Die 31 bereits fertig produzierten Videos nach einem festgelegten Zeitplan auf Facebook und Instagram veröffentlichen.

## Aktueller Stand

- [x] Projekt angelegt
- [x] Vorlage für 31 Videos und Veröffentlichungsdaten vorbereitet
- [ ] Tatsächliche Videodateinamen und Termine eintragen
- [ ] Veröffentlichungsweg festlegen und Meta-Zugriff einrichten
- [ ] Zugangsdaten sicher als GitHub Actions Secrets hinterlegen
- [ ] Testveröffentlichung durchführen
- [ ] Automatische Veröffentlichung aktivieren

## Wichtig: Videos nicht in GitHub hochladen

Die Videodateien bleiben zunächst auf deinem Rechner. GitHub speichert hier den Plan und den Programmcode, nicht die großen Videodateien. Für automatisches Posten muss später ein geeigneter Speicherort mit abrufbaren Video-URLs eingerichtet werden. Ein lokaler Dateipfad auf deinem Rechner reicht für einen Cloud-Workflow nicht aus.

## Erste Schritte

1. Öffne `veroeffentlichungsplan.csv`.
2. Ersetze `video01.mp4` bis `video31.mp4` durch die tatsächlichen Dateinamen deiner Videos.
3. Trage gewünschte Veröffentlichungsdaten und Uhrzeiten ein. Zeitzone: `Europe/Berlin`.
4. Ergänze pro Video den Begleittext und Hashtags.

Die CSV ist zunächst nur eine Planungsvorlage. Sie veröffentlicht noch nichts.

## Voraussetzungen für die spätere Automatisierung

- Eine Facebook-Seite, auf der du veröffentlichen darfst.
- Ein Instagram-Konto, das für die Veröffentlichung über die Meta-Schnittstelle geeignet und mit der Facebook-Seite verbunden ist.
- Meta-Zugriff und Berechtigungen für beide Konten.
- Ein Speicherort, von dem Meta die Videodateien abrufen kann.
- Sicher gespeicherte Zugangsdaten. Tokens und Passwörter dürfen niemals in Dateien oder Commits stehen.

Die Automatisierung wird erst aktiviert, wenn die Konten, der Speicherort und die Berechtigungen geprüft wurden. Bis dahin wird nichts veröffentlicht.
