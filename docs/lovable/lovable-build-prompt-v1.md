# Lovable Build Prompt v1 de Atlas

## Estado del documento

Prompt maestro documental para preparar la futura construcción de Atlas MVP v1 en Lovable. No debe ejecutarse todavía como generación de código sin ADR de inicio aprobada.

## Objetivo del prompt

Guiar a Lovable para construir Atlas MVP v1 respetando Product Bible, AIOS Bible, Design System, PRD, UX Specification, System Architecture, Database Schema v1 y Security Model v1.

## Contexto para Lovable

Atlas es una plataforma documental y operativa para convertir ideas, conversaciones y decisiones en una especificación clara, trazable y lista para ejecución.

El MVP debe enfocarse en visualizar y gestionar la especificación oficial del proyecto, no en automatizaciones avanzadas.

## Instrucciones principales

Cuando la implementación sea aprobada, construir una aplicación con:

- Dashboard de estado del proyecto.
- Biblioteca de documentos por dominio.
- Registro de decisiones.
- Backlog priorizado.
- Roadmap por etapas.
- Readiness checklist.
- Recursos y enlaces.

## Reglas obligatorias

- No inventar módulos fuera del MVP Definition v1.
- No agregar integraciones no aprobadas.
- No incluir secretos ni credenciales.
- Mantener diseño sobrio, claro y profesional.
- Usar navegación simple por dominios.
- Mostrar estado y próximos pasos de forma prioritaria.
- Respetar el Database Schema v1 conceptual.
- Respetar el Security Model v1.

## Navegación esperada

```text
Dashboard
Documentos
Decisiones
Backlog
Roadmap
Readiness
Recursos
```

## Pantalla Dashboard

Debe mostrar:

- Nombre del proyecto.
- Estado actual.
- Etapa del roadmap.
- Próximos pasos.
- Pendientes críticos.
- Últimas decisiones.

## Pantalla Documentos

Debe agrupar documentos por:

- Producto.
- Arquitectura.
- Diseño.
- Operación.
- Seguridad.
- API e integraciones.
- Roadmap.

## Pantalla Decisiones

Debe mostrar:

- Título.
- Tipo.
- Estado.
- Fecha.
- Contexto.
- Decisión.
- Consecuencias.

## Pantalla Backlog

Debe mostrar:

- Título.
- Prioridad.
- Estado.
- Documento relacionado.
- Decisión relacionada.

## Pantalla Readiness

Debe mostrar criterios por dominio y estado:

- Pendiente.
- Completo.
- Bloqueado.

## Fuera de alcance del prompt v1

- Automatizaciones con IA.
- Envío real de emails.
- Integraciones externas.
- Analítica avanzada.
- Editor colaborativo complejo.

## Condición de uso

Este prompt solo debe usarse cuando el equipo apruebe iniciar implementación mediante ADR formal.
