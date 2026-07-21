# Alineación CTO de Atlas

Este documento consolida los criterios esperados para que Atlas quede preparado según una revisión de CTO: orden, trazabilidad, claridad de alcance y cero implementación prematura.

## Lineamientos no negociables

- No generar código hasta que el alcance funcional esté aprobado.
- Mantener el README como entrada breve, no como documento extenso.
- Usar `docs/` como fuente principal de verdad.
- Separar producto, arquitectura, operación y seguridad.
- Registrar decisiones antes de ejecutar cambios estructurales.
- Mantener enlaces internos actualizados cuando se agreguen documentos.
- Evitar secretos, credenciales o información privada.

## Criterios de calidad documental

| Criterio | Expectativa |
| --- | --- |
| Claridad | Cada documento debe explicar su propósito desde el inicio. |
| Trazabilidad | Las decisiones deben conectarse con contexto, impacto y estado. |
| Mantenibilidad | La información debe vivir en un solo lugar principal. |
| Escalabilidad | La estructura debe permitir crecer sin reorganizar todo. |
| Control | La implementación queda bloqueada hasta cerrar definición. |

## Checklist CTO

- [x] Repositorio con README claro.
- [x] Índice documental disponible.
- [x] Arquitectura documentada sin código.
- [x] Producto documentado con PRD y alcance.
- [x] Roadmap por etapas.
- [x] Gobernanza y flujo de trabajo.
- [x] Seguridad y privacidad documentadas.
- [x] Plantillas para colaboración.
- [x] Criterios para pasar a implementación.
