# PP Erfassung

Kleine Web-App (PWA) fürs iPhone: Zinsen, Zinsbelastungen, Gebühren und Gebührenerstattungen
unterwegs erfassen und als CSV in Portfolio Performance (PP) importieren.

## Ablauf
1. App im Safari öffnen → Teilen → «Zum Home-Bildschirm».
2. «Konten aus PP-Datei laden» → PP-Datei in iCloud Drive wählen (nur lesend; XML, Binär und ZIP
   werden unterstützt, passwortgeschützte Dateien nicht – dann Konten manuell anlegen).
3. Buchungen erfassen. Bei Zinsen: Bruttozins + Steuern (Knopf «VST 35 %»); gebucht wird netto mit Steuer-Anteil.
4. «CSV teilen» → «In Dateien sichern» → iCloud Drive.
5. Am Mac in PP: Datei → Importieren → CSV-Dateien → Typ **Kontoumsätze**, Trennzeichen `;`,
   Datumsformat `yyyy-MM-dd`, Zahlenformat `1,234.56`. Die Spalten werden anhand der Überschriften
   automatisch zugeordnet; die Konfiguration kann in PP als Vorlage gespeichert werden.

Warum CSV statt direkt in die PP-Datei schreiben? PP hält die Datei im Speicher und überschreibt sie
beim nächsten Speichern – parallele Änderungen vom iPhone gingen dabei verloren oder erzeugen
iCloud-Konflikte. Der CSV-Import ist der sichere Weg, und PP zeigt vor dem Import eine Vorschau.

Daten bleiben ausschliesslich lokal auf dem iPhone (Browser-Speicher).
