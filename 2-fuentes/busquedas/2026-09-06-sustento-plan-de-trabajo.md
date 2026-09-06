# Búsqueda: sustento del Plan de Trabajo (semana 2)

- **Fecha de diseño:** 2026-09-06
- **Objetivo:** poblar los 4 huecos del sustento del Plan de Trabajo
- **Tema:** Sistema de gestión y priorización de prospectos de aporte con segmentación analítica
  para museos privados sin fines de lucro

## Descomposición del tema

| Componente | Término base | Variantes en inglés |
|---|---|---|
| **Problema** | baja conversión y retención de donantes | donor retention · donor churn · donor attrition · membership retention · lapsed donor |
| **Aporte** | sistema de gestión y priorización de prospectos | donor management system · prospect prioritization · nonprofit CRM · fundraising system |
| **Técnica** | segmentación analítica | donor segmentation · RFM analysis · clustering · unsupervised learning · predictive analytics |
| **Escenario** | museos privados sin fines de lucro | museum · cultural institution · cultural heritage · nonprofit · third sector |

---

## Capa 1 — Contexto del sector (NO es Scopus)

**Qué se busca:** evidencia de que los museos dependen de donaciones porque la taquilla no cubre
su operación.

**Por qué no en Scopus:** son datos estadísticos institucionales, no hallazgos de investigación.
El formato del Plan de Trabajo los admite expresamente: *"informes gubernamentales, informes de
instituciones tecnológicas confiables, diarios nacionales o internacionales"*.
Criterio aplicable: **≤ 5 años** (informes), no el de artículos científicos.

**Dónde buscar:**

| Fuente | Qué puede tener |
|---|---|
| Ministerio de Cultura del Perú — *Infocultura* | Estadísticas de museos en el Perú, visitantes, financiamiento |
| INEI | Datos de asistencia a actividades culturales, gasto cultural de los hogares |
| ICOM (International Council of Museums) | Informes sobre situación y financiamiento de museos |
| NEMO (Network of European Museum Organisations) | Encuestas anuales con estructura de ingresos de museos |
| AAM (American Alliance of Museums) | *Museums and Public Opinion*, informes financieros del sector |
| UNESCO | Informes globales sobre museos |

**Cómo buscar:** en el sitio de cada institución, o en Google con `site:`:
```
site:gob.pe museos estadísticas financiamiento
site:icom.museum museum funding report
site:ne-mo.org museum survey income
```

**Registro de lo encontrado:**

| Fuente | Año | Dato concreto | ¿Sirve? |
|---|---|---|---|
| | | | |

---

## Capa 2 — El problema: retención y conversión de donantes

**Dónde:** Scopus y Web of Science, vía proxy UPC.
**Criterio:** artículos ≤ 3 años (2023+), Q1/Q2, de aporte.

### Scopus — cadena equilibrada

```
TITLE-ABS-KEY(
  ("donor retention" OR "donor churn" OR "donor attrition" OR "membership retention"
   OR "lapsed donor" OR "donor loyalty")
  AND (nonprofit OR "non-profit" OR charity OR "third sector" OR museum OR "cultural institution")
)
AND PUBYEAR > 2022 AND DOCTYPE(ar) AND LANGUAGE(english)
```

### Scopus — cadena amplia (si la anterior devuelve muy pocos)

```
TITLE-ABS-KEY(
  ("donor retention" OR "donor churn" OR "charitable giving" OR "repeat donation"
   OR "membership renewal")
  AND (nonprofit OR "non-profit" OR charity OR philanthrop* OR fundraising)
)
AND PUBYEAR > 2021 AND DOCTYPE(ar)
```

### Web of Science

```
TS=(("donor retention" OR "donor churn" OR "membership retention")
    AND (nonprofit OR charity OR museum OR "cultural institution"))
```
Refinar: *Publication Years* 2023-2026 · *Document Types* Article

**Resultados:**

| Cadena | Base | Fecha | N devueltos | N útiles |
|---|---|---|---|---|
| | | | | |

---

## Capa 3 — La técnica: segmentación analítica de donantes

**Esta capa alimenta también el estado del arte del capítulo 2.** Guardar todo lo que salga.

### Scopus — segmentación aplicada a captación de fondos

```
TITLE-ABS-KEY(
  ("donor segmentation" OR "customer segmentation" OR "RFM analysis" OR clustering
   OR "unsupervised learning" OR "predictive analytics")
  AND (fundraising OR donation* OR philanthrop* OR nonprofit OR "non-profit" OR charity)
)
AND PUBYEAR > 2022 AND DOCTYPE(ar) AND LANGUAGE(english)
```

### Scopus — específica del escenario (museos y cultura)

```
TITLE-ABS-KEY(
  (museum* OR "cultural institution*" OR "cultural heritage" OR "arts organization*")
  AND (membership OR donor* OR fundraising OR patron* OR sponsor*)
  AND (analytics OR segmentation OR "machine learning" OR "data mining" OR CRM)
)
AND PUBYEAR > 2022 AND DOCTYPE(ar)
```

> Esta última probablemente devuelva **pocos resultados**. Eso no es un fracaso: es evidencia
> de la **brecha** que justifica el aporte, y se documenta como tal en el capítulo 2.4.

### Scopus — por qué no basta un CRM comercial

```
TITLE-ABS-KEY(
  ("CRM adoption" OR "CRM implementation" OR "information system adoption")
  AND (nonprofit OR "non-profit" OR charity OR "small organization*")
  AND (barrier* OR challenge* OR limitation* OR failure)
)
AND PUBYEAR > 2021 AND DOCTYPE(ar)
```

**Resultados:**

| Cadena | Base | Fecha | N devueltos | N útiles |
|---|---|---|---|---|
| | | | | |

---

## Criterios de inclusión y exclusión

**Incluir:** artículo de aporte · revista indexada · Q1 o Q2 · ≤ 3 años · aborda al menos 2 de los
4 componentes · texto completo accesible.

**Excluir:** revisiones · mapeos · conferencias · congresos · resúmenes · editoriales ·
Q3, Q4 o sin cuartil · sin texto completo · duplicado.

## Cribado

| Etapa | N |
|---|---|
| Identificados | |
| Duplicados eliminados | |
| Cribados por título/resumen | |
| Excluidos (con motivo) | |
| Evaluados a texto completo | |
| **Incluidos** | |
