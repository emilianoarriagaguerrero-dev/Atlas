# Database Design conceptual de Atlas

## Estado del documento

Este documento define un modelo conceptual de datos para una futura implementación de Atlas en Lovable. No crea base de datos, migraciones ni código.

## Objetivo

Identificar las entidades principales que Atlas podría necesitar si evoluciona de documentación estática a producto implementado.

## Entidades conceptuales

### Project

Representa el proyecto Atlas o un proyecto gestionado dentro de Atlas.

Campos conceptuales:

- id
- name
- description
- status
- current_stage
- created_at
- updated_at

### Document

Representa documentos oficiales como Product Bible, AIOS Bible, PRD o Design System.

Campos conceptuales:

- id
- project_id
- title
- domain
- status
- version
- content_reference
- updated_at

### Decision

Representa decisiones generales o arquitectónicas.

Campos conceptuales:

- id
- project_id
- title
- date
- status
- context
- decision
- consequences

### BacklogItem

Representa tareas, ideas o pendientes.

Campos conceptuales:

- id
- project_id
- title
- description
- priority
- status
- related_document_id

### RoadmapStage

Representa etapas del roadmap.

Campos conceptuales:

- id
- project_id
- name
- status
- description
- order

### ReadinessCriterion

Representa criterios necesarios antes de implementar.

Campos conceptuales:

- id
- project_id
- title
- status
- domain
- evidence_reference

### Resource

Representa enlaces, referencias o materiales de apoyo.

Campos conceptuales:

- id
- project_id
- title
- type
- url_or_reference
- notes

## Relaciones conceptuales

```text
Project 1---N Document
Project 1---N Decision
Project 1---N BacklogItem
Project 1---N RoadmapStage
Project 1---N ReadinessCriterion
Project 1---N Resource
Document 1---N BacklogItem
Document 1---N ReadinessCriterion
Decision 1---N BacklogItem
```

## Reglas de datos

- Todo documento debe pertenecer a un proyecto.
- Toda decisión debe tener estado.
- Todo criterio de readiness debe estar asociado a un dominio.
- Un backlog item puede relacionarse con un documento o decisión.
- No se deben almacenar secretos ni credenciales.

## Fuera de alcance actual

- Definir motor de base de datos.
- Crear tablas reales.
- Crear migraciones.
- Crear modelos en código.
- Definir autenticación o permisos finales.
