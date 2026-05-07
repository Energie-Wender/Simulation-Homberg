# Projektstatus: Aktiv

**Entscheidung am:** 2026-03-14
**Zuletzt aktualisiert:** 2026-05-07
**Repository:** https://github.com/Energie-Wender/Simulation-Homberg
**Organisation:** Energie-Wender
**Lokaler Pfad (WSL):** `/home/jsp/source/Energie-Wender/Simulation-Homberg`
**Lokaler Pfad (Windows):** `C:\Users\joern\source\Energie-Wender\Simulation-Homberg`

> **Hinweis:** Der WSL-Klon heißt bereits `Simulation-Homberg`. Ob der Windows-
> Klon noch unter `Sim-Homberg` liegt, ist nicht überprüft — bitte ggf. manuell
> umbenennen (außerhalb WSL, da `mv` auf NTFS verschachtelte Verzeichnisse
> erzeugt statt umzubenennen).

---

## Zusammenfassung der Analyse

Das Projekt enthält drei MATLAB/Simulink-Modelle (.slx) für Fahrdynamik-Simulationen:
- **TannenwegFinal.slx** — Streckenmodell Tannenweg (finale Version)
- **SpeedOptimisedVersionTannenweg.slx** — Geschwindigkeitsoptimierte Variante
- **workingGT3nomasknwithcontrol.slx** — GT3-Fahrzeugmodell mit Regelung

### Identifizierte Probleme
- Keine Dokumentation zu den Simulink-Modellen vorhanden
- Keine einheitliche Dateibenennungskonvention
- Keine MATLAB-Projektdatei (.prj)
- Keine Parameterdateien — alles vermutlich in den Modellen hartkodiert
- Keine Tests vorhanden
- .github/ enthält noch GitHub-Skills-Übungsdateien (nicht projektrelevant)

### Durchgeführte Maßnahmen
- Grundanalyse erstellt (docs/ANALYSIS.md)
- Test-Setup-Planung erstellt (docs/Test-Setup.md)
- Repository von `AsherFerdinand/MatlabSimulink` nach `Energie-Wender/Simulation-Homberg` überführt
- Lokales Verzeichnis nach `C:\Users\joern\source\Energie-Wender\` verschoben

---

## Aktuell geplante nächste Schritte

- [x] Grundanalyse durchgeführt (docs/ANALYSIS.md)
- [x] Test-Setup-Planung erstellt (docs/Test-Setup.md)
- [x] Repository in Organisation "Energie-Wender" überführt und umbenannt
- [x] Lokales Verzeichnis verschoben
- [x] Dokumentation auf aktuellen Stand gebracht
- [x] Lokales WSL-Verzeichnis heißt `Simulation-Homberg` (Windows-Klon ggf. noch prüfen)
- [x] README.md mit projektrelevanter Beschreibung ersetzen
- [ ] .github/-Übungsdateien aufräumen (Steps und Workflows entfernen)
- [ ] PROFILE.md entfernen (stammt aus GitHub-Skills-Übung)
- [ ] Einheitliche Dateibenennungskonvention für .slx-Dateien einführen
- [ ] MATLAB-Projektdatei (.prj) erstellen
- [ ] Parameterdateien aus den Modellen extrahieren
- [ ] Test-Setup mit matlab.unittest implementieren
