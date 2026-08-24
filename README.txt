Tamburi AR v10.23 – Handy Screenshot Positions-Fix

Problem:
Nach „✓ Übernehmen“ wechselte die App vom 4:3-Vollbild zurück auf eine anders
proportionierte mobile Vorschau. Dadurch sahen Hintergrund und Kasten versetzt aus.

Fix:
- Mobile Vorschau nach dem Vollbild ist jetzt ebenfalls exakt 4:3.
- Hintergrundfoto bleibt dort mit object-fit: contain identisch zum Vollbild.
- Position/Größe werden erst nach dem Umschalten auf die 4:3-Vorschau angewendet.
- Vollbild, normale Vorschau und Export verwenden damit dasselbe Seitenverhältnis.
- Export bleibt exakt 1024 x 768 px.

Desktop-Funktionen aus v10.22 bleiben unverändert.

Für GitHub nur index.html ersetzen.
