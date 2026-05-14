# 🧊 SmartFridge

Willkommen bei der offiziellen Dokumentation von SmartFridge.

SmartFridge ist eine moderne Open-Source-Webanwendung zur Verwaltung von Lebensmitteln, Rezepten und KI-gestützter Küchenunterstützung.

---

## ✨ Features

<div class="grid cards" markdown>

-   :material-fridge-outline: __Lebensmittelverwaltung__

    ---

    Verwalte Produkte, Mengen und Ablaufdaten zentral an einem Ort.

-   :material-robot-outline: __KI-Unterstützung__

    ---

    Generiere Rezepte und Vorschläge mit OpenAI, Gemini oder Ollama.

-   :material-cellphone: __PWA Unterstützung__

    ---

    Nutze SmartFridge auf Smartphone, Tablet oder Desktop wie eine normale App.

-   :material-home-assistant: __Home Assistant__

    ---

    Integration über HACS inklusive eigener Dashboard-Karte.

-   :material-api: __REST API__

    ---

    Greife über eine einfache API auf deine Daten zu.

-   :material-account-group-outline: __Mehrbenutzer__

    ---

    Unterstützung für mehrere Benutzer und persönliche Daten.

</div>

---

## 🧠 Unterstützte KI-Anbieter

=== "OpenAI"

    - GPT Modelle
    - Cloudbasiert
    - API-Key erforderlich

=== "Google Gemini"

    - Gemini API
    - Schnelle Antworten
    - API-Key erforderlich

=== "Ollama"

    - Lokale KI Modelle
    - Datenschutzfreundlich
    - Keine Cloud notwendig

---

## 🔄 Systemübersicht

```mermaid
graph TD
    A[Benutzer] --> B[SmartFridge]
    B --> C[Produkte]
    B --> D[Rezepte]
    B --> E[KI Anbieter]
    B --> F[REST API]
    F --> G[Home Assistant]
```

---

## 📚 Dokumentation

!!! tip "Empfohlen"

    Neue Nutzer sollten mit der Installationsanleitung beginnen und danach den Sicherheitsbereich lesen.

<div class="grid cards" markdown>

-   :material-download: __Installation__

    ---

    Einrichtung auf Linux, macOS, Windows und Raspberry Pi.

    [:octicons-arrow-right-24: Zur Installation](installation.md)

-   :material-shield-lock-outline: __Sicherheit__

    ---

    Produktionshinweise und bekannte Einschränkungen im aktuellen Stand.

    [:octicons-arrow-right-24: Zur Sicherheit](sicherheit.md)

-   :material-cog-outline: __Administration__

    ---

    Benutzerverwaltung, KI-Einstellungen und API-Key-Verwaltung.

    [:octicons-arrow-right-24: Zur Administration](admin.md)

-   :material-api: __API__

    ---

    Endpunkte, Authentifizierung und Beispielanfragen.

    [:octicons-arrow-right-24: Zur API](api.md)

-   :material-lifebuoy: __Troubleshooting__

    ---

    Typische Fehlerbilder und schnelle Lösungen.

    [:octicons-arrow-right-24: Zum Troubleshooting](troubleshooting.md)

</div>

---

## 🔗 Links

| Projekt | Link |
|---|---|
| SmartFridge PWA | https://github.com/henristr/SmartFridgePWA |
| Android App | https://github.com/henristr/SmartFridgeAndroid |
| Home Assistant | https://github.com/henristr/FridgeAssistant |

---

## ❤️ Open Source

SmartFridge ist ein Open-Source Projekt und wird aktiv weiterentwickelt.
