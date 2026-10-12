# Meta-Zugriff einrichten

Diese Checkliste ist der nächste Schritt vor dem Programmieren der automatischen Veröffentlichung. Die Facebook-Seite und das Instagram-Konto sind bereits miteinander verbunden.

## 1. Instagram-Kontotyp prüfen

Die Instagram-Veröffentlichungs-API setzt ein professionelles Instagram-Konto voraus (Business oder Creator). Ein privates persönliches Konto reicht nicht aus.

Prüfung in Instagram:
1. Profil öffnen.
2. Menü öffnen.
3. Nach „Kontotyp und Tools“ bzw. „Für Profis“ suchen.
4. Prüfen, ob das Konto als Business oder Creator geführt wird.

Wenn das Konto bereits professionell ist, nichts ändern.

## 2. Meta-Entwicklerkonto und App

1. Öffne https://developers.facebook.com/
2. Melde dich mit dem Facebook-Konto an, das die Seite verwaltet.
3. Öffne „Meine Apps“ und erstelle eine Meta-App für die Verwaltung deiner eigenen Inhalte. Die Bezeichnungen können sich je nach Meta-Oberfläche ändern.
4. Füge die passenden Facebook-/Instagram-Produkte bzw. Anwendungsfälle zum Veröffentlichen von Inhalten hinzu.
5. Verwende die offizielle Meta-Dokumentation für die aktuelle Anmeldung und Berechtigungen.

Für den üblichen Veröffentlichungsweg mit Facebook-Login sind unter anderem Berechtigungen wie `pages_show_list`, `pages_read_engagement`, `pages_manage_posts` und `instagram_content_publish` relevant. Welche Berechtigungen konkret benötigt werden, hängt vom verwendeten API-Weg und den aktuellen Meta-Anforderungen ab.

Offizielle Meta-Sammlung mit aktuellen Beispielaufrufen:
- Instagram API: https://www.postman.com/meta/instagram/documentation/6yqw8pt/instagram-api
- Facebook API: https://www.postman.com/meta/facebook/documentation/r56bjfd/facebook-api

## 3. IDs und Zugriff sicher ermitteln

Für die spätere Einrichtung benötigen wir:
- Facebook-Seiten-ID
- Instagram Professional Account ID
- einen geeigneten Seiten-Zugriffstoken mit den nötigen Berechtigungen

Bitte poste niemals Tokens, App-Geheimnisse oder Passwörter hier im Chat und speichere sie nicht in CSV-, README- oder Python-Dateien. Sie gehören später in die GitHub-Repository-Einstellungen unter **Settings → Secrets and variables → Actions**. Der Token wird erst eingetragen, wenn wir den Ablauf sicher eingerichtet haben.

## 4. Speicherort für die Videos auswählen

Die 31 Videos liegen momentan auf deinem Rechner. Ein GitHub-Automatisierungsjob kann nicht dauerhaft auf die Dateien deines Rechners zugreifen, wenn der Rechner aus ist.

Für Instagram-Reels muss Meta die Videodatei über einen unterstützten Upload-Weg abrufen können. Beim URL-basierten Veröffentlichungsweg muss die Video-URL zum Veröffentlichungszeitpunkt öffentlich abrufbar sein. Für Facebook gibt es Upload-Wege für lokale Dateien oder gehostete Videos.

Wir wählen den Speicherort, bevor wir den Veröffentlichungsjob aktivieren. Die Videodateien sollten nicht ins GitHub-Repository hochgeladen werden.

## 5. Noch nicht aktivieren

Bis IDs, Berechtigungen, Token, Videospeicher und Test erfolgreich geprüft wurden, veröffentlicht das Projekt nichts automatisch.
