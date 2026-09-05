# Proyecto de Tesis — Ingeniería de Sistemas UPC

Un solo proyecto de investigación, tres ciclos:

| Ciclo | Curso | Produce |
|---|---|---|
| VIII | **1FIS0311 Seminario de Investigación Aplicada** ← actual (2026-25) | Problema · Estado del arte · Diseño del aporte · Plan · Paper 1/3 |
| IX | 1FIS0307 Proyecto de Investigación 1 | Objetivos 1-3 de la solución · Paper 2/3 |
| X | 1FIS0308 Proyecto de Investigación 2 | Objetivo 4 · Validación · Resultados · Conclusiones · Paper 3/3 |

**Empieza por [`1-gestion/CONTEXTO.md`](1-gestion/CONTEXTO.md)** — hechos del curso, fechas, pesos,
criterios de fuentes y estado actual. Las reglas de trabajo están en [`CLAUDE.md`](CLAUDE.md).

---

## Estructura

```
tesis/
├── CLAUDE.md              Reglas de trabajo (marcadas por origen)
├── 1-gestion/
│   ├── CONTEXTO.md        ← FUENTE DE VERDAD del curso
│   ├── cronograma.md      15 semanas + hitos de evaluación
│   ├── preguntas-abiertas.md   Dudas para el profesor / asesor / coordinación
│   ├── bitacora/          Una entrada por sesión de trabajo
│   ├── asesorias/         Actas de reunión (artefacto de gestión evaluado)
│   ├── plan-proyecto/     Alcance, cronograma, calidad, riesgos
│   └── admin/             Carta de compromiso, control de cambios
├── 2-fuentes/             El activo que más valor acumula en 3 ciclos
│   ├── guia-zotero.md
│   ├── biblioteca.bib     Referencias (export de Zotero)
│   ├── matriz-estado-arte.csv   → se convierte en la tabla del cap. 2.3
│   ├── pdfs/              PDFs originales — solo renombrar, nunca editar
│   ├── fichas/            Nota interna de lectura, una por artículo
│   └── busquedas/         Registro de cada búsqueda, con fecha y cribado
├── 3-documento/
│   ├── formatos-oficiales/   .docx del profesor — SOLO LECTURA
│   ├── trabajo/              Donde se escribe (Word)
│   └── entregas/             Congeladas al entregar
├── 4-paper/               El artículo científico (IEEE)
├── 5-solucion/            Código y artefactos del aporte (ciclos IX-X)
│   ├── data/raw/          Datos originales — inmutable
│   ├── data/processed/    Datos derivados
│   ├── src/               Código
│   └── results/           Figuras, tablas, resultados
├── 6-material-curso/      Material original del profesor — SOLO LECTURA
└── 7-archivo/             Descartes y versiones muertas (no se borra)
```

### Regla clave

**Los formatos de entregable los da el profesor, semana a semana.** Van a
`3-documento/formatos-oficiales/` intactos, y se escribe sobre copias en `trabajo/`.
Si falta un formato, se pide — no se inventa.

---

## Flujo semanal

1. Abrir `1-gestion/CONTEXTO.md` §11 y `cronograma.md` → qué semana es y qué toca
2. Buscar fuentes con la skill `buscar-fuentes` → registro en `2-fuentes/busquedas/`
3. Fichar cada artículo aceptado (`fichar-articulo`) → ficha + BibTeX + fila de matriz
4. Redactar en Word sobre el formato oficial, citando desde Zotero
5. Cerrar con la skill `bitacora` y un commit

**Antes de cada entrega:** skill `revisar-entregable`.

## Skills disponibles

| Skill | Para qué |
|---|---|
| `buscar-fuentes` | Cadenas para Scopus/WoS, criterios de cribado, registro de la búsqueda |
| `fichar-articulo` | PDF → ficha + BibTeX + fila de la matriz |
| `estado-del-arte` | Construir el capítulo 2 y encontrar la brecha |
| `revisar-entregable` | Auditoría antes de TB1/TB2/TB3/DD |
| `bitacora` | Registro de sesión y actas de asesoría |

## Herramientas

- **Gestor bibliográfico:** Zotero → `2-fuentes/guia-zotero.md`
- **Bases:** Scopus, Web of Science, SCImago (cuartiles)
- **Texto de PDF:** `pdftotext -layout archivo.pdf -`
- **Git:** aislado de la configuración de trabajo. Usar `./gh-tesis` en vez de `gh`.

## Estado

Carga del ciclo: **24 artículos** Q1/Q2 entre las semanas 6 y 10.
Evaluaciones: TB1 (sem. 7, 20 %) · TB2 (sem. 11, 20 %) · TB3 (sem. 15, 30 %) · DD (sem. 15, 30 %).
**7 preguntas abiertas** pendientes de asesoría → `1-gestion/preguntas-abiertas.md`.
