Tamburi AR v10.35 – Desktop Schwenk-Positions-Fix

Problem:
Ohne Schwenken stimmte die Position im gespeicherten Bild.
Nach dem Schwenken verschob sich der Kasten im Export.

Ursache:
Der 3D-Snapshot hatte intern ein anderes Seitenverhältnis als die 4:3-Arbeitsfläche.
Beim proportionalen Einpassen änderte sich dadurch die Lage des sichtbaren Modells,
besonders deutlich nach einer 3D-Schwenkung.

Fix:
- 3D-Snapshot wird vor dem Export mittig und unverzerrt auf exakt 4:3 beschnitten.
- Danach werden Größe und X/Y-Position 1:1 auf 1024x768 übertragen.
- Der Kasten bleibt auch nach dem Schwenken an derselben Stelle wie in der Vorschau.
- Keine Verzerrung des Modells.
- Große Desktop-Arbeitsfläche bleibt erhalten.

Für GitHub nur index.html ersetzen.
