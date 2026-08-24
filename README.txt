Tamburi AR v10.9 – Smartphone/PC Bildimport-Fix

Änderungen:
- Gemeinsamer robuster Bildimport für Smartphone und Desktop.
- JPG/JPEG/PNG/WebP werden zuerst als echte Dateibytes gelesen.
- MIME-Typ wird anhand der Dateiendung korrigiert.
- Bild wird über createImageBitmap dekodiert und als sauberes JPG neu aufgebaut.
- Dadurch robuster bei Samsung Gallery, Android-Dateiauswahl, OneDrive-Dateien und Windows-Dateien.
- HEIC/HEIF-Unterstützung bleibt erhalten.
- Fehlermeldung zeigt jetzt zusätzlich Dateityp und Dateigröße.
- Desktop-Hintergrund-Fix aus v10.8 bleibt erhalten.

Für GitHub nur index.html ersetzen.
