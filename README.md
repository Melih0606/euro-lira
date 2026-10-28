# Euro ↔ Lira – iPhone-Web-App

Eine reine HTML/CSS/JavaScript-App. Kein Python, Build-Tool, API-Schlüssel oder App-Store nötig.

Auf dem iPhone die URL in **Safari** öffnen → **Teilen** → **Zum Home-Bildschirm** → **Als Web-App öffnen** aktivieren → **Hinzufügen**.

## Daten und Offlinebetrieb

- Referenzkurse: https://frankfurter.dev/ (tägliche Aktualisierung, nicht tickgenau live).
- Zum Abruf neuer Kurse ist Internet nötig.
- Der letzte erfolgreich abgerufene Kurs wird im Browser gespeichert; bei Internetausfall kann damit weiter umgerechnet werden.
- Service Worker speichert App-Dateien offline, sofern die Seite über HTTPS geladen wurde.
- Keine Serverkomponente; alle Rechenoperationen finden auf dem Gerät statt.
