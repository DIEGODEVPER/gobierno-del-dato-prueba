---
title: "Procedimiento para Transferencia de Propiedad en Unity Catalog — DG-PPRO-TPUC v1.0"
code_from_filename: DG-PPRO-TPUC
code_in_content: DG-PRO-TPTUC-MINS-001
version: "1.0"
source_file: "DG-PPRO-TPUC-Procedimiento para Transferencia de Propiedad en Unity Catalog v1.0.docx"
layout: default
description: "Procedimiento para transferir propiedad de tablas a un Service Principal en Unity Catalog (DEV, QAS, PRD)."
---

> **Descarga oficial (.docx):**  
> <a href="DG-PPRO-edimiento%20para%20Transferencia%20de%20Propiedad%20en%20Unity%20Catalog%20v1.0.docxDG-PPRO-TPUC v1.0</a>

# PROCEDIMIENTO PARA TRANSFERENCIA DE PROPIEDAD EN UNITY CATALOG
**Programa de Gobierno del Dato**  
**Código (en contenido):** **DG-PRO-TPTUC-MINS-001** — **Versión:** **1.0** — **Fecha:** 22/08/2025

> **Nota:** El código en el documento no coincide con el del nombre del archivo. Validar si el código oficial es `DG-PPRO-TPUC` o `DG-PRO-TPTUC-MINS-001`.

## OBJETIVO
Establecer las actividades necesarias para transferir la **propiedad de tablas** en Unity Catalog a un **Service Principal**, garantizando seguridad, control de accesos y cumplimiento de políticas de Gobierno del Dato.

## ALCANCE
Aplica a **todas las tablas** creadas en los ambientes **DEV, QAS y PRD** dentro de Unity Catalog, desde la creación y enlace del Service Principal hasta su asignación como **propietario** de las tablas.

## ROLES Y RESPONSABILIDADES (extracto)
- **Gestor Data TI:** solicita la creación del **Service Principal** (una sola vez).  
- **Administrador de Nube:** crea el **Service Principal** y lo enlaza como **usuario externo** en Databricks.  
- **Analista de Diseño del Dato:** otorga permisos y **modifica la propiedad** de tablas para asignarla al Service Principal.

## CONCEPTOS CLAVE
- **Unity Catalog:** gobierno centralizado de catálogos, esquemas y tablas.  
- **Service Principal:** identidad de aplicación usada para propiedad y automatizaciones.  
- **Matriz de Accesos:** documento que consolida roles, permisos y objetos.  
- **Metadata Driven:** procesos basados en metadatos para estandarizar accesos/ingestas.

## ETAPAS DEL PROCEDIMIENTO (resumen)
1. **Solicitud** de creación de Service Principal (Gestor Data TI).  
2. **Creación y enlace** del Service Principal como usuario externo en Databricks (Administrador de Nube).  
3. **Listado** de tablas del catálogo del proyecto (Gestor Data TI).  
4. **Concesión de permisos** al Service Principal (SELECT/MODIFY) para DEV, QAS y PRD (Analista de Diseño).  
5. **Cambio de propietario** de cada tabla a favor del Service Principal en DEV, QAS y PRD (Analista de Diseño).

## REFERENCIAS
- DG‑POL‑PCGD‑MINS‑001 — Política de Gobierno de Datos.  
- DG‑POL‑PCAMA‑MINS‑001 — Política de Arquitectura y Metadata Analítica.

## CONTROL DE VERSIONES
| Versión | Fecha       | Responsable   | Cambios          | Aprobado por     |
|---------|------------|--------------|------------------|------------------|
| 1.0     | 22/08/2025 | Jean Cabrera | Versión inicial  | Comité Directivo |

## APROBACIÓN Y VIGENCIA
Aprobado por Comité Directivo. Vigente desde su aprobación hasta su reemplazo o derogación.
