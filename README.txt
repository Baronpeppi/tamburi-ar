Tamburi AR v10.34 – Desktop Verzerrungs-Fix

Problem:
Nach Vergrößerung der Desktop-Arbeitsfläche wurde der 3D-Viewer-Snapshot beim Export
auf 1024x768 gestreckt. Dadurch wirkte der Kasten im gespeicherten Bild breiter.

Fix:
- Snapshot wird nicht mehr auf ein fixes 4:3-Rechteck verzerrt.
- Das native Seitenverhältnis des 3D-Snapshots bleibt erhalten.
- Skalierung erfolgt nur noch gleichmäßig in X und Y.
- Position aus der Desktop-Vorschau bleibt erhalten.
- Große Desktop-Arbeitsfläche aus v10.33 bleibt bestehen.
- Export weiterhin exakt 1024 x 768 px.

Für GitHub nur index.html ersetzen.
