# Reglas del proyecto de tesis

Proyecto de investigación para titulación en Ingeniería de Sistemas (UPC), a lo largo de tres cursos:
**1FIS0311 Seminario de Investigación Aplicada** (actual, 2026-25), **1FIS0307 Proyecto de
Investigación 1** y **1FIS0308 Proyecto de Investigación 2**.

**Antes de hacer nada, lee `1-gestion/CONTEXTO.md`.** Contiene los hechos verificados del curso.
Si algo de este archivo lo contradice, gana CONTEXTO.md.

Cada regla lleva marcado su origen:
🟥 **exigencia del curso** (no negociable) · 🟦 **acuerdo de trabajo con Hans** · 🟨 **criterio propio** (descartable)

---

## 🟥 1. Nunca inventar una referencia

Ni título, ni autores, ni año, ni DOI, ni journal, ni páginas. Una referencia falsa en una tesis es
falta de integridad académica, y se detecta pidiendo el PDF.

- Toda entrada de `2-fuentes/biblioteca.bib` debe venir de un PDF real en `2-fuentes/pdfs/` o de un
  registro verificado en Scopus / WoS / el sitio del editor.
- Lo que no se pueda verificar se escribe `[VERIFICAR]`. Nunca se rellena con algo plausible.
- **No tengo acceso a Scopus ni WoS.** Si pides "busca papers sobre X", diseño la cadena de búsqueda
  para que la ejecutes tú; no genero una lista de resultados.
- No citar un artículo cuyo texto no se haya leído (al menos abstract y conclusiones).

## 🟥 2. Criterios de admisión de fuentes

De `CONTEXTO.md` §5:
- **Artículos científicos:** ≤ 3 años (2023+), revista indexada, **Q1 o Q2**, **de aporte**
  (no revisiones, no conferencias, no congresos, no resúmenes), preferible en inglés.
- **Tesis, libros, artículos académicos, informes:** ≤ 5 años (2021+), preferible en inglés.

Verificar el cuartil en SCImago o JCR **antes** de fichar, y registrarlo con su año.
Una fuente que no cumpla puede usarse como contexto en el capítulo 1, marcada explícitamente como
tal — nunca como parte del estado del arte.

## 🟥 3. Los formatos de entregable los da el profesor

**Nunca crear un formato propio para algo que se entrega.** El profesor publica el formato oficial
de cada entregable semana a semana; van a `6-material-oficial/` y se usan tal cual.

Si falta el formato de un entregable: **se pide, no se inventa.** Anotarlo en
`1-gestion/preguntas-abiertas.md`.

*(Esta regla la aportó Hans, y aplica también a plantillas de capítulos, informes de análisis
de artículos y artefactos de gestión.)*

## 🟥 4. Coherencia de punta a punta

El curso evalúa explícitamente esta cadena:

```
Problemática → problemas a resolver → investigación → objetivos del proyecto
  → diseño de solución → solución elaborada → validación y resultados
```

Antes de cerrar cualquier sección, verificar que apunta hacia atrás. Si un objetivo específico no
resuelve ninguno de los problemas formulados, decirlo. Si el diseño no cubre algún objetivo, decirlo.

## 🟥 5. El problema se abstrae de la organización

El problema debe plantearse de forma que la solución sirva a **todas** las organizaciones similares.
Si Hans lo redacta pegado a una empresa concreta, corregirlo.

## 🟥 6. Normas de redacción

APA-7 en el documento de tesis. **IEEE** en el paper. Nunca mezclados en un mismo documento.

## 🟥 7. Material de solo lectura

`6-material-oficial/` **no se edita, no se renombra, no se reorganiza.** Es la evidencia de lo que se pidió.
`2-fuentes/pdfs/` tampoco: el PDF descargado se puede renombrar, nunca modificar. Las notas van en
`2-fuentes/fichas/`.

---

## 🟦 8. Formato de trabajo

- **Los entregables se escriben en Word**, sobre el formato oficial del profesor.
- **Markdown solo para notas internas:** fichas de lectura, bitácora, actas, borradores, búsquedas.
- Idioma: español. El paper puede ir en inglés.

## 🟦 9. Nombres de archivo

Minúsculas, sin espacios ni tildes, separadas por guiones, fechas ISO `YYYY-MM-DD`.
Ejemplo: `2026-09-15-acta-asesoria.md`.
**Excepción:** el material oficial conserva su nombre original tal cual.

## 🟦 10. Git

- Commits en español, en imperativo, describiendo el avance real:
  `añade fichas de artículos 5-8`, `redacta 1.2.3 importancia del problema`.
- **Nunca añadir líneas `Co-Authored-By:` ni referencias a Claude/Anthropic** en los mensajes de commit.
- Commit al cerrar cada sesión y **siempre antes de una entrega**.
- Cada entrega evaluada se etiqueta (`git tag TB1-2026-25`) y se congela en `3-documento/entregas/`.
- La identidad de git y la autenticación de `gh` son **locales a este repo**. No tocar la
  configuración global ni la cuenta de trabajo (`github.disney.com`).

## 🟦 11. Ante la duda, se pregunta

Cuando aparezca un criterio ambiguo o un dato que el material oficial no defina, **no se asume**:
se anota en `1-gestion/preguntas-abiertas.md` con a quién preguntar y por qué importa.

---

## 🟨 12. Anti-patrones

- No redactar secciones completas sin haber discutido antes el contenido y las fuentes.
  Primero esquema y fuentes, después redacción.
- No rellenar plantillas con texto de ejemplo plausible. Si falta información real, dejar el hueco.
- No borrar nada de `7-archivo/` — ahí va lo descartado, precisamente para poder volver.
- Al reportar avance, decir lo que realmente se hizo. Si algo quedó a medias o no se pudo verificar,
  decirlo explícitamente.
