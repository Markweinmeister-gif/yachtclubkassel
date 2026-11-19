# Yacht Club Kassel e.V. – Statische Website

Nachbau der bestehenden Wix-Website (yachtclubkassel.com) als statische, leichte Website.

## Seiten
- `index.html` – Startseite (Tradition & Gemeinschaft, Marina, Ausbildung, Statistiken)
- `termine.html` – Termine & Veranstaltungen
- `kontakt.html` – Kontakt & Anreise
- `impressum.html` – Impressum (Status: Entwurf, vor Veröffentlichung prüfen)
- `datenschutz.html` – Datenschutzerklärung (an statisches Hosting angepasst, vor Veröffentlichung prüfen)
- `404.html` – Fehlerseite
- `css/styles.css` – Design (maritim, responsiv, ohne externe Abhängigkeiten)

## Veröffentlichen mit GitHub Pages
1. Auf github.com ein Repository anlegen, z. B. `yachtclubkassel` (öffentlich oder privat, beide funktionieren mit GitHub Pages).
2. Alle Dateien aus diesem Ordner ins Repository hochladen (per Web-Upload oder `git push`).
3. In den Repositories-Einstellungen unter **Settings → Pages** als Source den Branch `main` (Ordner `/root`) auswählen.
4. Domain verbinden: unter **Settings → Pages → Custom domain** `yachtclubkassel.com` eintragen. GitHub erzeugt automatisch ein HTTPS-Zertifikat.
5. Beim Domain-Registrar (bzw. aktuellen DNS-Verwalter der Domain) diese Einträge setzen:
   - Für Subdomain `www`: CNAME auf `USERNAME.github.io.`
   - Für Apex `yachtclubkassel.com`: A-Records auf `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153`
6. Ergebnis: die Website läuft unter https://yachtclubkassel.com, kostenlos.

## Später pflegen
Einfach die HTML-Dateien im Repository bearbeiten; jede Änderung geht nach dem Commit automatisch online.

## Hinweise
- Impressum und Datenschutzerklärung haben auf der Wix-Site den Status "Entwurf". Vor dem Livegang bitte einmal juristisch prüfen lassen.
- Bilder vom Original (Wix) wurden nicht übernommen, da dort nicht frei zugänglich; eigene Fotos der Marina lassen sich jederzeit nachträglich einbauen.
