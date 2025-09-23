---
title: "Política Corporativa de Calidad del Dato — DG-POL-PCCD-MINS-001 v2.0 (archivo)"
code: DG-POL-PCCD-MINS-001
version_from_filename: "2.0"
version_in_content: "1.0"
source_file: "DG-POL-PCCD-MINS-001-Política Corporativo de Calidad de Datos v2.0.docx"
layout: default
description: "Dimensiones y reglas de calidad de datos en MINSUR; responsabilidades, monitoreo y remediación."
---

> **Descarga oficial (.docx):**  
> DG-POL-PCCD-MINS-001-Política%20Corporativo%20de%20Calidad%20de%20Datos%20v2.0.docxDG-POL-PCCD-MINS-001 v2.0 (archivo)</a>  
> **Nota:** En el contenido figura **Versión: 1.0**. Verificar consistencia de versión.

# POLÍTICA CORPORATIVA DE CALIDAD DEL DATO
**Programa de Gobierno del Dato**  
**Código:** **DG-POL-PCCD-MINS-001** — **Versión (contenido):** **1.0** — **Fecha:** 11/08/2025

## CONTENIDO
1. **Introducción**  
2. **Objetivo**  
3. **Alcance**  
4. **Principios Fundamentales de Calidad**  
5. **Responsabilidades**  
6. **Estándares de Calidad**  
7. **Proceso de Remediación de Datos**  
8. **Cumplimiento**  
9. **Referencia**  
10. **Control de Versiones**  
11. **Aprobación**  
12. **Vigencia**

## INTRODUCCIÓN
Lineamientos para la **gestión y gobierno de la calidad de datos** en el ecosistema corporativo: aplica tanto a **proyectos analíticos** como a procesos de **remediación** independientes.

## OBJETIVO
Asegurar **integridad, precisión, completitud, consistencia, disponibilidad y confiabilidad** a lo largo del ciclo de vida de los datos para favorecer la decisión, el cumplimiento normativo y la eficiencia operativa.

## ALCANCE
- Datos críticos del negocio (operativos, ambientales, geológicos, financieros, sociales, personales, regulatorios).  
- Procesos del ciclo minero (exploración → cierre).  
- Sistemas de información (SAP, PI, analítica, data lakes, hojas de cálculo).  
- Personal interno/externo que crea, modifica, consulta o administra datos.

## PRINCIPIOS FUNDAMENTALES (extracto)
- **Precisión** — representar la realidad.  
- **Completitud** — campos obligatorios informados.  
- **Consistencia** — coherencia entre sistemas/reportes.  
- **Trazabilidad** — acciones auditables.  
- **Oportunidad** — disponibles a tiempo.  
- **Validez** — reglas/dominios/formatos.  
- **Protección** — resguardos ante pérdida/acceso indebido.

## RESPONSABILIDADES (extracto)
- **Dueño del Dominio:** prioridades, clasificación, aprobación de estándares; valida criticidad de incidentes.  
- **Dueño del Dato:** define reglas/tolerancias; acepta/rechaza datos; aprueba remediación.  
- **Data Steward:** ejecuta controles; documenta hallazgos; gestiona remediación; mantiene inventario de reglas.  
- **Analista de Calidad y Seguridad del Dato:** define el modelo de calidad; monitorea reglas; valida efectividad.  
- **Analista de Diseño del Dato:** estandariza estructura; implementa estándares en diseño.  
- **Data Engineer:** diagnostica y corrige errores técnicos de pipelines/código.  
- **Data User:** usa datos conforme a estándares; reporta inconsistencias.

## ESTÁNDARES DE CALIDAD
### Dimensiones (extracto)
<table>
<tr><th>N°</th><th>Dimensión</th><th>Definición</th><th>Ejemplo</th></tr>
<tr><td>1</td><td>Precisión</td><td>Exactitud respecto a la realidad</td><td>Ley mineral = laboratorio</td></tr>
<tr><td>2</td><td>Completitud</td><td>Campos obligatorios informados</td><td>Mantenimiento: fecha/equipo/tipo/técnico</td></tr>
<tr><td>3</td><td>Consistencia</td><td>Sin contradicciones entre sistemas</td><td>Tn producida OT = SAP</td></tr>
<tr><td>4</td><td>Validez</td><td>Formatos/dominios correctos</td><td>Fecha YYYY‑MM‑DD</td></tr>
<tr><td>5</td><td>Integridad</td><td>Relaciones completas</td><td>OT con equipo y ubicación válidos</td></tr>
<tr><td>6</td><td>Trazabilidad</td><td>Origen y cambios identificables</td><td>Usuario y fecha de movimiento</td></tr>
<tr><td>7</td><td>Oportunidad</td><td>Disponibles a tiempo</td><td>Reporte ambiental dentro del plazo</td></tr>
<tr><td>8</td><td>Unicidad</td><td>Sin duplicidades</td><td>Proveedor único por RUC</td></tr>
</table>

### Reglas (extracto)
- **No nulos** en claves.  
- **Registros completos** (campos obligatorios).  
- **Formato de fechas** válido.  
- **Rangos numéricos** de negocio.  
- **Patrones de identificadores** (RUC, email).  
- **Consistencia de valores** (listas permitidas).  
- **Precisión decimal** (dígitos/decimales).

## MONITOREO (extracto)
- Dashboards por dominio/sistema/regla.  
- Alertas de calidad; reportes periódicos; auditorías.  
- Roles: Data Steward, Data Owner, Comité de Gobierno del Dato.

## PROCESO DE REMEDIACIÓN
**Identificación → Análisis de causa raíz → Corrección → Validación → Registro** (fecha, responsable, causa, acción).

## CUMPLIMIENTO (extracto)
Obligatorio para todas las áreas y terceros; **Auditoría Interna** y **Seguridad de la Información** supervisan evidencias y controles.

## REFERENCIA
- DG‑POL‑PCGD‑MINS‑001 — Política de Gobierno de Datos.  
- DG‑MAN‑INGS‑MINS‑001 — Procedimiento de Ingesta con Calidad y Seguridad de Datos.

## CONTROL DE VERSIONES
<table>
<tr><th>Versión</th><th>Fecha</th><th>Responsable</th><th>Cambios</th><th>Aprobado por</th></tr>
<tr><td>1.0</td><td>05/08/2025</td><td>Jean Cabrera</td><td>Versión inicial</td><td>Comité Directivo</td></tr>
</table>

## VIGENCIA Y APROBACIÓN
Vigente desde su aprobación formal hasta su reemplazo o derogación; aprobado por responsables indicados.
