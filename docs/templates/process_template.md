---
depends_on:
  - docs/HOSPITAL_OVERVIEW.md
impacts: []
---

# Plantilla de Documentacion de Proceso Hospitalario

> Copie esta plantilla para documentar un nuevo proceso del Hospital Provincial
> del Limari. Complete cada seccion segun corresponda y elimine las instrucciones
> entre parentesis.

---

## Nombre del Proceso

(Escriba el nombre oficial del proceso. Ejemplo: "Solicitud de Consultor de
Llamado", "Compra de Servicio por Sospecha de Cancer".)

## Codigo del Proceso

(Asigne un codigo unico. Ejemplo: PROC-URG-001, PROC-ADM-002.)

## Objetivo

(Describa el proposito principal del proceso. Que se busca lograr y por que
es relevante para el hospital.)

Ejemplo:
> Asegurar que las solicitudes de consultor de llamado se tramiten de forma
> oportuna, con validacion clinica, horaria, estadistica y financiera.

## Alcance

(Indique los limites del proceso: donde comienza y donde termina. Que areas
y actores estan involucrados.)

## Responsable

| Rol | Nombre / Cargo | Area |
|-----|---------------|------|
| Responsable del proceso | (Nombre o cargo) | (Area / servicio) |
| Ejecutor principal | (Nombre o cargo) | (Area / servicio) |
| Validador | (Nombre o cargo) | (Area / servicio) |

## Definiciones y Abreviaturas

| Termino | Definicion |
|---------|-----------|
| (Termino 1) | (Definicion) |
| (Termino 2) | (Definicion) |

## Pasos del Proceso

### Paso 1: (Nombre del paso)

- **Responsable:** (Quien ejecuta este paso)
- **Entrada:** (Que insumo o informacion necesita)
- **Accion:** (Descripcion de lo que se debe hacer)
- **Salida:** (Que produce este paso)
- **Tiempo estimado:** (Duracion esperada)

### Paso 2: (Nombre del paso)

- **Responsable:** (Quien ejecuta este paso)
- **Entrada:** (Que insumo o informacion necesita)
- **Accion:** (Descripcion de lo que se debe hacer)
- **Salida:** (Que produce este paso)
- **Tiempo estimado:** (Duracion esperada)

### Paso 3: (Nombre del paso)

(Agregue tantos pasos como sean necesarios.)

## Puntos de Decision

| # | Pregunta | Criterio | Ruta Si | Ruta No |
|---|----------|----------|---------|---------|
| 1 | (Pregunta de decision) | (Como se decide) | (Siguiente paso si es Si) | (Siguiente paso si es No) |

## Diagrama Asociado

| Campo | Valor |
|-------|-------|
| **Archivo del diagrama** | (Nombre del archivo .drawio) |
| **Ubicacion** | (Ruta relativa dentro del repositorio) |
| **Documentacion del diagrama** | (Enlace al .md en docs/diagrams/) |

> Para crear o editar el diagrama, abra el archivo `.drawio` con
> [diagrams.net](https://app.diagrams.net/) o la extension de VS Code.

## Normativa Aplicable

- (Norma, ley, decreto o protocolo que rige este proceso.)
- (Ejemplo: Garantias Explicitas en Salud -- GES.)
- (Ejemplo: Protocolos del Servicio de Salud Coquimbo.)
- (Ejemplo: Normas internas del Hospital Provincial del Limari.)

## Indicadores de Desempeno

| Indicador | Formula / Descripcion | Meta |
|-----------|-----------------------|------|
| (Nombre del indicador) | (Como se mide) | (Valor objetivo) |

## Registros y Evidencia

| Documento | Responsable | Retencion |
|-----------|-------------|-----------|
| (Nombre del registro) | (Quien lo genera) | (Tiempo de conservacion) |

## Historial de Cambios

| Fecha | Version | Descripcion del Cambio | Autor |
|-------|---------|----------------------|-------|
| (Fecha) | 1.0 | Creacion inicial del documento | (Nombre) |

---

> **Nota:** Una vez completada la documentacion, agregar la referencia del nuevo
> proceso en `docs/HOSPITAL_OVERVIEW.md` y actualizar `CHANGELOG.md`.
