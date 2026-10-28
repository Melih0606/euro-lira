# Euro ↔ Lira – iPhone-Web-App

Eine reine HTML/CSS/JavaScript-App. Kein Python, Build-Tool, API-Schlüssel oder App-Store nötig.

## Veröffentlichen über GitHub Pages

1. Auf https://github.com einloggen (kostenloses Konto bei Bedarf erstellen).
2. Ein **öffentliches** Repository anlegen, z. B. `euro-lira`.
3. Alle **sechs Dateien** aus diesem Ordner in das Hauptverzeichnis des Repositories hochladen (nicht den ZIP-Ordner selbst).
4. Unter **Settings → Pages → Build and deployment → Source** die Option **Deploy from a branch** auswählen.
5. Branch `main`, Ordner `/(root)` auswählen und **Save** anklicken.
6. Die unter Pages angezeigte HTTPS-Adresse öffnen (typischerweise `https://BENUTZERNAME.github.io/euro-lira/`). Die Bereitstellung kann einige Minuten benötigen.
7. Auf dem iPhone die URL in **Safari** öffnen → **Teilen** → **Zum Home-Bildschirm** → **Als Web-App öffnen** aktivieren → **Hinzufügen**.

## Lokal testen

Im Ordner `python -m http.server 8000` ausführen, dann am Computer `http://localhost:8000` öffnen. Das iPhone braucht zum Installieren eine veröffentlichte HTTPS-Adresse.

## Daten und Offlinebetrieb

- Referenzkurse: https://frankfurter.dev/ (tägliche Aktualisierung, nicht tickgenau live).
- Zum Abruf neuer Kurse ist Internet nötig.
- Der letzte erfolgreich abgerufene Kurs wird im Browser gespeichert; bei Internetausfall kann damit weiter umgerechnet werden.
- Service Worker speichert App-Dateien offline, sofern die Seite über HTTPS geladen wurde.
- Keine Serverkomponente; alle Rechenoperationen finden auf dem Gerät statt.
