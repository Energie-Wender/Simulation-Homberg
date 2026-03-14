# Test-Setup

## Status

Aktuell ist **kein Test-Framework** im Projekt eingerichtet.

## Geplantes Framework

**MATLAB Unit Test Framework (`matlab.unittest`)** — MATLABs integriertes Test-Framework.

### Voraussetzungen
- MATLAB (Version abhängig von den Simulink-Modellen)
- Simulink
- Ggf. weitere Toolboxen (Simscape, Vehicle Dynamics Blockset, Control System Toolbox)

## Geplante Tests

### Unit-Tests
- Modell-Ladetests: Prüfen, ob jedes Modell fehlerfrei geladen werden kann
- Simulationslauffähigkeit: Prüfen, ob jedes Modell ohne Fehler simuliert werden kann
- Parametervalidierung: Prüfen, ob alle benötigten Workspace-Variablen definiert sind

### Integrationstests
- Ergebnisvergleich: Simulationsergebnisse gegen Referenzdaten prüfen
- Variantenvergleich: TannenwegFinal vs. SpeedOptimisedVersion — Ergebnisse vergleichen

## Testausführung

```matlab
% Alle Tests ausführen
results = runtests('tests');

% Einzelnen Test ausführen
result = runtests('tests/LoadModelTest.m');
```

> **Hinweis:** Tests können nur in einer MATLAB-Umgebung ausgeführt werden, nicht in WSL/Linux ohne MATLAB-Installation.
