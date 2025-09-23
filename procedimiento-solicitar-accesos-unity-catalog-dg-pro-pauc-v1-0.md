---
title: "Procedimiento para Solicitar Accesos a Unity Catalog — DG-PRO-PAUC v1.0"
code: DG-PRO-PAUC
version: "1.0"
source_file: "DG-PRO-PAUC-Procedimiento para Solicitar Accesos a Unity Catalog v1.0.docx"
layout: default
description: "Procedimiento para gestionar solicitudes de acceso a Unity Catalog en proyectos analíticos."
---

> **Descarga oficial (.docx):**  
> <a href="DG-PRO-PAUC-Proced0para%20Solicitar%20Accesos%20a%20Unity%20Catalog%20v1.0.docxDG-PRO-PAUC v1.0</a>

# PROCEDIMIENTO PARA SOLICITAR ACCESOS A UNITY CATALOG
**Programa de Gobierno del Dato**  
**Código:** DG-PRO-PAUC — **Versión:** 1.0 — **Fecha:** 22/08/2025

## OBJETIVO
Definir el flujo para solicitar, evaluar, aprobar y configurar accesos en Unity Catalog, asegurando control y trazabilidad.

## ALCANCE
Aplica a proyectos de Analítica Avanzada que requieran habilitar accesos en Unity Catalog.  
**Excepción:** no aplica a Storage Account ni al catálogo de experimentación.

## ROLES Y RESPONSABILIDADES (extracto)
- **Solicitante:** envía formulario con datos (usuario, rol, objetos, ambiente, fechas, conformidad del Data Owner).  
- **Analista de Diseño del Dato:** valida solicitud, asigna permisos en Unity Catalog.  
- **Seguridad de la Información:** aprueba accesos.  
- **Gobierno del Dato:** recepciona y deriva solicitudes.  
- **Consumidor de dato:** valida accesos concedidos.

## CONCEPTOS CLAVE
- **Unity Catalog:** componente de Databricks para gobierno centralizado.  
- **Matriz de Accesos:** documento con roles, permisos y objetos.

## ETAPAS DEL PROCEDIMIENTO (extracto)
1. Enviar solicitud con formulario completo.  
2. Gobierno del Dato deriva al Analista de Diseño.  
3. Validación de solicitud.  
4. Observación o aprobación → envío a Seguridad.  
5. Autorización por Seguridad.  
6. Asignación de permisos en Unity Catalog (ejemplo: `GRANT SELECT ON TABLE ...`).  
7. Notificación al solicitante.  
8. Validación de accesos (Power BI para Business Data Users).

## CONSIDERACIONES DE SEGURIDAD
- Revisar accesos trimestralmente.  
- Revocar accesos cuando un usuario cambia de rol o sale de la compañía.

## REFERENCIA
- DG-POL-PCGD-MINS-001 — Política de Gobierno de Datos.  
- DG-POL-PCAMA-MINS-001 — Política de Arquitectura y Metadata Analítica.

## CONTROL DE VERSIONES
| Versión | Fecha       | Responsable   | Cambios          | Aprobado por     |
|---------|------------|--------------|------------------|------------------|
| 1.0     | 22/08/2025 | Jean Cabrera | Versión inicial  | Comité Directivo |

## APROBACIÓN Y VIGENCIA
Aprobado por Comité Directivo; vigente hasta su reemplazo o derogación.
