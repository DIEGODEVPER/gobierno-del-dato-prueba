---
title: "Procedimiento Corporativo de Remediación de Datos — DG-PRO-PCRD-MINS-001 v1.0"
code: DG-PRO-PCRD-MINS-001
version: "1.0"
source_file: "DG-PRO-PCRD-MINS-001-Procedimiento Corporativo de Remediación de Datos v1.0.docx"
layout: default
description: "Procedimiento para corregir incidencias de calidad de datos, roles, etapas y flujos."
---

> **Descarga oficial (.docx):**  
> <a href="DG-PRO-PCRD-MINS-001-Proo%20Corporativo%20de%20Remediación%20de%20Datos%20v1.0.docxDG-PRO-PCRD-MINS-001 v1.0</a>

# PROCEDIMIENTO CORPORATIVO DE REMEDIACIÓN DE DATOS
**Programa de Gobierno del Dato**  
**Código:** DG-PRO-PCRD-MINS-001 — **Versión:** 1.0 — **Fecha:** 01/08/2025

## OBJETIVO
Definir actividades, roles y responsabilidades para corregir incidencias de calidad de datos, asegurando cumplimiento de reglas y medidas preventivas.

## ALCANCE
Aplica a datos críticos en SAP, OT/PI, Data Lake, plataformas analíticas y fuentes externas integradas.

## ROLES Y RESPONSABILIDADES (extracto)
- **Analista de Calidad y Seguridad del Dato:** define y monitorea el proceso.  
- **Data Steward:** coordina remediación, valida cumplimiento, actualiza inventario de reglas.  
- **Data Owner:** aprueba acciones correctivas.  
- **Domain Owner:** supervisa remediaciones críticas.  
- **Data Engineer:** corrige errores técnicos en pipelines.  
- **Analista de Diseño del Dato:** modifica reglas en repositorio.  
- **Data User:** participa en validaciones.

## CONCEPTOS CLAVE
- **Remediación de datos:** corrección planificada para restituir calidad.  
- **Estados:** Activo → En proceso → Remediado.  
- **Niveles:**  
  - Nivel 1: técnico (errores en ETL, código).  
  - Nivel 2: negocio (reglas obsoletas, inconsistencias).  
  - Nivel 3: falso positivo.

## ETAPAS DEL PROCEDIMIENTO (extracto)
1. **Detección y registro:** marcar incidencia en Autoservicio Analítico.  
2. **Análisis de causa raíz:** diagnóstico técnico/negocio.  
3. **Ejecución:**  
   - Solución técnica (Data Engineer).  
   - Solución de negocio (Data Owner).  
   - Ajuste de reglas (Data Steward + Analista de Diseño).  
4. **Reprocesamiento:** configurar Metadata Driven y ejecutar pipelines.  
5. **Cierre:** marcar alerta como remediada y registrar en tabla.

## SUBPROCESO: Modificar Validación de Reglas de Calidad
- Decidir tipo de cambio (modificación/eliminación).  
- Actualizar documento y repositorio.  
- Validar en Databricks y cerrar.

## REFERENCIA
- DG-POL-PCGD-MINS-001 — Política de Gobierno de Datos.  
- DG-POL-PCCD-MINS-001 — Política de Calidad de Datos.  
- DG-MAN-INGS-MINS-001 — Procedimiento de Ingesta con Calidad y Seguridad.

## CONTROL DE VERSIONES
| Versión | Fecha       | Responsable   | Cambios          | Aprobado por     |
|---------|------------|--------------|------------------|------------------|
| 1.0     | 01/08/2025 | Jean Cabrera | Versión inicial  | Comité Directivo |

## APROBACIÓN Y VIGENCIA
Aprobado por Comité Directivo; vigente hasta su reemplazo o derogación.
