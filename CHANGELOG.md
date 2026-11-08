# Changelog

## 0.1.0 – Phase 1: technisches Fundament
- Monorepo mit gemeinsamer Core-Bibliothek (`core/`), vier Plugin-Ordnern und eigenem Testwerkzeug.
- Neu: RAVE-STATION, MELODY-STUDIO, SPACE-FX als **Fundament-Builds** (nur Testfunktionen, noch keine Plugin-Features).
- NEO//WAVE als viertes Plugin eingehängt (bestehender Funktionsumfang, unverändert).
- Eindeutige Plugin-Codes und Namen, per CMake erzwungen.
- Windows-x64-CI (MSVC), Linux-Referenz-Build, Release-Job für Tags `v*`.
