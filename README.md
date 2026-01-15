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

## Metodología elegida (BEM) y comparación breve con OOCSS y SMACSS

| Metodología | Fortalezas | Debilidades | Mejor para |
|-------------|------------|-------------|------------|
| **BEM** | Nombres claros, escalable, sin conflictos | Nombres largos | Equipos grandes, PixelPerfect[web:44] |
| OOCSS | Reutilización, separa estructura/piel | Abstracta para novatos | UI consistente |
| SMACSS | Flexible, categorías | Menos reglas, inconsistencias | Equipos que definen sus guías |

**Elegimos BEM** porque PixelPerfect tiene **múltiples equipos** y proyectos simultáneos. La nomenclatura explícita (`profile-card__name`) evita colisiones y facilita colaboración.[web:44][file:1]

| Metodología | Naming | Colaboración |
|-------------|--------|--------------|
| **BEM** | `bloque__elemento--modificador` | ⭐⭐⭐⭐⭐ |
| OOCSS | `.grid-3` reutilizable | ⭐⭐⭐ |
| SMACSS | `.module .state-active` | ⭐⭐⭐⭐ |

**BEM gana**: Nomenclatura explícita para PixelPerfect Studio.[web:44]
## Diseño e implementación. (explicar el componente y clases BEM + Estructura SCSS)
## Documentación técnica de la estructura CSS/SCSS.
## Reflexión final del proceso.