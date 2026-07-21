# Lovable Master Spec de Atlas

## Estado del documento

Documento maestro para preparar una futura implementación real de Atlas en Lovable. No contiene código ni instrucciones de generación automática todavía.

## Objetivo

Traducir la documentación oficial de Atlas en una especificación clara que pueda usarse como base para construir el MVP en Lovable cuando la implementación sea aprobada.

## Fuente de verdad

La implementación futura debe respetar estos documentos:

- Product Bible.
- AIOS Bible.
- AIOS Technical Specification.
- PRD oficial.
- UX Specification.
- Design System.
- System Architecture.
- Database Design.
- Roadmap MVP Execution Plan.

## MVP esperado en Lovable

El MVP debe priorizar:

1. Dashboard de estado del proyecto.
2. Biblioteca documental por dominios.
3. Registro de decisiones.
4. Backlog priorizado.
5. Roadmap por etapas.
6. Readiness checklist.
7. Recursos y enlaces.

## Reglas para Lovable

- No inventar funcionalidades fuera del PRD.
- No crear integraciones sin ADR aprobada.
- No manejar secretos en frontend.
- Mantener tono visual sobrio y claro.
- Seguir Design System y UX Specification.
- Mantener estructura modular por dominios.

## Navegación propuesta

```text
Dashboard
Documentos
Decisiones
Backlog
Roadmap
Readiness
Recursos
Configuración futura
```

## Datos conceptuales a representar

- Project
- Document
- Decision
- BacklogItem
- RoadmapStage
- ReadinessCriterion
- Resource

## Criterios de aceptación del MVP

- El usuario entiende el estado del proyecto en la primera pantalla.
- Los documentos oficiales son navegables por dominio.
- Las decisiones muestran contexto, estado e impacto.
- El backlog permite distinguir prioridad y estado.
- El roadmap muestra etapa actual y etapas futuras.
- Readiness deja claro qué bloquea implementación.
- La UI respeta el Design System.

## Bloqueos antes de construir

- Falta aprobar alcance funcional definitivo.
- Falta decidir stack/configuración final en Lovable.
- Falta confirmar si habrá autenticación.
- Falta aprobar modelo de datos final.
- Falta ADR de inicio de implementación.
