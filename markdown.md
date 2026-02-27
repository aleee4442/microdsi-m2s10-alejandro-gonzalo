# M2-S10 · Entregable rápido · ITSM Triage

## Inventario (L1)
Gestionar incidencias P1 (críticas)
Gestionar incidencias P2-P3 (medias/bajas)
Gestionar solicitudes de servicio
Gestionar problemas (análisis causa raíz)
Gestionar cambios estándar
Gestionar cambios normales con CAB
Gestionar accesos y permisos
Gestionar backups y restauraciones
Gestionar monitorización de infraestructura
Gestionar parches de seguridad
Gestionar releases y despliegues
Atender consultas de usuarios en portal
Gestionar documentación de Knowledge Base
Gestionar inventario CMDB
Gestionar certificados SSL y dominios

## Priorización (Impacto/Esfuerzo/Riesgo)
Gestionar incidencias P1 | Impacto:5 | Esfuerzo:3 | Riesgo:4 | Score:-2 | Nota: 200 tickets/mes, críticos para operación, riesgo alto por PII en descripciones, 30% requieren escalado urgente
Gestionar accesos y permisos | Impacto:4 | Esfuerzo:2 | Riesgo:5 | Score:-3 | Nota: 150 solicitudes/mes, riesgo alto por seguridad y auditoría SOX, requiere doble validación
Gestionar problemas | Impacto:4 | Esfuerzo:4 | Riesgo:2 | Score:-2 | Nota: 45 problemas/mes, el 30% de tickets son recurrentes, ahorro estimado 120h/mes si se resuelven causas raíz
Gestionar cambios con CAB | Impacto:3 | Esfuerzo:4 | Riesgo:4 | Score:-5 | Nota: 25 cambios/mes, riesgo alto por impacto en producción, requiere reunión semanal CAB
Gestionar solicitudes de servicio | Impacto:3 | Esfuerzo:2 | Riesgo:2 | Score:-1 | Nota: 400 solicitudes/mes, proceso maduro con plantillas, bajo riesgo, 80% se resuelven en <2h

## SIPOC
Suppliers: Usuarios finales, Monitoring Tools (Zabbix/Dynatrace), Service Desk L1, Ticketing Tool, Equipo de Seguridad
Inputs: Ticket con descripción, logs de error, capturas de pantalla, alerta automática, PII (nombre, email, IP, datos de contacto)
Process:
1) Recepción y validación automática del ticket (campos obligatorios)
2) Clasificación de severidad (P1-P4) y prioridad según impacto/urgencia
3) Enriquecimiento con datos de CMDB (activos afectados)
4) Diagnóstico inicial con búsqueda en Knowledge Base (KB)
5) Asignación a grupo funcional (Redes, Sistemas, BD, etc.) si no se resuelve en L1
6) Resolución documentada o escalado con trazabilidad completa
7) Cierre con encuesta CSAT y actualización de KB si aplica
Outputs: Incidente resuelto, ticket cerrado con trazabilidad, KB actualizada, métricas (MTTR, FCR, SAT), datos para análisis de tendencias
Customers: Usuario final, Service Owner, Gestor de incidencias, Equipo de mejora continua, Auditores

## Nota (trade-off)
_(2 criterios numéricos + 1 restricción)_
