Tamburi AR v10.19 – Vollbild-Steuerung wiederhergestellt

Ursache:
- In v10.17/v10.18 wurde der alte Desktop-Drehungsregler entfernt.
- Im JavaScript blieb aber noch eine alte Zeile `desktopRotate.step='1'`.
- Dadurch entstand ein JavaScript-Fehler und spätere Steuerungslogik konnte nicht sauber initialisiert werden.

Fix:
- Alte Referenz vollständig entfernt.
- Vollbild-Steuerung für Verschieben, Schwenken und Zoomen wieder aktiv.
- Desktop-Modi aus v10.18 bleiben erhalten.
- Export-Fix aus v10.18 bleibt erhalten.

Für GitHub nur index.html ersetzen.
