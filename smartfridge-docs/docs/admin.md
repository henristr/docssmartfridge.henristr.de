# ⚙️ Administration

Diese Seite beschreibt die wichtigsten Admin-Funktionen in SmartFridge.

---

## 👤 Admin-Benutzer

Beim ersten Start wird automatisch ein Benutzer `admin` erstellt.

| Benutzername | Passwort |
|---|---|
| admin | admin |

!!! warning "Pflicht nach Erststart"

    Ändere das Admin-Passwort direkt nach der Installation.

---

## 👥 Benutzerverwaltung

Als Admin kannst du:

- neue Benutzer anlegen
- vorhandene Benutzer löschen
- den eigenen Admin-Zugang verwalten

!!! info "Einschränkung"

    Der Benutzer `admin` selbst kann nicht gelöscht werden.

---

## 🤖 KI-Verwaltung

Im Admin-Bereich kann der KI-Anbieter eingestellt werden:

- Google Gemini
- OpenAI
- Ollama (lokal)

Zusätzlich können API-Key und Modell pro Anbieter gesetzt werden.

---

## 🔑 API-Key Verwaltung

Für externe Integrationen (z. B. Home Assistant) setzt der Admin den API-Key über den API-Bereich.

Der Key wird für den Endpunkt `/api/products` benötigt und über den Header `API-Key` übergeben.

---

## 🧾 Wichtige Dateien

| Datei | Zweck |
|---|---|
| `users.json` | Benutzerkonten und Passwörter |
| `ai_config.json` | KI-Anbieter, Modelle und Schlüssel |
| `config.json` | API-Key für externe API |
| `rezepte.json` | Rezept-Historie pro Benutzer |
