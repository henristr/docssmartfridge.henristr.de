# 🛜 SmartFridge API

!!! example "Überblick"

    SmartFridge stellt eine externe REST API für Produktdaten bereit.

---

## 🔐 Authentifizierung

Die externe API nutzt einen Header mit API-Key.

| Header | Wert |
|---|---|
| `API-Key` | Dein in SmartFridge gesetzter Schlüssel |

Den API-Key setzt du als Admin im Bereich **API-Einstellungen**.

---

## 📦 Externe API

### `GET /api/products`

Liefert den Inhalt aus `produkte.json` als JSON zurück.

=== "Request"

    ```http
    GET https://deine-installation.com/api/products
    API-Key: dein-key
    ```

=== "cURL"

    ```bash
    curl -X GET https://deine-installation.com/api/products \
      -H "API-Key: dein-key"
    ```

=== "Antwort"

    ```json
    {
      "admin": [
        {
          "name": "Milch",
          "ablauf": "2026-05-20"
        }
      ]
    }
    ```

!!! warning "Unauthorized"

    Ist kein API-Key gesetzt oder stimmt der Header nicht, antwortet die API mit `401 Unauthorized`.

---

## 🧩 Interne API (für Weboberfläche)

Diese Endpunkte werden von der SmartFridge-Oberfläche genutzt:

- `/api/change-password`
- `/api/get-diet`
- `/api/save-diet`
- `/api/ai-config` (nur Admin)
- `/api/generate-recipe`
- `/api/recipe-history`
- `/api/toggle-favorite`
- `/api/admin/api-settings` (nur Admin)

!!! info "Hinweis"

    Diese Endpunkte sind für die interne Nutzung gedacht und setzen eine aktive Session voraus.
