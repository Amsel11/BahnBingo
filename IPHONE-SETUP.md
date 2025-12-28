# 📱 Bahn-Bingo auf iPhone installieren - Schritt für Schritt

## 🚀 Methode 1: GitHub Pages (Empfohlen - 100% kostenlos)

### Schritt 1: GitHub Repository erstellen

1. Gehe zu [github.com](https://github.com) und logge dich ein (oder erstelle einen Account)
2. Klicke auf das **"+"** Symbol oben rechts → **"New repository"**
3. Repository Name: `bahn-bingo` (oder wie du willst)
4. Wähle **"Public"** (wichtig für kostenloses Hosting!)
5. **NICHT** "Initialize with README" ankreuzen
6. Klicke **"Create repository"**

### Schritt 2: Dateien hochladen

**Option A: Über GitHub Website (Einfachste Methode)**

1. Auf der neuen Repository-Seite, klicke **"uploading an existing file"**
2. Ziehe diese 3 Dateien in den Browser:
   - `bahn-bingo.html`
   - `manifest.json`
   - `sw.js`
3. Klicke **"Commit changes"** (unten)

**Option B: Mit Git (Für Fortgeschrittene)**

```bash
cd c:\dev
git init
git add bahn-bingo.html manifest.json sw.js
git commit -m "Initial commit"
git branch -M main
git remote add origin https://github.com/DEIN-USERNAME/bahn-bingo.git
git push -u origin main
```

### Schritt 3: GitHub Pages aktivieren

1. Im Repository, klicke auf **"Settings"** (oben)
2. Scrolle zu **"Pages"** (links im Menü)
3. Unter **"Source"** wähle: **"Deploy from a branch"**
4. Branch: **"main"** (oder "master"), Folder: **"/ (root)"**
5. Klicke **"Save"**
6. Warte 1-2 Minuten...

### Schritt 4: URL finden

Deine App ist jetzt unter:
```
https://DEIN-USERNAME.github.io/bahn-bingo/bahn-bingo.html
```
(Ersetze `DEIN-USERNAME` mit deinem GitHub Username)

### Schritt 5: Auf iPhone installieren

1. **Öffne Safari** auf deinem iPhone (nicht Chrome!)
2. Gehe zu deiner GitHub Pages URL
3. Tippe auf das **Teilen-Symbol** (Quadrat mit Pfeil nach oben) unten in Safari
4. Scrolle im Menü nach unten
5. Tippe auf **"Zum Home-Bildschirm"**
6. Du kannst den Namen ändern (z.B. "Bahn-Bingo")
7. Tippe **"Hinzufügen"**
8. **Fertig!** 🎉 Die App ist jetzt auf deinem Home-Bildschirm!

---

## 🖥️ Methode 2: Lokaler Server (Nur für Tests)

Wenn du es nur schnell testen willst, ohne GitHub:

### Auf deinem Computer:

1. Öffne Terminal/Command Prompt
2. Gehe zum Projektordner:
   ```bash
   cd c:\dev
   ```
3. Starte einen lokalen Server:

   **Windows (PowerShell):**
   ```powershell
   python -m http.server 8000
   ```
   
   Oder falls Python nicht installiert ist, installiere es von [python.org](https://python.org)

4. Finde deine IP-Adresse:
   - Windows: `ipconfig` im Terminal → Suche nach "IPv4 Address"
   - Beispiel: `192.168.1.100`

### Auf iPhone:

1. Stelle sicher, dass iPhone und Computer im **gleichen WLAN** sind
2. Öffne Safari auf iPhone
3. Gehe zu: `http://192.168.1.100:8000/bahn-bingo.html`
   (Ersetze mit deiner IP-Adresse)
4. Installiere wie in Methode 1, Schritt 5 beschrieben

**⚠️ Hinweis:** Diese Methode funktioniert nur, wenn beide Geräte im gleichen Netzwerk sind!

---

## 🌐 Methode 3: Andere kostenlose Hosting-Optionen

### Netlify Drop (Super einfach!)

1. Gehe zu [app.netlify.com/drop](https://app.netlify.com/drop)
2. Ziehe den ganzen `c:\dev` Ordner in den Browser
3. Fertig! Du bekommst sofort eine URL
4. Öffne die URL auf iPhone und installiere wie oben

### Vercel

1. Gehe zu [vercel.com](https://vercel.com)
2. Verbinde dein GitHub Repository
3. Automatisches Deployment!

---

## ✅ Checkliste

- [ ] GitHub Repository erstellt
- [ ] Dateien hochgeladen (bahn-bingo.html, manifest.json, sw.js)
- [ ] GitHub Pages aktiviert
- [ ] URL auf iPhone in Safari geöffnet
- [ ] "Zum Home-Bildschirm" hinzugefügt
- [ ] App funktioniert! 🎉

## 🆘 Probleme?

**"Service Worker konnte nicht registriert werden"**
- Stelle sicher, dass du HTTPS verwendest (GitHub Pages hat das automatisch)
- Lokaler Server funktioniert nur mit HTTPS für Service Worker

**"App öffnet sich nicht richtig"**
- Verwende Safari, nicht Chrome auf iPhone
- Prüfe, ob die URL korrekt ist

**"Icons fehlen"**
- Das ist OK! Die App funktioniert auch ohne Icons
- Du kannst später `create-icons.html` verwenden, um Icons zu generieren

---

## 💡 Tipp

GitHub Pages ist die beste Option, weil:
- ✅ 100% kostenlos
- ✅ Automatisches HTTPS
- ✅ Funktioniert überall
- ✅ Einfach zu aktualisieren (einfach neue Dateien hochladen)

