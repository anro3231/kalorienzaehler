# Version 16

Kalorien-Eingabefeld schmaler (82 px, auf schmalen Displays 76 px) und Schrift kleiner (16 px). Restliches Layout unverändert.

Version 14: Mahlzeitenname und Kalorieneingabe beginnen auf derselben Höhe; Plus/Minus links unter dem Namen, direkt neben dem Eingabefeld.

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
- Die Statistik zeigt immer die letzten 7 bzw. 30 Kalendertage einschließlich heute – unabhängig vom ausgewählten Bearbeitungsdatum.

## Version 2
- Helles Design und horizontale Ziel-Linie in der Statistik.
- Kalorienzahlen direkt über den Balken.
- Die 30-Tage-Ansicht ist horizontal scrollbar (auf dem iPhone wischen).
- Beim Ersetzen der Dateien bleiben bestehende Einträge im selben Browser erhalten.

## Version 3
- Der heutige Tag ist immer der letzte Balken in beiden Statistiken.
- Jeder Balken zeigt den Wochentag und das Datum; heute ist zusätzlich hervorgehoben.

## Version 4
- Unter jeder Mahlzeit stehen Schnellwahlknöpfe +50, +100 und +200 kcal.
- Ein Tipp addiert den Wert zur bestehenden Mahlzeit und speichert automatisch.

## Version 5
- Kleine, dezente Schnellwahlknöpfe −200, −100, −50, +50, +100 und +200 kcal.
- Kalorien-Eingabefeld ist größer und deutlicher hervorgehoben.
- Minusknöpfe reduzieren einen Wert nie unter 0 kcal.


## Version 6
Beide Diagramme zeigen alle 7 bzw. 30 Tage ohne horizontales Scrollen. Der Durchschnitt wird über alle Kalendertage des Zeitraums berechnet (Tage ohne Eintrag zählen als 0 kcal).

## Version 7
Lokale Sicherung und Wiederherstellung direkt auf der Startseite sowie in der Statistik. Die Sicherungsdatei enthält das Kalorienziel und alle gespeicherten Tage. Beim Import wird die Datei geprüft und vor dem Überschreiben um Bestätigung gebeten.


## Version 8
- Die untere Navigation liegt nun außerhalb des scrollbaren Inhalts und bleibt stabil sichtbar, auch beim Scrollen auf iPhones.
- Neues helles Farbschema in Salbei/Mint mit Lavendel als Akzent für die Ziellinie.
- In der 30-Tage-Ansicht nur Tageszahlen (keine Wochentage); in der 7-Tage-Ansicht weiterhin Wochentage und Datum.

## Version 9
Kalorien-Eingabefeld kompakt direkt unter der Mahlzeitenbezeichnung. Plus- und Minus-Knöpfe darunter rechtsbündig. Alle bisherigen Funktionen und gespeicherten Daten bleiben erhalten.


Version 10: Schnellwahlknöpfe rechts in derselben Zeile wie die Mahlzeitenbezeichnung; Kalorienfeld darunter.

## Version 11
Die Schnellbuttons stehen in zwei Zeilen rechts neben dem Mahlzeitennamen: oben +50, +100, +200 und direkt darunter −50, −100, −200.

## Version 12
Schnellbuttons direkt unter der Mahlzeitenbezeichnung links; Kalorien-Eingabefeld rechts in derselben Zeile.


## Version 13
Die Plus- und Minus-Schnellwahltasten stehen unmittelbar links neben dem Kalorienfeld. Beide Tastenreihen zusammen sind exakt so hoch wie das Eingabefeld (66 px).


Version 15: Schnellwahl-Tasten und Kalorienfeld beginnen auf derselben Höhe wie die Mahlzeitenbezeichnung; Buttons links direkt neben dem Eingabefeld.


## Version 17
Der Durchschnitt der letzten 7 oder 30 Tage erscheint in einer großen farbigen Karte: grün bei Durchschnitt ≤ Tagesziel, rot bei Überschreitung. Nicht erfasste Tage zählen weiterhin mit 0 kcal.
