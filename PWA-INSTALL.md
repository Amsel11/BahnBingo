# Bahn-Bingo als Phone App installieren

Diese App ist jetzt eine **Progressive Web App (PWA)** und kann auf deinem Handy installiert werden!

## 📱 Installation

### Android (Chrome/Edge)
1. Öffne die App im Browser (Chrome oder Edge)
2. Tippe auf das Menü (3 Punkte oben rechts)
3. Wähle **"Zur Startseite hinzufügen"** oder **"Zum Startbildschirm hinzufügen"**
4. Bestätige die Installation
5. Die App erscheint jetzt wie eine normale App auf deinem Startbildschirm!

### iPhone/iPad (Safari)
1. Öffne die App im Safari Browser
2. Tippe auf das **Teilen-Symbol** (Quadrat mit Pfeil nach oben)
3. Scrolle nach unten und wähle **"Zum Home-Bildschirm"**
4. Tippe auf **"Hinzufügen"**
5. Die App erscheint jetzt auf deinem Home-Bildschirm!

## 🎨 Icons hinzufügen (Optional)

Für schönere App-Icons:

1. Öffne `create-icons.html` im Browser
2. Die Icons werden automatisch generiert und können heruntergeladen werden
3. Speichere `icon-192.png` und `icon-512.png` im gleichen Ordner wie `bahn-bingo.html`
4. Die App verwendet diese Icons automatisch!

## ✨ Features

- ✅ Funktioniert offline (nach erstem Laden)
- ✅ Sieht aus wie eine native App
- ✅ Keine App Store nötig
- ✅ Automatische Updates
- ✅ Alle Daten werden lokal gespeichert

## 🔧 Technische Details

- **Manifest**: `manifest.json` - Definiert App-Name, Icons, etc.
- **Service Worker**: `sw.js` - Ermöglicht Offline-Funktionalität
- **Icons**: `icon-192.png` und `icon-512.png` (optional)

## 🚀 Deployment

Um die App online zu stellen:

1. Lade alle Dateien auf einen Webserver hoch:
   - `bahn-bingo.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png` (optional)
   - `icon-512.png` (optional)

2. Stelle sicher, dass der Server HTTPS verwendet (für Service Worker)

3. Öffne die App im Browser und installiere sie!

## 📝 Hinweise

- Die App funktioniert am besten mit HTTPS
- Service Worker funktionieren nur auf HTTPS oder localhost
- Alle Daten werden im Browser-LocalStorage gespeichert

