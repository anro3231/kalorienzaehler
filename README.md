# Kalorien-App V25

Kalorienzähler für iPhone über GitHub Pages.

- Tageskalorien für Frühstück, Mittagessen, Abendessen und Snacks
- 7-, 14- und 30-Tage-Diagramme mit Kalorienziel und Durchschnitt
- Konfigurierbare Tagesziele mit Statistik
- Lokale Sicherung und Wiederherstellung
- Garmin Connect: Tageswerte per Knopfdruck abrufen
- Anzeige von aktiven Kalorien, Ruhekalorien, Gesamtverbrauch und Kalorienbilanz

App: https://anro3231.github.io/kalorienzaehler/

Die persönlichen Essensdaten und abgerufenen Garmin-Tageswerte werden lokal im Browser gespeichert.

## Garmin-Backend einrichten

Die App verwendet eine Supabase Edge Function. Der Garmin-Personal-API-Schlüssel wird ausschließlich serverseitig als Secret gespeichert und ist nicht Teil dieses GitHub-Repositories.

Supabase-Projekt: `qqimqcfqxdmhnvzthhvc`
Edge Function: `garmin-daily-calories`

Im Supabase-Dashboard unter **Edge Functions → Secrets** zwei Secrets anlegen:

- `GARMIN_PERSONAL_API_KEY`: der persönliche API-Schlüssel aus Garmin Connect
- `GARMIN_APP_PASSWORD`: ein eigenes, langes und zufälliges Zugriffspasswort (mindestens 32 Zeichen)

Weder den Garmin-Schlüssel noch das Zugriffspasswort in GitHub, in den Quellcode oder in öffentliche Nachrichten kopieren. Das Zugriffspasswort wird beim Abruf in der App abgefragt und nicht gespeichert.

Die Funktion verwendet Garmins Personal API, holt für das ausgewählte Datum `totalKilocalories`, `activeKilocalories` und `bmrKilocalories` und gibt nur diese Tageswerte an die App zurück.

Garmin-Personal-API-Schlüssel laufen entsprechend der bei Garmin gewählten Laufzeit ab. Bei Ablauf muss ein neuer Schlüssel in den Supabase Secrets hinterlegt werden.
