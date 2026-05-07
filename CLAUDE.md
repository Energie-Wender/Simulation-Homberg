# Hinweise für Claude Code

## Einstiegspunkt

1. **`devstate_active.md`** (Wurzelverzeichnis) — aktueller Projektstatus, durchgeführte Maßnahmen, nächste Schritte. Bei jedem Arbeitsschritt aktuell halten.
2. **`_claude-session/RESUME.md`** (sofern vorhanden, unversioniert) — frischer Briefing-Snapshot der letzten Session mit priorisierten offenen Punkten.
3. **`docs/ANALYSIS.md`** — detaillierte Projektanalyse.
4. **`docs/Test-Setup.md`** — Planung des Test-Frameworks.

## Konventionen

- **Kommunikation mit dem User:** Deutsch.
- **Code, Kommentare, Commits:** Englisch.
- **Dokumentation in `docs/`:** Deutsch.
- `devstate_*.md` und `README.md` im **Wurzelverzeichnis**, alle anderen `.md` in `docs/`.
- Bei Zweifel **nachfragen**, bevor Code erzeugt oder Dateien geändert werden.
- Nach jeder Umbauphase **Commit anbieten** (nicht selbst committen).

## Projektkontext

MATLAB/Simulink-Modelle für Fahrdynamik-Simulationen. Drei `.slx`-Dateien (binär, nicht CLI-analysierbar), keine `.m`-Skripte, keine Tests, keine `.prj`-Datei. Repo: `Energie-Wender/Simulation-Homberg` (vormals `AsherFerdinand/MatlabSimulink`).
