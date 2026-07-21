# UX Specification de Atlas

## Estado del documento

Esta especificación UX forma parte de la documentación oficial de Atlas y prepara una futura implementación en Lovable. No incluye componentes en código.

## Objetivo UX

Crear una experiencia clara para consultar el estado del proyecto, navegar documentación oficial, revisar decisiones y entender qué falta antes de implementar.

## Principios UX

- Estado primero.
- Navegación por dominios.
- Lectura rápida antes de detalle.
- Trazabilidad visible.
- Acciones futuras simples y reversibles.

## Usuarios y necesidades

| Usuario | Necesidad UX |
| --- | --- |
| Responsable del proyecto | Ver qué está listo y qué falta |
| CTO | Validar arquitectura, readiness y decisiones |
| Colaborador | Encontrar el documento correcto para contribuir |
| Desarrollador futuro | Entender requisitos antes de implementar |

## Arquitectura de información futura

```text
Inicio
├── Estado del proyecto
├── Producto
│   ├── Product Bible
│   ├── PRD
│   ├── Requisitos
│   └── Roadmap
├── Arquitectura
│   ├── AIOS Bible
│   ├── System Architecture
│   ├── Database Design
│   └── ADRs
├── Diseño
│   ├── Design System
│   └── UX Specification
├── Operación
│   ├── Gobernanza
│   ├── Backlog
│   └── Definition of Done
└── Recursos
```

## Pantallas futuras sugeridas para Lovable

### 1. Dashboard

Debe mostrar:

- Estado general.
- Etapa actual.
- Próximos pasos.
- Pendientes críticos.
- Últimas decisiones.

### 2. Biblioteca documental

Debe permitir navegar documentos por dominio: producto, arquitectura, diseño, operación y seguridad.

### 3. Backlog

Debe mostrar tareas por prioridad y estado.

### 4. Decisiones

Debe listar decisiones con fecha, estado, contexto e impacto.

### 5. Readiness

Debe mostrar criterios pendientes antes de permitir implementación.

## Flujos principales

### Flujo: revisar estado

1. Entrar al dashboard.
2. Revisar etapa actual.
3. Consultar próximos pasos.
4. Abrir documentos relacionados.

### Flujo: validar implementación futura

1. Abrir Readiness.
2. Revisar criterios técnicos y de producto.
3. Consultar ADRs.
4. Confirmar si se puede pasar a Lovable.

## Reglas de contenido

- Usar español claro.
- Mostrar resúmenes antes de texto largo.
- Evitar duplicar información.
- Enlazar documentos relacionados.
- Indicar estado de cada documento cuando aplique.

## Fuera de alcance UX actual

- Wireframes visuales finales.
- Prototipo interactivo.
- Componentes implementados.
- Animaciones o microinteracciones finales.
