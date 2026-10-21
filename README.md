# Satzbuch (Android)

Persönliches Trainings-Logbuch. Alle Daten bleiben auf dem Handy.

## APK bekommen
Jeder Push auf `main` baut die App über GitHub Actions. Die fertige `Satzbuch.apk`
liegt danach unter **Releases** (neueste Version oben).

## Installieren
1. Release-Seite auf dem Handy öffnen, `Satzbuch.apk` herunterladen.
2. Datei öffnen. Android fragt einmalig, ob der Browser/Dateimanager Apps installieren darf → erlauben.
3. Updates genauso installieren – sie ersetzen die alte Version, die Daten bleiben erhalten.

## Wichtig
- Der Signaturschlüssel liegt NICHT im Repo, sondern als GitHub-Secrets (`KEYSTORE_BASE64`, `KEYSTORE_PASSWORD`).
  Den Schlüssel sicher aufbewahren: Mit einem anderen Schlüssel lässt sich ein Update nicht über die alte
  Version installieren.
- Wer das Repo forkt, muss eigene Secrets mit eigenem Schlüssel anlegen.
- Backups: in der App unter „Plan“ → „Backup exportieren“ (landet im Download-Ordner).

## Inhalt ändern
Die App selbst ist `app/src/main/assets/index.html`.
