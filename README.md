# PlaybookLTC für Mac

Fertige Downloads der Mac-App für **PlaybookLTC**, das mitlaufende Spielbuch fürs Mischpult.
Hier liegen nur die gebauten Apps, der Quellcode ist im (privaten) Hauptprojekt.

## Installation

1. Unter **[Releases](../../releases/latest)** die Datei `PlaybookLTC_…_universal.dmg` herunterladen (läuft auf Apple Silicon und Intel, ab macOS 11).
2. Die DMG öffnen und **PlaybookLTC** in den Ordner **Programme** ziehen.
3. **Erster Start**: Die App ist nicht von Apple signiert. macOS blockiert sie deshalb beim ersten Öffnen.
   - Einmal öffnen (die Warnung schließen), dann **Systemeinstellungen → Datenschutz & Sicherheit** → unten **„Trotzdem öffnen“**.
   - Alternativ im Terminal: `xattr -dr com.apple.quarantine /Applications/PlaybookLTC.app`
4. Server-Adresse eintragen (z.B. `10.1.90.2:3006`) → **Speichern & verbinden**.

## Bedienung

- Die App startet im **Vollbild** und verbindet sich automatisch mit dem eingetragenen Server. Ist der Server noch nicht erreichbar, versucht sie es alle 2 Sekunden erneut.
- **⌘,** Einstellungen · **⌘R** neu laden · **⇧⌘R** neu verbinden · **⌃⌘F** Vollbild an/aus
- Der Bildschirm bleibt wach, solange die App läuft (abschaltbar).

## Updates

Die App sucht beim Start und alle 6 Stunden nach einer neuen Version, fragt nach und installiert sie selbst. Manuell: Menü **PlaybookLTC → Nach Updates suchen …**.
Updates sind signiert. Die App installiert nur Pakete aus dem offiziellen Build.
