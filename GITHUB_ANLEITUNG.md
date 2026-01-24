# 🚀 GitHub Pages Deployment - Anleitung

## Schnellstart (5 Minuten)

### Schritt 1: GitHub Account erstellen
1. Gehe zu [github.com](https://github.com)
2. Klicke auf "Sign up" (falls du noch keinen Account hast)
3. Erstelle einen kostenlosen Account

### Schritt 2: Neues Repository erstellen
1. Klicke auf das **+** Symbol oben rechts
2. Wähle **"New repository"**
3. Fülle aus:
   - **Repository name**: `pin-app` (oder ein anderer Name)
   - **Public** auswählen (muss öffentlich sein für GitHub Pages)
   - ✅ **"Add a README file"** NICHT aktivieren
4. Klicke auf **"Create repository"**

### Schritt 3: Dateien hochladen
1. Auf der Repository-Seite, klicke auf **"uploading an existing file"**
2. Ziehe alle 5 Dateien in das Upload-Feld:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `README.md`
   - `beispiel.csv`
3. Scrolle runter und klicke **"Commit changes"**

### Schritt 4: GitHub Pages aktivieren
1. Gehe zu **Settings** (oben in deinem Repository)
2. Klicke links auf **"Pages"**
3. Unter **"Source"**:
   - Branch: **main** (oder **master**)
   - Folder: **/ (root)**
4. Klicke **"Save"**
5. Warte 1-2 Minuten ⏳

### Schritt 5: Deine App öffnen! 🎉
Deine App ist jetzt verfügbar unter:
```
https://DEIN-USERNAME.github.io/pin-app/
```

Ersetze `DEIN-USERNAME` mit deinem GitHub Benutzernamen.

---

## Alternative: GitHub Desktop (wenn du lieber eine App benutzt)

### Methode A: GitHub Desktop
1. Lade [GitHub Desktop](https://desktop.github.com/) herunter
2. Melde dich mit deinem GitHub Account an
3. Klicke auf **"Create a New Repository"**
   - Name: `pin-app`
   - Local Path: Wähle einen Ordner
4. Klicke **"Create Repository"**
5. Kopiere alle 5 Dateien in den Ordner
6. In GitHub Desktop:
   - Schreibe eine Commit Message: "Initial commit"
   - Klicke **"Commit to main"**
   - Klicke **"Publish repository"**
   - ✅ Entferne das Häkchen bei "Keep this code private"
   - Klicke **"Publish Repository"**
7. Aktiviere GitHub Pages (siehe Schritt 4 oben)

---

## 📱 Als App auf dem Handy installieren

### Android (Chrome):
1. Öffne den Link in Chrome
2. Tippe auf **⋮** (Menü)
3. Wähle **"Zum Startbildschirm hinzufügen"**
4. Tippe **"Installieren"** oder **"Hinzufügen"**
5. ✅ Die App ist jetzt auf deinem Homescreen!

### iPhone (Safari):
1. Öffne den Link in Safari
2. Tippe auf das **Teilen**-Symbol (Viereck mit Pfeil)
3. Scrolle runter und wähle **"Zum Home-Bildschirm"**
4. Tippe **"Hinzufügen"**
5. ✅ Die App ist jetzt auf deinem Homescreen!

---

## Troubleshooting

### Problem: "404 - File not found"
- **Lösung**: Warte 2-3 Minuten nach dem Aktivieren von GitHub Pages
- Stelle sicher, dass `index.html` im Root-Verzeichnis liegt

### Problem: App lädt nicht
- **Lösung**: Überprüfe, ob das Repository **Public** ist
- Gehe zu Settings → Danger Zone → "Change repository visibility"

### Problem: Keine PWA-Installation möglich
- **Lösung**: GitHub Pages muss über HTTPS laufen (macht es automatisch)
- Öffne die Seite mindestens einmal, damit der Service Worker installiert wird

---

## Dateien aktualisieren

Wenn du später etwas ändern möchtest:

### Über die Website:
1. Gehe zu deinem Repository auf github.com
2. Klicke auf die Datei, die du ändern möchtest
3. Klicke auf das **Stift-Symbol** (Edit)
4. Mache deine Änderungen
5. Scrolle runter und klicke **"Commit changes"**
6. Warte 1-2 Minuten, dann ist die Änderung live

### Über GitHub Desktop:
1. Ändere die Dateien lokal
2. Öffne GitHub Desktop
3. Schreibe eine Commit Message
4. Klicke **"Commit to main"**
5. Klicke **"Push origin"**

---

## 🎯 Dein finaler Link

Nach der Einrichtung kannst du die App aufrufen unter:

```
https://DEIN-USERNAME.github.io/pin-app/
```

**Diesen Link kannst du:**
- Als Lesezeichen speichern
- Per WhatsApp/E-Mail teilen
- Als PWA installieren
- Auf jedem Gerät öffnen

---

## Vorteile von GitHub Pages

✅ **Kostenlos** - Komplett gratis  
✅ **Schnell** - Lädt blitzschnell  
✅ **HTTPS** - Sicher verschlüsselt  
✅ **Zuverlässig** - 99.9% Uptime  
✅ **Einfach** - Keine Server-Konfiguration nötig  

---

## Custom Domain (Optional)

Wenn du eine eigene Domain hast (z.B. `meine-pin-app.de`):
1. Gehe zu Settings → Pages
2. Unter "Custom domain" gib deine Domain ein
3. Konfiguriere deine Domain bei deinem Domain-Provider:
   - Füge einen CNAME Record hinzu, der auf `DEIN-USERNAME.github.io` zeigt

---

Viel Erfolg! 🚀
