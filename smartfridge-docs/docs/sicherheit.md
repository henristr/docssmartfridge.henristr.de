# 🔒 Sicherheit

SmartFridge ist für den privaten Betrieb konzipiert und sollte bewusst abgesichert werden.

---

## ⚠️ Aktuelle Sicherheitsrelevante Punkte

!!! danger "Passwortspeicherung"

    Benutzer und Passwörter werden aktuell unverschlüsselt in `users.json` gespeichert.

!!! warning "Session-Secret"

    Die Anwendung nutzt in der Standardkonfiguration ein statisches Secret in `app.py`.

!!! warning "Debug-Modus"

    Die Anwendung wird im aktuellen Stand mit aktiviertem Debug-Modus gestartet.

!!! warning "API-Key-Speicherung"

    Der externe API-Key wird als Klartext in `config.json` gespeichert.

---

## ✅ Empfehlungen für den Betrieb

1. Nur im privaten Netzwerk oder hinter VPN betreiben
2. Reverse Proxy mit TLS verwenden (z. B. Caddy oder Nginx)
3. Standard-Admin-Passwort sofort ändern
4. API-Key nur an vertrauenswürdige Integrationen weitergeben
5. Daten-Dateien regelmäßig sichern

---

## 🌐 Reverse Proxy Beispiele

=== "Caddy"

    ```caddy
    smartfridge.example.com {
        reverse_proxy localhost:8080
    }
    ```

=== "Nginx"

    ```nginx
    server {
        server_name smartfridge.example.com;

        location / {
            proxy_pass http://localhost:8080;
        }
    }
    ```

---

## 🚫 Nicht empfohlen

- Direkte Portfreigabe ins öffentliche Internet
- Betrieb mit unverändertem Standard-Login
- Teilen des API-Keys in öffentlichen Dashboards oder Repositories
