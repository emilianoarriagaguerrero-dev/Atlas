# Decisiones arquitectónicas

Este documento registra decisiones técnicas o estructurales relacionadas con la arquitectura de Atlas.

## ADR-001 — Priorizar documentación fundacional

**Fecha:** 2026-07-21

**Estado:** aceptada

**Contexto:** Atlas necesita una base clara antes de iniciar cualquier implementación.

**Decisión:** crear primero la estructura documental fundacional y no generar código en esta etapa.

**Consecuencias:** el repositorio crecerá inicialmente con documentos de producto, arquitectura, operación y seguridad. El código se agregará solo cuando existan requisitos aprobados.

## ADR-002 — Separar documentación por áreas

**Fecha:** 2026-07-21

**Estado:** aceptada

**Contexto:** la documentación inicial puede crecer y volverse difícil de mantener si todo vive en un solo archivo.

**Decisión:** separar la documentación en carpetas por área: arquitectura, producto, operación, seguridad y plantillas.

**Consecuencias:** cada área tendrá su propio lugar y el README seguirá siendo una entrada breve.

## ADR-003 — Bloquear implementación hasta cumplir Definition of Ready

**Fecha:** 2026-07-21

**Estado:** aceptada

**Contexto:** iniciar código sin requisitos claros puede generar retrabajo, deuda técnica y decisiones prematuras.

**Decisión:** Atlas no tendrá código hasta completar los criterios de implementación definidos en `criterios-implementacion.md`.

**Consecuencias:** cualquier solicitud de implementación deberá pasar primero por producto, arquitectura, seguridad y backlog.
