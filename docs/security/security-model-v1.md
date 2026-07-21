# Security Model v1 de Atlas

## Estado del documento

Modelo de seguridad oficial para preparar Atlas MVP v1. No implementa controles técnicos todavía.

## Objetivo

Definir principios, riesgos, roles conceptuales y controles mínimos antes de iniciar implementación real en Lovable.

## Principios de seguridad

- No almacenar secretos en el repositorio.
- Minimizar datos sensibles.
- Documentar integraciones antes de activarlas.
- Mantener revisión humana en decisiones importantes.
- Separar documentación pública de información privada.

## Roles conceptuales

| Rol | Permisos esperados |
| --- | --- |
| Owner | Administrar proyecto, documentos y decisiones |
| CTO | Revisar arquitectura, readiness y ADRs |
| Contributor | Proponer cambios y tareas |
| Viewer | Consultar documentación y estado |

## Riesgos principales

| Riesgo | Impacto | Mitigación |
| --- | --- | --- |
| Exposición de secretos | Alto | No guardar credenciales, usar variables seguras futuras |
| Decisiones no autorizadas | Medio | Requerir revisión y ADR |
| Cambios destructivos | Medio | Confirmaciones y control de versiones |
| Datos personales innecesarios | Alto | Minimización de datos |
| Integraciones prematuras | Medio | Bloquear integraciones sin ADR |

## Controles mínimos para MVP

- Validar que no existan secretos en documentación.
- Definir si el MVP requiere autenticación.
- Limitar acciones críticas a roles autorizados si hay usuarios.
- Registrar decisiones relevantes antes de cambios de alcance.
- Documentar cualquier integración externa.

## Email y notificaciones

La integración de email debe permanecer conceptual hasta aprobar:

- Proveedor.
- Propósito exacto.
- Datos enviados.
- Preferencias de notificación.
- Reglas de privacidad.

## Checklist antes de implementación

- [ ] Roles confirmados.
- [ ] Política de datos definida.
- [ ] Autenticación decidida.
- [ ] Integraciones aprobadas o descartadas.
- [ ] ADR de seguridad creada.
