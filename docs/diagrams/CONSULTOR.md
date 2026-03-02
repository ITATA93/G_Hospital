---
depends_on:
  - docs/HOSPITAL_OVERVIEW.md
impacts: []
---

# Diagrama: Consultor de Llamado

## Informacion General

| Campo | Valor |
|-------|-------|
| **Archivo fuente** | `CONSULTOR.drawio` |
| **Formato** | draw.io (diagrams.net) XML |
| **Tipo de diagrama** | Diagrama de carriles (swimlane) horizontal |
| **Estado** | Activo |
| **Hospital** | Hospital Provincial del Limari, Ovalle |

## Descripcion del Proceso

Este diagrama representa el **flujo completo del consultor de llamado** en el
Hospital Provincial del Limari. El consultor de llamado es un medico especialista
que se encuentra de turno (guardia pasiva) y es convocado cuando el Servicio de
Urgencias requiere una evaluacion especializada que excede las competencias del
medico de urgencias.

El proceso abarca desde la solicitud inicial hasta el cierre administrativo y
financiero de la prestacion.

## Carriles (Actores / Areas)

El diagrama esta organizado en **6 carriles horizontales**, cada uno representando
un area o rol dentro del hospital:

### 1. Servicio de Urgencias

- **Actores:** Medico de Urgencias, Residente.
- **Funcion:** Origen de la solicitud. El medico de urgencias identifica la
  necesidad de un especialista, realiza comunicacion telefonica con el consultor
  de llamado y genera la solicitud formal.
- **Datos requeridos en la solicitud:**
  - Nombre del medico solicitante
  - Hora del llamado telefonico

### 2. Evaluacion Especialista

- **Actor:** Consultor de llamado (especialista de guardia).
- **Funcion:** El especialista asiste al hospital, registra su ingreso en el
  reloj control, realiza la evaluacion clinica del paciente, contesta la
  interconsulta (estado ejecutado), redacta la evolucion del paciente y completa
  el registro clinico.
- **Secuencia:**
  1. Consultor de llamado recibe la solicitud
  2. Asiste al hospital
  3. Marca reloj control (registro de hora de llegada)
  4. Evaluacion clinica del paciente
  5. Contestar interconsulta (estado: Ejecutado) + Evolucion a paciente
  6. Registro clinico

### 3. Contralor Clinico

- **Actores:** Medico Jefe de Unidad, Especialista Referente.
- **Funcion:** Ambos analizan el caso clinico y generan una "nota a la orden"
  que valida la necesidad y pertinencia de la consulta especializada.
- **Salida:** Solicitud de consultor de llamado validada clinicamente.

### 4. Contralor Horario

- **Actor:** Contralor Horario.
- **Funcion:** Contrasta y verifica los horarios registrados (hora de llamado
  vs. hora de llegada vs. hora de atencion) para asegurar la consistencia
  temporal de la prestacion.
- **Salida:** Solicitud de consultor de llamado verificada en horario.

### 5. Contralor Estadistica

- **Actor:** Contralor Estadistica.
- **Funcion:** Contrasta y verifica los codigos de prestacion, diagnosticos y
  procedimientos para asegurar la correcta codificacion estadistica.
- **Salida:** Solicitud de consultor de llamado verificada en codigos.

### 6. Finanzas

- **Actores:** Contralor Referente, Contralor Finanzas.
- **Funcion:** Recibe la solicitud ya validada clinica, horaria y
  estadisticamente. El Contralor Finanzas verifica y el Contralor Referente
  aprueba para proceder al pago de la prestacion.
- **Salida:** Solicitud de consultor de llamado procesada para pago.

## Flujo Principal

```
Servicio de Urgencias (solicitud)
  --> Consultor de Llamado (evaluacion clinica + registro)
  --> Contralor Clinico (validacion clinica - nota a la orden)
  --> Contralor Horario (verificacion de horarios)
  --> Contralor Estadistica (verificacion de codigos)
  --> Finanzas (procesamiento de pago)
```

## Normativa Aplicable

- Normas internas del Servicio de Salud Coquimbo sobre consultores de llamado.
- Protocolos de interconsulta del Hospital Provincial del Limari.
- Reglamento de control horario para prestaciones de urgencia.
