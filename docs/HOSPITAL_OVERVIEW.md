---
depends_on:
  - docs/diagrams/CONSULTOR.md
  - docs/diagrams/COMPRA_SERVICIO.md
  - docs/diagrams/DIAGRAMA_BORRADOR.md
  - docs/templates/process_template.md
impacts:
  - README.md
  - CHANGELOG.md
---

# Hospital Provincial del Limari -- Vista General de Procesos

## Acerca del Hospital

El **Hospital Provincial del Limari** es un establecimiento de salud publica ubicado
en la ciudad de **Ovalle, Region de Coquimbo, Chile**. Forma parte de la red
asistencial del Servicio de Salud Coquimbo y atiende a la poblacion de la
Provincia del Limari.

Este repositorio centraliza la documentacion de procesos hospitalarios mediante
diagramas de flujo (formato `.drawio` / diagrams.net) y documentacion asociada.

## Procesos Documentados

### 1. Flujo de Consultor de Llamado

- **Archivo:** `CONSULTOR.drawio`
- **Documentacion:** [docs/diagrams/CONSULTOR.md](diagrams/CONSULTOR.md)
- **Descripcion:** Proceso completo de solicitud, evaluacion y registro del
  consultor de llamado (especialista de guardia). Cubre desde la solicitud
  originada en el Servicio de Urgencias hasta el cierre administrativo en
  Finanzas.
- **Areas involucradas:** Servicio de Urgencias, Evaluacion Especialista,
  Contralor Clinico, Contralor Horario, Contralor Estadistica, Finanzas.

### 2. Flujo de Compra de Servicio (Sospecha de Cancer)

- **Archivo:** `Compra de Servicio..drawio`
- **Documentacion:** [docs/diagrams/COMPRA_SERVICIO.md](diagrams/COMPRA_SERVICIO.md)
- **Descripcion:** Ruta clinica para pacientes con sospecha de cancer (Ca),
  desde el ingreso y sospecha inicial hasta el tratamiento y seguimiento con
  equipo multidisciplinario.
- **Fases:** Sospecha, Diagnostico, Tratamiento, Seguimiento.

### 3. Diagrama sin Titulo (Borrador)

- **Archivo:** `Diagrama sin titulo.drawio`
- **Documentacion:** [docs/diagrams/DIAGRAMA_BORRADOR.md](diagrams/DIAGRAMA_BORRADOR.md)
- **Descripcion:** Diagrama en blanco, reservado como espacio de trabajo para
  futuros procesos por documentar.

## Estructura de Documentacion

```
G_Hospital/
  CONSULTOR.drawio                    # Diagrama: consultor de llamado
  Compra de Servicio..drawio          # Diagrama: ruta clinica sospecha Ca
  Diagrama sin titulo.drawio          # Diagrama: borrador vacio
  docs/
    HOSPITAL_OVERVIEW.md              # Este archivo
    diagrams/
      CONSULTOR.md                    # Documentacion del diagrama consultor
      COMPRA_SERVICIO.md              # Documentacion del diagrama compra servicio
      DIAGRAMA_BORRADOR.md            # Nota sobre el diagrama sin titulo
    templates/
      process_template.md             # Plantilla reutilizable para documentar procesos
```

## Plantilla para Nuevos Procesos

Para documentar un nuevo proceso hospitalario, utilice la plantilla disponible en
[docs/templates/process_template.md](templates/process_template.md). La plantilla
incluye secciones estandarizadas para nombre, objetivo, responsable, pasos,
diagrama asociado y normativa aplicable.

## Proyectos Relacionados

| Proyecto | Relacion |
|----------|----------|
| `G_Hospital_Organizador` | Organizacion documental del hospital |
| `G_Informatica_Medica` | Estandares de informatica medica y transformacion digital |
| `G_TrakCare_Explorer` | Flujogramas tecnicos del sistema HIS (TrakCare) |
| `G_Consultas` | Gestion de consultas medicas |
| `G_Analizador_RCE` | Analisis de registros clinicos electronicos |
