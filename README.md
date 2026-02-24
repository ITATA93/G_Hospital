# G_Hospital

> Satellite project in the Antigravity ecosystem — Gemini CLI variant.

**Domain:** `01_HOSPITAL_PRIVADO`
**Status:** Active
**Orchestrator:** GEN_OS
**Prefix:** G_
**AG Counterpart:** `AG_Hospital`

## Proposito

Hub de documentacion y diagramas de procesos hospitalarios para el Hospital
Provincial del Limari. Incluye flujogramas de compras, consultorias y procesos
administrativos del hospital.

- Documentar procesos hospitalarios con diagramas draw.io
- Mantener flujogramas de compras de servicios y consultorias
- Servir como wiki institucional de procesos
- Centralizar documentacion administrativa del hospital

## Arquitectura

```
G_Hospital/
├── .gemini/                          # Configuracion Gemini CLI
├── .claude/                          # Configuracion Claude Code
├── .subagents/                       # Dispatch multi-vendor
├── docs/                             # Documentacion y estandares
├── exports/                          # Exportaciones de sesion
├── Compra de Servicio..drawio        # Flujograma compras
├── CONSULTOR.drawio                  # Flujograma consultorias
├── Diagrama sin titulo.drawio        # Diagrama de trabajo
├── GEMINI.md                         # Perfil Gemini CLI
└── CLAUDE.md                         # Instrucciones Claude Code
```

## Uso con Gemini CLI

```bash
# Revisar procesos documentados
gemini "Lista los procesos hospitalarios documentados en este proyecto"

# Analizar flujograma de compras
gemini "Describe el flujo del proceso de compra de servicios"

# Sugerir mejoras a procesos
gemini "Analiza el flujograma de consultorias y sugiere mejoras"

# Documentar nuevo proceso
gemini "Ayuda a documentar el proceso de adquisicion de insumos"
```

## Scripts

Este proyecto es principalmente documental. Los archivos `.drawio` se editan
con draw.io (diagrams.net) para disenar flujogramas de procesos.

## Configuracion

- `GEMINI.md` -- Perfil del proyecto para Gemini CLI
- `CLAUDE.md` -- Instrucciones para Claude Code
- `docs/standards/` -- Estandares de gobernanza

## Diagramas Disponibles

| Archivo | Proceso |
|---------|---------|
| `Compra de Servicio..drawio` | Flujo de compra de servicios |
| `CONSULTOR.drawio` | Flujo de consultorias externas |
| `Diagrama sin titulo.drawio` | Diagrama de trabajo en progreso |

## Proyectos Relacionados

| Proyecto | Sinergia |
|----------|----------|
| `G_Hospital_Organizador` | Organizacion documental |
| `G_Informatica_Medica` | Estandares y transformacion digital |
| `G_TrakCare_Explorer` | Flujogramas tecnicos del HIS |
