# Arquitectura de Atlas

Esta carpeta concentra la documentación arquitectónica fundacional de Atlas. No contiene implementación ni código; su objetivo es dejar preparada la estructura de trabajo acordada para que el proyecto pueda evolucionar con orden.

## Principios arquitectónicos

- **Documentación primero:** antes de construir, toda decisión importante debe quedar escrita.
- **Separación por dominios:** producto, arquitectura, operación y seguridad viven en documentos separados.
- **Trazabilidad:** cada decisión relevante debe poder conectarse con una necesidad, una restricción o una tarea.
- **Evolución incremental:** la arquitectura se actualizará por fases, sin asumir detalles técnicos que todavía no estén definidos.
- **Claridad para colaboración:** cualquier persona que entre al repositorio debe entender qué existe, qué falta y dónde documentarlo.

## Estructura documental acordada

```text
docs/
├── arquitectura/       # Visión técnica, decisiones y componentes futuros
├── producto/           # Problema, usuarios, alcance y criterios de éxito
├── operacion/          # Flujo de trabajo, seguimiento y mantenimiento
├── seguridad/          # Riesgos, controles y privacidad
└── plantillas/         # Formatos reutilizables para nuevas definiciones
```

## Documentos iniciales

- [Visión técnica](vision-tecnica.md)
- [Mapa de componentes](mapa-componentes.md)
- [Decisiones arquitectónicas](decisiones-arquitectonicas.md)
