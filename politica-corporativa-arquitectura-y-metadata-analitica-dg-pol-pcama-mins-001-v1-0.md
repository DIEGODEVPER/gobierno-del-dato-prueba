---
title: "Política Corporativa de Arquitectura y Metadata Analítica — DG-POL-PCAMA-MINS-001 v1.0"
code: DG-POL-PCAMA-MINS-001
version: "1.0"
source_file: "DG-POL-PCAMA-MINS-001-Política Corporativo de Arquitectura y Metadata Analítica (Datalake, Deltalake, UnityCatalog, Metadata driven) v1.0.docx"
layout: default
description: "Lineamientos de arquitectura analítica (Data Lake, Delta Lake, Unity Catalog) y enfoque metadata-driven en MINSUR."
---

> **Descarga oficial (.docx):**  
> DG-POL-PCAMA-MINS-001-Política%20Corporativo%20de%20Arquitectura%20y%20Metadata%20Analítica%20(Datalake,%20Deltalake,%20UnityCatalog,%20Metadata%20driven)%20v1.0.docxDG-POL-PCAMA-MINS-001 v1.0</a>

# POLÍTICA CORPORATIVA DE ARQUITECTURA Y METADATA ANALÍTICA
**(Data Lake, Delta Lake, Unity Catalog, Metadata‑Driven)**  
**Programa de Gobierno del Dato**  
**Código:** **DG-POL-PCAMA-MINS-001** — **Versión:** **1.0** — **Fecha:** 22/08/2025
## CONTENIDO
1. **Introducción**  
2. **Objetivo**  
3. **Alcance**  
4. **Glosario de Términos**  
5. **Principios Fundamentales**  
6. **Componentes de la Arquitectura Analítica**  
7. **Lineamientos Datalake** (Esquema Medallón)  
8. **Lineamientos de Unity Catalog**  
9. **Lineamientos de Metadata**  
10. **Ciclo de Vida**  
11. **Monitoreo**  
12. **Referencia**  
13. **Control de Versiones**  
14. **Aprobación**  
15. **Vigencia**

## INTRODUCCIÓN
Lineamientos para implementar y gestionar la **arquitectura analítica corporativa** basada en **Data Lake**, **Delta Lake**, **Unity Catalog** y el enfoque **metadata‑driven**, asegurando calidad, interoperabilidad, gobierno y soporte a analítica avanzada/IA.

## OBJETIVO
Definir los lineamientos corporativos para el **diseño, gestión y control** de la arquitectura analítica y del **uso de metadatos**, garantizando información confiable, segura, trazable y explotable bajo un modelo **metadata‑driven**.

## ALCANCE
- Fuentes integradas al Data Lake (SAP, operativos, IoT, geológicos, ambientales, financieros, etc.).  
- Plataformas (Databricks, Delta Lake, Unity Catalog, repositorios de metadatos).  
- Áreas de negocio y roles de datos (analistas, científicos, ingenieros, arquitectos, usuarios).

## GLOSARIO (extracto)
- **Unity Catalog:** servicio de gobierno/catalogación en Lakehouse.  
- **Delta Lake:** almacenamiento transaccional con control de versiones.  
- **Data Lake:** almacén masivo de datos estructurados/no estructurados.  
- **Arquitectura Medallón:** capas **Bronce, Plata, Oro**.  
- **Metadatos:** datos que describen a otros datos (origen, formato, reglas, uso).

## PRINCIPIOS (extracto)
- **Escalabilidad y flexibilidad**.  
- **Metadata‑driven** en cargas, transformaciones y calidad.  
- **Interoperabilidad** entre SAP, aplicaciones y nube.  
- **Trazabilidad y linaje** end‑to‑end.  
- **Seguridad y cumplimiento** (accesos por roles, auditoría).  
- **Estandarización y reutilización**.

## COMPONENTES (extracto)
- **Data Lake Corporativo**, **Delta Lake**, **Unity Catalog**, **Metadata‑Driven Framework**.

## LINEAMIENTOS DATALAKE — ESQUEMA MEDALLÓN
**Capa Bronce:** datos crudos; conversión/unificación de formatos.  
**Capa Plata:** limpieza, **reglas de calidad**, remediación.  
**Capa Oro:** datos enriquecidos listos para consumo.  
**Capa Auditoría (transversal):** métricas de calidad y controles de acceso/seguridad.

**Organización (extracto):**
- Jerarquía por capas (ingesta → procesamiento → entrega).  
- **Nomenclatura consistente** y **versionado** (Delta time travel).  
- **Registro de metadatos** por dataset (descripción, propietarios, etiquetas).

**Cargas Full/Incrementales (extracto):**
- **Full:** registrar commit/versión en Delta; respaldo previo en Bronce; reglas en Plata.  
- **Incremental:** campos de control; **MERGE** en Delta; punto de corte **metadata‑driven**; área de remediación.

## LINEAMIENTOS DEL DELTA LAKE (extracto)
- **Estándar único** de procesamiento analítico.  
- **Control de versiones** (time travel) y atomicidad.  
- Organización **Bronce/Plata/Oro** con controles por capa.  
- **Validaciones automáticas** y linaje integrado con Unity Catalog.  
- **Interoperabilidad** con SAP/apps externas.

## LINEAMIENTOS DE UNITY CATALOG (extracto)
- **Catálogo centralizado**: único repositorio de objetos (catálogos, esquemas, tablas, vistas, volúmenes, funciones, modelos).  
- **Accesos por roles** (mínimo privilegio; por ambiente/objeto).  
- **Convención Catálogo‑Esquema‑Tabla** (ejemplos en el documento).  
- **Trazabilidad y linaje** centralizados.  
- **Clasificación/sensibilidad** condiciona accesos y controles.  
- **Roles y permisos** (matriz de responsabilidades).

## LINEAMIENTOS DE METADATA (extracto)
- **Técnicos:** estructura, tipos, validaciones, relaciones, versionado, origen.  
- **Negocio:** definiciones, reglas de calidad, responsables, criticidad/sensibilidad.  
- **Operacionales:** ejecución de pipelines, frecuencia, indicadores de calidad.  
- **Gobierno activo:** actualización y auditoría continua; gestión de cambios.  
- **Uso metadata‑driven:** cargas/transformaciones/publicaciones parametrizadas por metadatos.

## CICLO DE VIDA (extracto)
**Ingesta → Transformación → Consumo → Retención/Depuración** (con reglas documentadas y linaje).

## MONITOREO (extracto)
Métricas de calidad/uso/rendimiento; auditorías; alertas ante fallos de reglas o metadatos.

## REFERENCIA
- DG‑POL‑PCGD‑MINS‑001 — Política de Gobierno de Datos.  
- DG‑POL‑PCCD‑MINS‑001 — Política de Calidad de Datos.  
- DG‑MAN‑INGS‑MINS‑001 — Procedimiento de Ingesta con Calidad y Seguridad de Datos.  
- DG‑PRO‑PCCD‑MINS‑001 — Procedimiento Corporativo de Calidad de Datos.

## CONTROL DE VERSIONES
<table>
<tr><th>Versión</th><th>Fecha</th><th>Responsable</th><th>Cambios</th><th>Aprobado por</th></tr>
<tr><td>1.0</td><td>22/08/2025</td><td>Jean Cabrera</td><td>Versión inicial</td><td>Comité Directivo</td></tr>
</table>

## APROBACIÓN Y VIGENCIA
Aprobado por el Comité Directivo. Vigente desde su aprobación hasta su reemplazo o derogación.
