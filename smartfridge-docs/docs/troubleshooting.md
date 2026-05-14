# 🛠️ Troubleshooting

Häufige Probleme und schnelle Lösungen für SmartFridge.

---

## 🔐 Login funktioniert nicht

### Symptom
Benutzername oder Passwort wird nicht akzeptiert.

### Lösung
1. Prüfen, ob Benutzer korrekt geschrieben ist
2. Standarddaten testen (`admin` / `admin`) falls Erststart
3. Bei lokalem Test `users.json` prüfen

---

## 🤖 Rezeptgenerierung schlägt fehl

### Symptom
Rezept kann nicht generiert werden oder es erscheint eine Fehlermeldung.

### Lösung
1. KI-Anbieter im Admin-Bereich prüfen
2. API-Key kontrollieren (Gemini/OpenAI)
3. Bei Ollama URL und Modell prüfen
4. Erneut versuchen, nachdem Produkte vorhanden sind

---

## 📡 Externe API liefert 401 Unauthorized

### Symptom
`GET /api/products` antwortet mit 401.

### Lösung
1. Prüfen, ob ein API-Key gesetzt wurde
2. Header exakt als `API-Key` senden
3. Alten Schlüssel in Clients durch den aktuellen ersetzen

---

## 📲 PWA wird nicht installiert

### Symptom
Browser zeigt keine Installationsoption.

### Lösung
1. HTTPS bzw. sicheres Umfeld verwenden
2. In unterstütztem Browser testen (z. B. Chrome, Edge)
3. Seite neu laden und Browser-Cache leeren

!!! info "Hinweis"

    Die PWA-Installation ist verfügbar. Ein vollständiger Offline-Modus ist aktuell noch nicht aktiv.

---

## 📦 Daten scheinen verschwunden

### Symptom
Produkte, Nutzer oder Rezepte fehlen.

### Lösung
1. Prüfen, ob JSON-Dateien gelöscht wurden
2. Backup der Dateien zurückspielen
3. Dateirechte des SmartFridge-Verzeichnisses prüfen
