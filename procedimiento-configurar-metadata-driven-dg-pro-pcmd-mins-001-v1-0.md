---
title: "Procedimiento para Configurar Metadata Driven — DG-PRO-PCMD-MINS-001 v1.0"
code: DG-PRO-PCMD-MINS-001
version: "1.0"
source_file: "DG-PRO-PCMD-MINS-001-Procedimiento para Configurar Metadata Driven v1.0.docx"
layout: default
description: "Procedimiento para configurar Metadata Driven en ingestas al Datalake, roles, lineamientos y pasos."
---

> **Descarga oficial (.docx):**  
> DG-PRO-PCMD-MINS-001-Procedimiento%20para%20Configurar%20Metadata%20Driven%20v1.0.docxDG-PRO-PCMD-MINS-001 v1.0</a>

# PROCEDIMIENTO PARA CONFIGURAR METADATA DRIVEN
**Programa de Gobierno del Dato**  
**Código:** DG-PRO-PCMD-MINS-001 — **Versión:** 1.0 — **Fecha:** 22/08/2025

## OBJETIVO
Definir el procedimiento para configurar la Metadata Driven en cada iniciativa analítica, estableciendo parámetros para conexión con fuentes y asegurando estandarización.

## ALCANCE
Aplica a todas las ingestas de datos que aterrizan en el Datalake.

## ROLES Y RESPONSABILIDADES (extracto)
- **Gestor Data TI:** solicita llenado del formato de metadata driven.  
- **Analista de Diseño del Dato:** valida formatos, crea carpetas en SharePoint, llena formatos en QAS/PRD, coordina cambios en notebooks.  
- **Data Engineer / Arquitecto del Dato:** llena formatos en DEV, desarrolla procesos de ingesta.  
- **Arquitectura de Soluciones:** aprueba artefactos y cambios en notebooks, ejecuta pipelines.

## CONCEPTOS CLAVE
- **Metadata Driven:** estrategia para definir procesos basados en metadatos (fuentes, parámetros, periodicidad, tipo de carga).  
- **Gobierno del Dato:** políticas y roles que aseguran calidad, seguridad y trazabilidad.

## LINEAMIENTOS
- Toda metadata debe registrarse en plantillas oficiales en SharePoint.  
- Cambios en parámetros deben quedar aprobados y registrados.  
- Procesamiento mediante Azure Data Factory (ADF) Analítica.

## ETAPAS DEL PROCEDIMIENTO (extracto)
1. Enviar artefacto de arquitectura aprobado.  
2. Solicitar llenado de plantillas.  
3. Evaluar si hay nuevas fuentes.  
4. Crear carpetas y plantillas en SharePoint si aplica.  
5. Actualizar programación del notebook en ADF.  
6. Llenar formatos según ambiente (DEV/QAS/PRD).  
7. Ejecutar pipeline y notificar.  
8. Desarrollar proceso de ingesta.

## ESTRUCTURA DE PLANTILLAS
Campos clave: Id, UM, Dominio, Subdominio, SourceType, Type, SourceSettings (host, instance, userName, secretName, etc.), CopySettings, SinkSetting, DataLoadingBehavior, EntityType, DataCatalog.

## REFERENCIA
- DG-POL-PCGD-MINS-001 — Política de Gobierno de Datos.  
- DG-POL-PCAMA-MINS-001 — Política de Arquitectura y Metadata Analítica.

## CONTROL DE VERSIONES
| Versión | Fecha       | Responsable   | Cambios          | Aprobado por     |
|---------|------------|--------------|------------------|------------------|
| 1.0     | 22/08/2025 | Jean Cabrera | Versión inicial  | Comité Directivo |

## APROBACIÓN Y VIGENCIA
Aprobado por Comité Directivo; vigente hasta su reemplazo o derogación.
