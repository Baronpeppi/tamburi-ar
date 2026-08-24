Tamburi AR v10.18 – Desktop Auswahl- und Export-Fix

Behoben:
1) Blaues Markieren beim Verschieben
- Browser-Text-/Bildauswahl im Desktop-Vorschaubereich deaktiviert.
- Hintergrundfoto ist nicht mehr draggable.
- Pointer-Drag verhindert Standard-Browserauswahl.
- Beim Verschieben wird nur der Kasten bedient.

2) Gespeichertes Desktopfoto war zu klein
Ursache:
- Canvas war 1024x768, aber Hintergrund und Modell wurden noch in den Pixelmaßen
  der Bildschirm-Vorschau hineingezeichnet.
- Dadurch belegte das eigentliche Foto nur einen Teil des 1024x768-Bildes.

Fix:
- Export rechnet Vorschaukoordinaten jetzt sauber auf 1024x768 um.
- Hintergrundbild füllt den verfügbaren 4:3-Bereich proportional.
- Position und Größe des Kastens werden proportional aus der Desktop-Vorschau übertragen.
- 3D-Schwenkwinkel bleibt erhalten.
- Ausgabe immer exakt 1024x768 Pixel.

Für GitHub nur index.html ersetzen.
