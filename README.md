# QR-Code Scanner Anwendung

Eine dynamische QR-Code Scanning-Anwendung für Gruppenverfolgung.

## Projektstruktur

- **github-pages/** - Die HTML-Version der Anwendung (eigenständig ohne Server)
  - index.html - Die Hauptdatei, die für GitHub Pages verwendet wird
  - static/ - Enthält CSS, JS und Medien

- **app.py** - Die Python/Flask-Version der Anwendung
- **run.py** - Startet den Flask-Server für die Python-Version

## Bereitstellungsoptionen

Diese Anwendung ist für drei Hauptbereitstellungsplattformen optimiert:

### 1. GitHub Pages
- Die Anwendung wird automatisch über GitHub Actions bereitgestellt
- Verwendet den Inhalt des `github-pages/` Ordners
- Workflow: `.github/workflows/copy-deploy-files.yml`

### 2. Azure Static Web Apps
- Konfiguriert für Azure Static Web Apps Bereitstellung
- Workflow: `.github/workflows/azure-static-web-apps.yml`
- Konfiguration: `staticwebapp.config.json`

### 3. Netlify
- Kann direkt aus dem `github-pages/` Ordner bereitgestellt werden
- Keine spezielle Konfiguration erforderlich

## Funktionalitäten

- QR-Code Scannen mit Kamera
- QR-Code Scannen aus Bildern
- Manuelle Eingabe von QR-Codes
- Gruppierung von Scans (automatisch oder manuell)
- 30-Minuten Countdown-Timer für Gruppen
- Notfall-Funktionalität mit Alarm
- "Trupp fertig" Markierung
- Zeitleiste für alle gescannten Gruppen

## Entwicklung

- HTML-Version: Bearbeite Dateien im `github-pages/` Ordner
- Python-Version: Bearbeite `app.py` 
- React-Version: Dateien im `client/` und `server/` Ordner (in Entwicklung)