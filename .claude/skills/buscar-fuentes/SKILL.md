---
name: buscar-fuentes
description: Diseña y registra búsquedas de literatura para el estado del arte (Scopus, Web of Science, SCImago). Úsala cuando haya que encontrar artículos, construir cadenas de búsqueda, definir criterios de inclusión/exclusión, verificar si una fuente cumple los criterios del curso, o registrar el cribado.
---

# Búsqueda de fuentes

## Límite que no se negocia

**No tengo acceso a Scopus ni a Web of Science.** Mi trabajo es *diseñar* la búsqueda y *procesar*
lo que Hans traiga de vuelta. Nunca generar una lista de resultados: sería inventar referencias
(regla 🟥1 de `CLAUDE.md`).

Si hace falta resultados: entregar las cadenas listas para pegar y pedir el export.

## Contexto de carga 🟥

Son **24 artículos** repartidos en 5 semanas (`CONTEXTO.md` §4), con dos revisiones aleatorias del
asesor. Talleres oficiales de búsqueda: semana 3 (SCOPUS, WoS, SCIMAGO) y semana 6 (WoS, SCIMAGO, APA).

## Paso 1 — Descomponer el tema 🟥

Extraer los 4 componentes (`CONTEXTO.md` §6) y sus sinónimos en inglés:

| Componente | Término base | Sinónimos / variantes |
|---|---|---|
| Problema | | |
| Aporte | | |
| Técnica | | |
| Escenario | | |

Incluir plurales, siglas y su expansión, y términos del vocabulario del área.

## Paso 2 — Construir la cadena

Bloques `OR` dentro de cada componente, unidos por `AND` entre componentes.

**Scopus:**
```
TITLE-ABS-KEY( ("term1" OR "term2") AND ("term3" OR "term4") AND ("term5") )
AND PUBYEAR > 2022 AND DOCTYPE(ar) AND LANGUAGE(english)
```
`DOCTYPE(ar)` = *article*. Excluye `cp` (conference paper) y `re` (review), **que el curso
prohíbe expresamente** 🟥.

**Web of Science:**
```
TS=( ("term1" OR "term2") AND ("term3" OR "term4") )
```
Refinar por año y por *Document Types: Article*.

🟨 *Criterio propio:* generar 2-3 variantes (restrictiva / equilibrada / amplia). Una cadena que
devuelve 4 resultados o 40 000 está mal calibrada. Descartable si Hans prefiere una sola.

## Paso 3 — Criterios de inclusión y exclusión 🟥

**Inclusión:** artículo de aporte · revista indexada · **Q1 o Q2** · ≤ 3 años · aborda al menos
2 de los 4 componentes · texto completo accesible.

**Exclusión:** revisiones, mapeos, conferencias, congresos, resúmenes, editoriales · Q3, Q4 o sin
cuartil · sin acceso al texto completo · duplicado.

> ⚠️ El alcance exacto de este criterio sobre los 24 artículos es la **pregunta #4** de
> `1-gestion/preguntas-abiertas.md`. Hasta que el asesor responda, aplicar el criterio estricto.

## Paso 4 — Verificar el cuartil 🟥

Para cada candidato, **antes** de fichar:
1. Buscar el journal en [SCImago](https://www.scimagojr.com/) → anotar cuartil SJR **y el año**
   (un journal cambia de cuartil entre años).
2. Contrastar con JCR si está disponible.

Q3 o Q4 → no entra al estado del arte. Puede citarse en el capítulo 1 como contexto, marcado como tal.

## Paso 5 — Registrar la búsqueda

Crear `2-fuentes/busquedas/YYYY-MM-DD-<tema-corto>.md`:

```markdown
# Búsqueda: <tema>
- Fecha: · Base: Scopus | WoS
- Cadena ejecutada: `...`
- Filtros: años, tipo de documento, idioma
- Resultados devueltos: N

## Cribado
| Etapa | N |
|---|---|
| Identificados | |
| Duplicados eliminados | |
| Cribados por título/abstract | |
| Excluidos (con motivo) | |
| Evaluados a texto completo | |
| **Incluidos** | |

## Incluidos
| # | Autor, año | Título | Journal | Cuartil | DOI |
```

**Por qué importa** 🟥: el capítulo 2.1 se llama *"Metodología y planificación"*. Sin estos números
no se puede documentar cómo se buscó, que es justo lo que esa sección evalúa.

🟨 *Criterio propio:* la estructura de cribado sigue el estilo PRISMA. **El curso no nombra ningún
estándar** — habla de "fases 1 a 4" del estado del arte. Es la **pregunta #5** de
`preguntas-abiertas.md`. Si el asesor indica otro método, se cambia esta plantilla.

## Paso 6 — Entregar

Devolver siempre:
1. Las cadenas listas para copiar y pegar, por base de datos
2. El archivo de registro creado en `2-fuentes/busquedas/`
3. Qué exportar (RIS/BibTeX) y dónde dejarlo

Después del export, encadenar con la skill `fichar-articulo`.
