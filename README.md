# Kalorientagebuch für iPhone (GitHub Pages)

## Veröffentlichen
1. Auf GitHub ein neues **öffentliches** Repository erstellen, z. B. `kalorien-app`.
2. Die Dateien `index.html`, `manifest.webmanifest`, `sw.js` und `icon.svg` in das Hauptverzeichnis hochladen.
3. Unter **Settings → Pages → Build and deployment** bei **Source** „Deploy from a branch“ wählen, Branch `main` und Ordner `/ (root)` auswählen und speichern.
4. Nach der Veröffentlichung die angezeigte GitHub-Pages-Adresse im iPhone-Safari öffnen (normalerweise `https://BENUTZERNAME.github.io/kalorien-app/`).
5. In Safari **Teilen → Zum Home-Bildschirm** auswählen.

## Hinweise
- Keine Anmeldung und kein Server erforderlich.
- Die Eingaben werden im lokalen Browser-Speicher gespeichert, nicht in GitHub. Sie synchronisieren sich **nicht** zwischen Geräten.
- Im Statistik-Tab können Daten als JSON exportiert und wieder importiert werden.
- Leere Tage werden als „kein Eintrag“ markiert und nicht als erfolgreiche Zieltage gezählt.
- Die Statistik bezieht sich auf das im Tages-Tab ausgewählte Datum und die vorherigen 6 bzw. 29 Tage.

## Version 2
- Helles Design und horizontale Ziel-Linie in der Statistik.
- Kalorienzahlen direkt über den Balken.
- Die 30-Tage-Ansicht ist horizontal scrollbar (auf dem iPhone wischen).
- Beim Ersetzen der Dateien bleiben bestehende Einträge im selben Browser erhalten.
