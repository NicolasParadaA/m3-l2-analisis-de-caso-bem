# Documentación Análisis de caso

## Introducción y contexto del caso

PixelPerfect Studio enfrenta problemas de escalabilidad en CSS por selectores genéricos y duplicados. Se adopta **BEM** para modularizar estilos en múltiples proyectos.[file:1]

Componente elegido: **Profile Card** (adaptado de W3Schools), bloque BEM: `profile-card`.
## Diagnóstico técnico del problema

- **Selectores genéricos**: `.card` afecta múltiples elementos no deseados.[file:1]
- **Especificidad alta**: `!important` y selectores anidados generan conflictos.
- **Duplicación**: Mismo estilo repetido en varios archivos.
- **Dificultad colaborativa**: Sin convención, cada dev usa su naming.

BEM soluciona con **bloques independientes** (ej: `profile-card`), **elementos** (`__name`) y **modificadores** (`--featured`).[web:20]

## Metodología elegida (BEM) y comparación breve con OOCSS y SMACSS.
## Diseño e implementación. (explicar el componente y clases BEM + Estructura SCSS)
## Documentación técnica de la estructura CSS/SCSS.
## Reflexión final del proceso.