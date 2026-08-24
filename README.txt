Tamburi AR v10.20 – Desktop Position/Verzerrung Fix

Problem:
Die Desktop-Vorschau hatte ein anderes Seitenverhältnis als der 1024x768-Export.
Dadurch wurden X und Y mit unterschiedlichen Faktoren übertragen:
- Kasten verschob sich
- Kasten wurde im gespeicherten Bild verzerrt

Fix:
- Sobald am Desktop ein Foto geladen ist, wird die Arbeitsfläche exakt 4:3.
- Diese 4:3-Vorschau entspricht direkt dem späteren 1024x768-Bild.
- Position wird mit einem einzigen einheitlichen Skalierungsfaktor übertragen.
- Modell wird nicht mehr unterschiedlich in X und Y skaliert.
- Größe, Position und 3D-Schwenkung bleiben erhalten.
- Ausgabe weiterhin exakt 1024x768.

Für GitHub nur index.html ersetzen.
