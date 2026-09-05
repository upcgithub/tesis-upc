---
name: estado-del-arte
description: Consolida las fichas en el capítulo 2 del documento — metodología, desarrollo, análisis y discusión. Úsala para construir la tabla comparativa, identificar la brecha de investigación que justifica el aporte, o trabajar cualquier sección del capítulo 2 (2.1 a 2.4).
---

# Capítulo 2: Estado del arte

Estructura exigida 🟥 (`CONTEXTO.md` §3):

| Sección | Contenido | Se evalúa en |
|---|---|---|
| 2.1 | Metodología y planificación | TB1 (sem. 7) |
| 2.2 | Desarrollo de la investigación | TB1 (sem. 7) |
| 2.3 | Análisis de la investigación | TB2 (sem. 11) |
| 2.4 | Discusión y resultados para el proyecto | TB2 (sem. 11) |

**El documento se escribe en Word**, sobre el formato oficial del profesor
(`6-material-oficial/`). Aquí se prepara el contenido, no el formato.

## 2.1 Metodología y planificación

Se construye **desde `2-fuentes/busquedas/`**, no desde cero. Debe contener:
- Preguntas de investigación que guían la revisión
- Bases consultadas y **fecha** de consulta
- Cadenas de búsqueda **textuales**, por base
- Criterios de inclusión y exclusión
- Proceso de cribado con números por etapa
- Criterio de evaluación de calidad de los estudios

> 🟨 La estructura de cribado que uso sigue el estilo PRISMA. **El curso no nombra ningún estándar**
> (habla de "fases 1 a 4"). Es la **pregunta #5** de `preguntas-abiertas.md`. Si el asesor indica
> otro método, esta sección cambia.

## 2.2 Desarrollo de la investigación

Presentar los estudios **agrupados por criterio**, no uno tras otro.
Agrupar por técnica, por enfoque del problema o por dominio — y **decir explícitamente qué criterio
de agrupación se usó y por qué**.

🟨 *Criterio propio:* el antipatrón a evitar es el catálogo —
*"Zhang (2024) propone… Li (2024) propone… Kumar (2023) propone…"*.
Patrón preferible: *"Los enfoques basados en X se dividen en dos familias. La primera, representada
por Zhang (2024) y Li (2024), comparte el supuesto de que […]. La segunda […]"*.
Esto es guía de escritura académica general, no exigencia del curso.

## 2.3 Análisis de la investigación

Aquí entra la **tabla comparativa**, generada desde `2-fuentes/matriz-estado-arte.csv`.
Ejes útiles: problema atacado · técnica · dataset/escenario · métricas · resultados · limitaciones.

Debe responder 🟥:
- ¿Qué técnicas dominan y por qué?
- **¿Qué métricas usa la comunidad para validar?** → definen los indicadores de éxito del cap. 1
- ¿Qué escenarios se han probado y cuáles no?
- **¿Cuáles son los mejores resultados reportados?** → es la línea base que hay que superar

El curso exige que el aporte tenga *"mejores resultados que la literatura"*. Sin esta sección
no hay contra qué compararse.

## 2.4 Discusión y resultados para el proyecto

Cierra con **la brecha**:

> 🟨 *Plantilla, no exigencia:*
> "Ningún trabajo revisado aborda [problema] mediante [técnica] en [escenario]. Los trabajos más
> cercanos, [A] y [B], presentan la limitación de […]. Esta brecha justifica el aporte del capítulo 3."

Esa frase sostiene la **originalidad** 🟥 — el curso la define como que no existan dos tesis con el
mismo problema + propuesta + técnica + escenario. Construirla es el propósito del capítulo entero.

## Verificaciones antes de cerrar el capítulo

- [ ] Todo artículo citado tiene ficha en `2-fuentes/fichas/` y entrada en `biblioteca.bib`
- [ ] Todo artículo del estado del arte cumple: ≤3 años, Q1/Q2, de aporte
- [ ] La cantidad coincide con lo que pide el cronograma (**24 al cierre de la semana 10**)
- [ ] Citas en APA-7; toda cita está en las referencias y toda referencia se cita
- [ ] La brecha de 2.4 apunta directamente a los objetivos del capítulo 1
- [ ] Las métricas de 2.3 son las mismas que los indicadores de éxito de 1.3
- [ ] Ninguna afirmación con `[VERIFICAR]` pendiente
