Tamburi AR v10.10 – Smartphone Foto-Upload Fix

Ursache gefunden:
Der Bildimport selbst funktionierte bereits. Danach griff die App noch auf den
alten, inzwischen entfernten DOM-Button #arButton zu. Dadurch entstand:
"Cannot read properties of null (reading 'style')"

Fix:
- Zugriff auf den alten #arButton abgesichert.
- Foto-Upload kann danach normal in den Positionierungsmodus wechseln.
- Desktop-/Varianten-/Kamera-Funktionen bleiben unverändert.

Für GitHub nur index.html ersetzen.
