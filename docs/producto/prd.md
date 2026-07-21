# PRD oficial de Atlas

## Estado del documento

Este PRD forma parte de la especificación oficial de Atlas y prepara el proyecto para una futura implementación en Lovable. No define código ni stack final; documenta producto, alcance, requisitos y criterios de aceptación.

## Resumen ejecutivo

Atlas es una plataforma documental y operativa que convierte ideas, conversaciones y decisiones en una especificación clara, trazable y lista para ejecución. Su primera etapa vive en GitHub como fuente de verdad y su implementación futura podrá construirse en Lovable cuando el alcance funcional sea aprobado.

## Objetivo del producto

Permitir que una persona o equipo organice el estado completo de un proyecto: visión, decisiones, tareas, recursos, arquitectura, diseño y próximos pasos.

## Usuarios objetivo

### Usuario primario

Responsable del proyecto que necesita convertir ideas en una especificación ordenada.

### Usuarios secundarios

- CTO o líder técnico que revisa arquitectura y readiness.
- Colaboradores de producto o diseño.
- Futuros desarrolladores que recibirán la especificación para implementar.
- Stakeholders que necesitan entender estado, alcance y decisiones.

## Problema

La información crítica de un proyecto suele quedar dispersa entre conversaciones, notas y decisiones informales. Esto dificulta saber qué está aprobado, qué falta, qué puede implementarse y qué debe esperar.

## Propuesta de valor

Atlas crea una fuente única de verdad para que el proyecto avance con claridad antes de construir software.

## Alcance funcional futuro para Lovable

Cuando Atlas pase a implementación, la primera versión debería contemplar:

1. Dashboard de estado del proyecto.
2. Vista de documentación oficial.
3. Registro de decisiones.
4. Backlog priorizado.
5. Roadmap por etapas.
6. Vista de recursos.
7. Panel de criterios de readiness.
8. Sección de diseño y arquitectura.

## Requisitos funcionales

| ID | Requisito | Prioridad |
| --- | --- | --- |
| PRD-001 | Mostrar estado general del proyecto | Alta |
| PRD-002 | Listar documentos oficiales por área | Alta |
| PRD-003 | Registrar y consultar decisiones | Alta |
| PRD-004 | Mantener backlog priorizado | Alta |
| PRD-005 | Mostrar roadmap por etapas | Media |
| PRD-006 | Consultar criterios de implementación | Media |
| PRD-007 | Centralizar recursos y enlaces | Media |
| PRD-008 | Preparar handoff para implementación futura | Media |

## Requisitos no funcionales

- La experiencia debe ser clara y sobria.
- El contenido debe organizarse por dominios.
- El sistema debe evitar acciones confusas o destructivas.
- La navegación debe priorizar estado, documentos y próximos pasos.
- La implementación futura debe respetar Product Bible, AIOS Bible y Design System.

## Fuera de alcance actual

- Generar código en esta etapa.
- Definir base de datos física final.
- Integrar servicios externos.
- Crear autenticación real.
- Automatizar flujos con IA.

## Criterios de aceptación para pasar a Lovable

- Product Bible, AIOS Bible y Design System están completos.
- UX Specification está documentada.
- System Architecture está documentada.
- Database Design conceptual está documentado.
- Roadmap y backlog están alineados.
- Existe decisión aprobada para iniciar implementación.
