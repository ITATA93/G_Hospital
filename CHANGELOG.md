---
depends_on: []
impacts: []
---

# Changelog — G_Hospital

All notable changes to this project will be documented in this file.
Format follows [Keep a Changelog](https://keepachangelog.com/en/1.1.0/).

## [Unreleased]

### Added

- docs/HOSPITAL_OVERVIEW.md: vista general de procesos documentados del Hospital Provincial del Limari
- docs/diagrams/CONSULTOR.md: documentacion del diagrama de consultor de llamado (6 carriles: Urgencias, Especialista, Contralor Clinico, Contralor Horario, Contralor Estadistica, Finanzas)
- docs/diagrams/COMPRA_SERVICIO.md: documentacion del diagrama de ruta clinica sospecha de cancer (4 fases: Sospecha, Diagnostico, Tratamiento, Seguimiento)
- docs/diagrams/DIAGRAMA_BORRADOR.md: nota sobre diagrama vacio reservado para uso futuro
- docs/templates/process_template.md: plantilla reutilizable para documentar procesos hospitalarios (secciones: Nombre, Objetivo, Responsable, Pasos, Diagrama Asociado, Normativa Aplicable)

### Changed

- docs/TODO.md: 3 items de backlog marcados como completados

### Previous Unreleased

- Governance audit: docs/TODO.md verified
- README.md enhanced with architecture and usage docs
- Gemini CLI integration validated

## [1.0.0] — 2026-02-23

### Added

- Full GEN_OS mirror infrastructure migrated from AG_Hospital.
- Multi-vendor dispatch: .subagents/, .claude/, .codex/, .gemini/, .agent/.
- Governance standards: docs/standards/.
- CI/CD workflows: .github/workflows/.
- All domain content preserved from AG_Hospital.
