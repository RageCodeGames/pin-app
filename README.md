# Pin Verbindungs App - PWA

Eine Progressive Web App zum Durchgehen von Pin-Verbindungen aus Excel/CSV-Dateien.

## Features

✅ **Excel & CSV Support**: Lädt .xlsx, .xls und .csv Dateien  
✅ **Touch-Navigation**: Tippen in die Mitte = nächster Schritt  
✅ **Fortschritt speichern**: Automatisches Speichern des Fortschritts  
✅ **Offline-fähig**: Funktioniert ohne Internetverbindung  
✅ **Responsive Design**: Optimiert für Smartphone und Tablet  
✅ **PWA-Installation**: Kann auf dem Homescreen installiert werden  

## Installation

### Methode 1: Lokal verwenden
1. Alle Dateien in einen Ordner kopieren
2. `index.html` in einem Browser öffnen

### Methode 2: Auf einem Webserver
1. Alle Dateien auf einen Webserver hochladen
2. Mit dem Browser auf die URL zugreifen
3. "Zum Homescreen hinzufügen" für App-Installation

### Methode 3: Mit Python (lokaler Server)
```bash
python -m http.server 8000
```
Dann im Browser: `http://localhost:8000`

## Verwendung

### 1. Datei einlesen
- Auf "📁 Datei auswählen" klicken
- Excel (.xlsx, .xls) oder CSV-Datei auswählen
- Die Datei muss folgendes Format haben:
  - Zeile 1: Header (wird ignoriert)
  - Spalte A: Schritt
  - Spalte B: Von Pin
  - Spalte C: Zu Pin

### 2. Navigation
- **Vorwärts**: Tippen/Klicken in die Mitte des Bildschirms
- **Zurück**: Button "⬅ Schritt zurück"

### 3. Buttons
- **🔄 Zurücksetzen**: 10 Sekunden gedrückt halten um zu Schritt 1 zurückzuspringen
- **🏠 Home**: Datei entfernen (mit doppelter Bestätigung)

### 4. Fortschritt
- Der aktuelle Schritt wird automatisch gespeichert
- Beim erneuten Öffnen der App wird an der gleichen Stelle weitergemacht
- Der Fortschritt bleibt auch nach dem Schließen des Browsers erhalten

## Dateiformat Beispiel

```csv
Schritt,Von Pin,Zu Pin
1,A1,B2
2,B2,C3
3,C3,D4
...
```

## Browser-Kompatibilität

- ✅ Chrome/Edge (empfohlen)
- ✅ Safari (iOS/macOS)
- ✅ Firefox
- ✅ Opera

## Als App installieren

### Auf Android (Chrome):
1. Öffne die Webseite
2. Tippe auf das Menü (⋮)
3. Wähle "Zum Startbildschirm hinzufügen"

### Auf iOS (Safari):
1. Öffne die Webseite
2. Tippe auf das Teilen-Symbol
3. Wähle "Zum Home-Bildschirm"

### Auf Desktop (Chrome/Edge):
1. Öffne die Webseite
2. Klicke auf das ⊕-Symbol in der Adressleiste
3. Wähle "Installieren"

## Technische Details

- **Framework**: Vanilla JavaScript (kein Framework nötig)
- **Excel-Bibliothek**: SheetJS (xlsx.js)
- **Speicher**: localStorage (Browser)
- **Offline**: Service Worker für PWA-Funktionalität

## Dateien

- `index.html` - Hauptanwendung
- `manifest.json` - PWA-Manifest
- `sw.js` - Service Worker
- `README.md` - Diese Datei

## Troubleshooting

**Problem**: Datei wird nicht geladen  
**Lösung**: Überprüfen Sie, dass die Datei das richtige Format hat (Spalten A, B, C)

**Problem**: Fortschritt wird nicht gespeichert  
**Lösung**: Stellen Sie sicher, dass localStorage im Browser aktiviert ist

**Problem**: App funktioniert nicht offline  
**Lösung**: Öffnen Sie die App mindestens einmal online, damit sie gecacht wird

## Support

Bei Fragen oder Problemen:
- Überprüfen Sie das Dateiformat
- Testen Sie mit einer kleineren Beispieldatei
- Verwenden Sie die Browser-Konsole (F12) für Fehlermeldungen
