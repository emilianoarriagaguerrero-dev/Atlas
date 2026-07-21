# ADR-001 — Arquitectura Atlas MVP v1 para Lovable

## Estado

Status: Approved
Approved by: CEO / CTO
Approval date: 2026-07-21

## Fecha

2026-07-21

## Contexto

Atlas ya cuenta con documentación oficial de producto, AIOS, diseño, arquitectura, base de datos, seguridad, roadmap y preparación Lovable. Antes de iniciar construcción del MVP v1, se requiere una decisión formal que apruebe la arquitectura objetivo y confirme que no se agregará código sin autorización explícita.

## Decisión propuesta

Aprobar Atlas MVP v1 como una aplicación modular orientada a documentación, estado del proyecto y trazabilidad, preparada para construirse en Lovable con los siguientes módulos:

- Dashboard.
- Documentos.
- Decisiones.
- Backlog.
- Roadmap.
- Readiness.
- Recursos.

## Documentos base obligatorios

La implementación deberá respetar:

- Product Bible.
- PRD oficial.
- MVP Definition v1.
- AIOS Bible.
- AIOS Technical Specification.
- System Architecture.
- Database Schema v1.
- Security Model v1.
- UX Specification.
- Design System.
- Lovable Master Spec.
- Lovable Build Prompt v1.

## Arquitectura aprobada

La arquitectura se basará en dominios separados:

| Dominio | Responsabilidad |
| --- | --- |
| Producto | Visión, requisitos, PRD y roadmap |
| AIOS | Contexto, decisiones, backlog y readiness |
| Diseño | Experiencia, tono y consistencia visual |
| Seguridad | Roles, riesgos y controles mínimos |
| Datos | Entidades conceptuales y relaciones |
| Operación | Gobernanza, Definition of Done y checklist |

## Restricciones

- No agregar integraciones externas sin ADR adicional.
- No almacenar secretos ni credenciales.
- No implementar email real en MVP v1.
- No agregar automatizaciones con IA en MVP v1.
- No cambiar el alcance sin actualizar PRD, roadmap y backlog.

## Consecuencias

Si se aprueba esta ADR:

- Atlas podrá avanzar a preparación de construcción en Lovable.
- Lovable Build Prompt v1 podrá usarse como guía de implementación.
- Cualquier desviación requerirá nueva decisión documentada.

Si no se aprueba:

- Atlas permanecerá en etapa documental.
- Se deberán resolver los bloqueos antes de construir.

## Criterios de aprobación

- [ ] Product Bible aprobada.
- [ ] PRD oficial aprobado.
- [ ] UX Specification aprobada.
- [ ] Database Schema v1 aprobado.
- [ ] Security Model v1 aprobado.
- [ ] Lovable Build Prompt v1 aprobado.
- [ ] Responsable del proyecto autoriza iniciar Lovable.
- [ ] CTO o líder técnico valida arquitectura MVP v1.
