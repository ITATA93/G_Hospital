---
depends_on:
  - docs/HOSPITAL_OVERVIEW.md
impacts: []
---

# Diagrama: Compra de Servicio -- Ruta Clinica Sospecha de Cancer

## Informacion General

| Campo | Valor |
|-------|-------|
| **Archivo fuente** | `Compra de Servicio..drawio` |
| **Formato** | draw.io (diagrams.net) XML |
| **Tipo de diagrama** | Diagrama de carriles (swimlane) vertical |
| **Estado** | Activo |
| **Hospital** | Hospital Provincial del Limari, Ovalle |

## Descripcion del Proceso

Este diagrama representa la **ruta clinica para pacientes con sospecha de cancer
(Ca)** en el Hospital Provincial del Limari. Documenta el flujo completo desde
el ingreso del paciente con sospecha oncologica hasta el tratamiento definitivo
y seguimiento, incluyendo los puntos de decision criticos en cada fase.

El proceso esta alineado con las Garantias Explicitas en Salud (GES) de Chile
para patologias oncologicas y los protocolos del Servicio de Salud Coquimbo.

## Fases del Proceso

El diagrama esta organizado en **4 fases** (carriles verticales):

### Fase 1: Sospecha

- **Entrada:** Ingreso espontaneo o por derivacion.
- **Decision clave:** "Existe sospecha de Ca?" (cancer).
  - **Si:** El paciente avanza a la fase de diagnostico.
  - **No:** El paciente es evaluado y dado de alta del flujo oncologico.

### Fase 2: Diagnostico

- **Evaluacion:** Evaluacion clinica inicial del paciente.
- **Realizacion de examenes:** Solicitud y ejecucion de estudios diagnosticos.
- **Decision:** "Examenes disponibles?"
  - **Si:** Se procede con los examenes correspondientes.
  - **Tipos de examenes:**
    - **Biopsia:** Estudio histopatologico del tejido.
    - **Laboratorio / Imagenologia:** TAC, ecografia (ECO), radiografia (Rx).
- **Decision:** "Se confirma diagnostico?"
  - **Sospecha clinica alta con resultado negativo:** Se reevalua el caso.
  - **Diagnostico confirmado:** Pasa al medico especialista.
- **Medico especialista:** Asume el caso confirmado.
- **Etapificacion:** Clasificacion del estadio de la enfermedad (staging).

### Fase 3: Tratamiento

- **Evaluacion comite quirurgico:** El comite multidisciplinario analiza las
  opciones terapeuticas.
- **Decision:** "Tiene opcion de tratamiento?"
  - **Si:** Se define tratamiento:
    - Radioterapia
    - Quirurgico
    - Farmacologico
  - **No:** Se deriva a:
    - Alivio del dolor y cuidados paliativos.

### Fase 4: Seguimiento

- **Tratamiento y seguimiento:** Control periodico post-tratamiento.
- **Tratamiento con equipo multidisciplinario:** Atencion integral con
  participacion de multiples especialidades.
- **Salida:** Alta o fallecimiento del paciente.

## Flujo Principal

```
Ingreso (espontaneo / derivacion)
  --> Sospecha de Ca? (decision)
    --> [Si] Evaluacion diagnostica
      --> Examenes (biopsia / imagenologia / laboratorio)
        --> Diagnostico confirmado? (decision)
          --> [Si] Medico especialista --> Etapificacion
            --> Comite quirurgico
              --> Tratamiento disponible? (decision)
                --> [Si] Tratamiento (Rt / Qx / Farmacologico)
                  --> Seguimiento multidisciplinario
                    --> Alta o fallecimiento
                --> [No] Cuidados paliativos
          --> [No] Reevaluacion por sospecha alta
    --> [No] Paciente evaluado (fin del flujo)
```

## Puntos de Decision

| Decision | Criterio | Ruta Si | Ruta No |
|----------|----------|---------|---------|
| Existe sospecha Ca? | Evaluacion clinica inicial | Diagnostico | Paciente evaluado (alta) |
| Examenes disponibles? | Disponibilidad en el hospital | Realizar examenes | Derivar/esperar |
| Se confirma diagnostico? | Resultado de examenes | Especialista + etapificacion | Reevaluar sospecha |
| Tiene opcion de tratamiento? | Comite quirurgico | Tratamiento activo | Cuidados paliativos |

## Normativa Aplicable

- Garantias Explicitas en Salud (GES) -- patologias oncologicas cubiertas.
- Guias clinicas del Ministerio de Salud (MINSAL) para cancer.
- Protocolos del Servicio de Salud Coquimbo.
- Normas de derivacion y contrarreferencia de la red asistencial.
