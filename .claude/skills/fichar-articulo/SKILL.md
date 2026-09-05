---
name: fichar-articulo
description: Convierte un PDF de artículo científico en una ficha de lectura estructurada, su entrada BibTeX y una fila de la matriz del estado del arte. Úsala cuando haya un PDF nuevo en 2-fuentes/pdfs/, o cuando Hans pida "fichar", "analizar este paper" o preparar el informe de análisis de artículos.
---

# Fichar un artículo

Cada artículo aceptado produce **tres salidas sincronizadas**:
1. Ficha en `2-fuentes/fichas/`
2. Entrada en `2-fuentes/biblioteca.bib`
3. Fila en `2-fuentes/matriz-estado-arte.csv`

**La ficha es nota interna, no un entregable.** El informe de análisis de artículos que sí se
entrega puede tener formato oficial del profesor → **pregunta #3** en `preguntas-abiertas.md`.
Si llega ese formato, la ficha alimenta al informe; no lo reemplaza.

## Ritmo real 🟥

24 artículos en 5 semanas (~5 por semana). El fichado tiene que ser rápido y uniforme, o no se llega.

| Semana | Artículos | Revisión aleatoria del asesor |
|---|---|---|
| 6 | 1-4 | |
| 7 | 5-8 | ← artículos 1 al 4 |
| 8 | 9-14 | |
| 9 | 15-20 | ← artículos 5 al 14 |
| 10 | 21-24 | |

En las revisiones aleatorias el asesor puede preguntar por cualquiera. La ficha tiene que servir
para responder **sin releer el PDF**.

## Paso 0 — Verificar admisibilidad ANTES de invertir tiempo 🟥

Contra `CONTEXTO.md` §5: ¿año ≥ 2023? ¿artículo de aporte (no revisión, no conferencia)?
¿journal Q1 o Q2 en SCImago?

Si falla alguno: **detenerse y avisar.** No fichar algo inutilizable. Ofrecer registrarlo como
fuente de contexto para el capítulo 1 si aporta datos del sector.

## Paso 1 — Extraer el texto

```bash
pdftotext -layout "2-fuentes/pdfs/<archivo>.pdf" -
```

Si el PDF es una imagen escaneada, `pdftotext` devuelve poco o nada: **avisarlo, no inventar contenido**.

## Paso 2 — Nombrar el PDF 🟦

`autor-año-palabraclave.pdf`, minúsculas, sin tildes ni espacios.
Ejemplo: `zhang-2024-federated-learning-health.pdf`.
El PDF **solo se renombra**, nunca se modifica (regla 🟥7).

## Paso 3 — Escribir la ficha

Plantilla: `2-fuentes/fichas/_plantilla-ficha.md` → guardar como `2-fuentes/fichas/autor-año-palabra.md`.

Reglas de contenido:
- **Todo dato bibliográfico sale del PDF o de la base de datos.** Lo no verificable va `[VERIFICAR]` 🟥.
- **Número de página obligatorio** en cada afirmación importante: sin él no se puede citar
  textualmente después en APA-7.
- "Relación con nuestro proyecto" es lo que realmente importa. Un resumen genérico no sirve:
  responder *¿qué me llevo y para qué sección?*

**Las dos secciones que más rinden** 🟥:
- **Métricas de validación** → definen los *indicadores de éxito* del capítulo 1. El curso lo dice
  literal: el estado del arte *"permite conocer métodos / métricas para validar solución"*.
- **Limitaciones y trabajo futuro** → de ahí sale la brecha. El curso lista los *"capítulos trabajos
  futuros"* como fuente de ideas de investigación.

## Paso 4 — BibTeX

Añadir a `2-fuentes/biblioteca.bib`. Clave `autorAñoPalabra` (ej. `zhang2024federated`).
Campos mínimos: `author`, `title`, `journal`, `year`, `volume`, `number`, `pages`, `doi`.

**El DOI es obligatorio.** Si no aparece, `doi = {VERIFICAR}` y avisar.

Si Hans usa Zotero (ver `2-fuentes/guia-zotero.md`), preferir **exportar desde Zotero** en vez de
escribir la entrada a mano: menos errores de transcripción.

## Paso 5 — Fila en la matriz

Añadir a `2-fuentes/matriz-estado-arte.csv` respetando las columnas.

**Usar vocabulario consistente** entre artículos: la matriz se convierte en la tabla comparativa
del capítulo 2.3, y si cada fila parafrasea distinto no se puede comparar nada.

## Paso 6 — Cierre

- Si surgió una duda de criterio → anotarla en `1-gestion/preguntas-abiertas.md` (regla 🟦11).
- El anexo de uso de IA aún **no se lleva**: pendiente de la respuesta del asesor (pregunta #2).
