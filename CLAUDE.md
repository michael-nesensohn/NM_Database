# NM_Database – Hinweise für KI-Assistenten

LabVIEW-Bibliothek (VIPM-Paket) für die Kommunikation mit Microsoft SQL Server:
Treibererkennung, Verbindungsaufbau (MSOLEDBSQL), Verbindungsstrings.
Autor: Michael Nesensohn. Lizenz: MIT, kostenlos und ohne kommerziellen Hintergrund.

## Aufbau
- `source/` – LabVIEW-Code: `DB-Tool.lvlib` und die VIs (`SQL_*.vi`)
- `package/NM_Database.vipb` – VIPM-Paketdefinition (Version, Beschreibung, Ziele)
- `NM_Database.lvproj` – LabVIEW-Projekt
- `software-sql-color-*.png` – Paket-Icons
- `LICENSE`, `README.md`, `SECURITY.md`

## Regeln
- LabVIEW-Dateien (`.vi`, `.ctl`, `.lvlib`, `.lvclass`) sind binär: nicht als Text lesen oder ändern,
  keine Merge-Konflikte von Hand auflösen. Änderungen am Code macht der Entwickler in LabVIEW.
- Zielversion: LabVIEW 24.3 (`Package_LabVIEW_Version` in der `.vipb`).
- Nicht ins Repo: `*.vip`, `*.vipc`, `*.aliases`, `*.lvlps`, Build-Ausgaben (siehe `.gitignore`).
- In der `.vipb` keine absoluten Pfade (`C:\...`) eintragen, nur relative.
- Release: Versionsnummer in der `.vipb` erhöhen, gleichen Git-Tag setzen (`vX.Y.Z`),
  `.vip` im VI Package Builder bauen und als GitHub-Release anhängen, nicht committen.
- Der Text in der `.vipb` ist Windows-1252 kodiert (Umlaute); Encoding beim Bearbeiten erhalten.
- Persönliche Daten (E-Mail in `.vipb` und `SECURITY.md`) nur nach Rücksprache ändern oder weitergeben.

## Sprache
Dokumentation und Kommunikation mit dem Entwickler auf Deutsch; Paketbeschreibung für VIPM
darf Deutsch oder Englisch sein.
