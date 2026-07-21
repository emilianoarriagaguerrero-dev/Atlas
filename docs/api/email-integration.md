# Email Integration Specification de Atlas

## Estado del documento

Documento oficial de especificación conceptual para una futura integración de correo. No implementa API, credenciales ni código.

## Propósito

Preparar una posible integración de email para notificaciones, invitaciones o resúmenes del proyecto Atlas cuando exista una implementación real.

## Casos de uso futuros

- Enviar resumen de estado del proyecto.
- Notificar nuevas decisiones aprobadas.
- Avisar cambios de etapa en roadmap.
- Enviar invitaciones a colaboradores.
- Recordar criterios de readiness pendientes.

## Eventos potenciales

| Evento | Descripción | Prioridad |
| --- | --- | --- |
| project.summary.ready | Resumen periódico disponible | Media |
| decision.approved | Nueva decisión aprobada | Alta |
| backlog.item.assigned | Tarea asignada a colaborador | Media |
| roadmap.stage.changed | Cambio de etapa en roadmap | Media |
| readiness.blocked | Implementación bloqueada por criterio pendiente | Alta |

## Datos mínimos de email

- recipient_email
- subject
- template_type
- project_id
- event_type
- created_at
- delivery_status

## Reglas de seguridad

- No guardar credenciales en el repositorio.
- No enviar información sensible sin aprobación.
- Permitir desactivar notificaciones futuras.
- Registrar proveedor de email mediante ADR antes de implementar.
- Cumplir requisitos de privacidad antes de activar envíos reales.

## Plantillas futuras sugeridas

- Resumen de proyecto.
- Decisión aprobada.
- Tarea pendiente.
- Readiness bloqueado.
- Invitación a colaborar.

## Fuera de alcance actual

- Seleccionar proveedor de email.
- Crear endpoints.
- Crear templates HTML.
- Enviar correos reales.
- Gestionar bajas o preferencias.
