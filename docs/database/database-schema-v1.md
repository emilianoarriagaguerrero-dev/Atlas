# Database Schema v1 de Atlas

## Estado del documento

Especificación oficial del esquema conceptual v1 para Atlas MVP. No crea tablas reales, migraciones ni código.

## Objetivo

Definir las entidades, campos y relaciones mínimas para que Atlas MVP v1 pueda implementarse de forma consistente en Lovable cuando sea aprobado.

## Entidades v1

### projects

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| name | text | Nombre del proyecto |
| description | text | Descripción corta |
| status | enum | planning, ready, blocked, active |
| current_stage | text | Etapa actual del roadmap |
| created_at | datetime | Fecha de creación |
| updated_at | datetime | Última actualización |

### documents

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| project_id | uuid | Relación con projects |
| title | text | Título del documento |
| domain | enum | product, architecture, design, operation, security, roadmap, api |
| status | enum | draft, official, deprecated |
| version | text | Versión del documento |
| path | text | Ruta o referencia documental |
| summary | text | Resumen breve |
| updated_at | datetime | Última actualización |

### decisions

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| project_id | uuid | Relación con projects |
| title | text | Título de la decisión |
| decision_type | enum | product, architecture, operation, security |
| status | enum | proposed, accepted, rejected, superseded |
| context | text | Contexto |
| decision | text | Decisión tomada |
| consequences | text | Consecuencias |
| decided_at | date | Fecha de decisión |

### backlog_items

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| project_id | uuid | Relación con projects |
| title | text | Título de la tarea |
| description | text | Detalle |
| priority | enum | high, medium, low |
| status | enum | todo, in_progress, done, blocked |
| related_document_id | uuid | Opcional |
| related_decision_id | uuid | Opcional |

### roadmap_stages

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| project_id | uuid | Relación con projects |
| name | text | Nombre de etapa |
| description | text | Descripción |
| status | enum | complete, pending, blocked, active |
| sort_order | number | Orden visual |

### readiness_criteria

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| project_id | uuid | Relación con projects |
| title | text | Criterio |
| domain | enum | product, architecture, design, security, operation |
| status | enum | pending, complete, blocked |
| evidence_reference | text | Documento o decisión que respalda el estado |

### resources

| Campo | Tipo conceptual | Notas |
| --- | --- | --- |
| id | uuid | Identificador único |
| project_id | uuid | Relación con projects |
| title | text | Nombre del recurso |
| resource_type | enum | link, document, note, asset |
| reference | text | URL o ruta |
| notes | text | Comentarios |

## Relaciones v1

```text
projects 1---N documents
projects 1---N decisions
projects 1---N backlog_items
projects 1---N roadmap_stages
projects 1---N readiness_criteria
projects 1---N resources
documents 1---N backlog_items
decisions 1---N backlog_items
documents 1---N readiness_criteria
```

## Reglas de integridad

- Toda entidad principal pertenece a un proyecto.
- Todo documento tiene dominio y estado.
- Toda decisión tiene contexto, decisión y consecuencias.
- Todo backlog item tiene prioridad y estado.
- Todo readiness criterion pertenece a un dominio.
- No se almacenan secretos ni credenciales.

## Pendiente antes de implementación

- Confirmar proveedor de datos en Lovable.
- Confirmar autenticación.
- Definir políticas de acceso.
- Crear ADR de modelo de datos final.
