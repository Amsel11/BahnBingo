# 🔧 Fix: "Zum Home-Bildschirm" erscheint nicht

## Das Problem:
Safari auf iPhone zeigt "Zum Home-Bildschirm" **NUR** wenn Icons vorhanden sind!

## ✅ Lösung: Icons erstellen und hochladen

### Schritt 1: Icons generieren

1. **Öffne `create-icons.html`** in deinem Browser (lokal oder auf GitHub)
2. Die Seite generiert automatisch 2 Icons
3. **Klicke auf die Download-Links** für:
   - `icon-192.png`
   - `icon-512.png`

### Schritt 2: Icons ins GitHub Repository hochladen

1. Gehe zu: `https://github.com/amsel11/BahnBingo`
2. Klicke **"Add file"** → **"Upload files"**
3. **Ziehe beide Icon-Dateien** (`icon-192.png` und `icon-512.png`) in den Browser
4. Klicke **"Commit changes"**

### Schritt 3: Manifest aktualisieren

Ich habe das Manifest bereits angepasst, aber du musst die Icons hochladen!

Nach dem Hochladen der Icons, aktualisiere `manifest.json`:

```json
{
  "icons": [
    {
      "src": "/BahnBingo/icon-192.png",
      "sizes": "192x192",
      "type": "image/png"
    },
    {
      "src": "/BahnBingo/icon-512.png",
      "sizes": "512x512",
      "type": "image/png"
    }
  ]
}
```

### Schritt 4: Testen

1. **Warte 1-2 Minuten** (GitHub Pages braucht Zeit zum Aktualisieren)
2. Öffne Safari auf iPhone
3. Gehe zu: `https://amsel11.github.io/BahnBingo/`
4. **Tippe auf Teilen-Symbol** (unten)
5. **"Zum Home-Bildschirm"** sollte jetzt erscheinen! ✅

---

## 🚀 Alternative: Ohne Icons (Workaround)

Falls Icons nicht funktionieren, gibt es einen Workaround:

### Methode 1: Über Bookmarks

1. Safari → **Teilen-Symbol**
2. **"Add Bookmark"** wählen
3. Speichere als "Bahn-Bingo"
4. Gehe zu **Bookmarks**
5. Tippe auf "Bahn-Bingo" → **Teilen** → **"Add to Home Screen"**

### Methode 2: Über Shortcuts App (iOS)

1. Öffne **Shortcuts App** auf iPhone
2. **"+"** → **"Add Action"**
3. **"Open URLs"** wählen
4. URL: `https://amsel11.github.io/BahnBingo/`
5. **"Add to Home Screen"**
6. Fertig!

---

## ⚠️ Wichtig:

**Die beste Lösung ist, Icons hinzuzufügen!** Safari zeigt "Add to Home Screen" nur zuverlässig mit Icons.

Nach dem Hochladen der Icons sollte alles funktionieren! 🎉

