Tamburi AR v10.16 – Positions-Fix Uploadfoto

Problem:
Die Position im Vollbild-Uploadmodus wurde bisher relativ zum gesamten
Smartphone-Bildschirm gespeichert. Der Export ist aber 1024x768 (4:3).
Dadurch verschob sich der Kasten im fertigen Bild.

Fix:
- Im Vollbildmodus gibt es jetzt einen echten 4:3-Aufnahmerahmen.
- Hintergrund + Kasten liegen beide exakt innerhalb dieses Rahmens.
- Position wird relativ zu genau diesem Rahmen gespeichert.
- Export verwendet dieselben normierten X/Y-Werte und dieselbe Skalierung.
- Schwenkwinkel wird ebenfalls exakt aus der bestätigten Vollbildansicht übernommen.
- Ausgabe bleibt immer 1024 x 768 Pixel.

Damit soll gelten:
Was im 4:3-Rahmen vor dem Übernehmen zu sehen ist, ist auch die gespeicherte Position.

Für GitHub nur index.html ersetzen.
