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


### Ejecutada — Scopus, 2026-09-06

**Cadena:** la equilibrada de arriba, tal cual.
**Resultado: 15 documentos.** Pocos (el rango cómodo son 50-300), lo que indica que el cruce
retención/conversión de donantes × sector no lucrativo y cultural está poco explorado.

> Los cuartiles **NO están verificados todavía**. Hay que comprobarlos uno por uno en SCImago,
> con el año de publicación del artículo. Hasta entonces, `[VERIFICAR]`.

| # | Autor, año | Título | Revista | Cuartil | Valoración |
|---|---|---|---|---|---|
| 6 | Sinha, Malik, Mahajan & ter Hofstede, 2025 | Retain, reactivate or acquire: Can nonprofits reliably use community profiles as an alternative to past donation data? | Journal of Business Research, 186, 114997 | [VERIFICAR] | **CLAVE** — usar perfiles demográficos comunitarios cuando NO hay historial de donación. Es exactamente nuestro caso |
| 4 | Hesse, 2025 | Using Machine Learning to Understand and Manage the Transformation of Peer Donors to Organizational Donors | Nonprofit Management and Leadership, 36(1) | [VERIFICAR] | **CLAVE** — ML aplicado a la transformación de donantes. Open access |
| 10 | Hoskins & Hoskins, 2024 | Age as a determinant of new donor acquisition and year-on-year retention in the university healthcare fundraising context | Journal of Philanthropy and Marketing, 29(2), e1864 | [VERIFICAR] | **ALTA** — variable demográfica como predictor; tenemos edad de los 1080 |
| 11 | Pressgrove, McKeever, McKeever & Waters, 2024 | Investigating Membership Retention: Employing Public Relations Theory to Better Understand Relationship Management | Journal of Nonprofit and Public Sector Marketing, 36(1) | [VERIFICAR] | **ALTA** — retención de membresías |
| 2 | Teck et al., 2026 | Strategies for Membership Growth in Nonprofit Organizations: Evidence from Lions Clubs New Zealand | International Review of Management and Marketing, 16(5) | [VERIFICAR] | **ALTA** — crecimiento de membresía; revisar cuartil, puede ser bajo |
| 9 | Shehu, Veseli, Clement & Winterich, 2024 | Improving Blood Donor Retention and Donor Relationships with Past Donation Use Appeals | Journal of Service Research, 27(3) | [VERIFICAR] | MEDIA — retención, dominio distinto |
| 13 | Chell, Mortimer, Masser & Russell-Bennett, 2023 | An Identity-Based Model Explaining Online Donor Appreciation | Australasian Marketing Journal, 31(1) | [VERIFICAR] | MEDIA — reconocimiento al donante; conecta con el problema de las credenciales |
| 5 | Marteau, 2025 | The power of micro-campaigns in an annual giving programme | Journal of Education Advancement and Marketing, 10(2) | [VERIFICAR] | MEDIA — campañas en programas de aporte anual |
| 14 | Samek & Longfield, 2023 | Do Thank-You Calls Increase Charitable Giving? Expert Forecasts and Field Experimental Evidence | American Economic Journal: Applied Economics, 15(2) | [VERIFICAR] | MEDIA — evidencia experimental sobre fidelización |
| 3 | Lemons, Hudson & Mazzei, 2025 | Experience design: Creating value for nonprofits | Business Horizons, 68(5) | [VERIFICAR] | MEDIA |
| 12 | Ali, Elaref & Yacout, 2023 | The effect of charity brand experience on donors' behavioral intentions | International Review on Public and Nonprofit Marketing, 20(4) | [VERIFICAR] | BAJA |
| 1 | Utaramat & Palusuk, 2026 | The Influence of Blood Donation Experience on Donor Behavior Through Donor Pride in Thailand | Journal of Nonprofit and Public Sector Marketing | [VERIFICAR] | BAJA — donación de sangre |
| 7 | Zheng, Liu, Tang & Yang, 2025 | Failed charity fundraising and strengthened benevolence | Journal of Marketing Theory and Practice | [VERIFICAR] | BAJA |
| 15 | Lawson-Body et al., 2023 | Cybersecurity and Social Media Networks for Donations | Journal of Organizational and End User Computing, 35(1) | [VERIFICAR] | BAJA — tangencial |
| 8 | Romero & Abril, 2024 | Exploring the dimensions of NGO donor-based brand equity: **A literature review** | Nonprofit Management and Leadership, 35(1) | — | **EXCLUIDO** — es una revisión, prohibida por el curso |

**Aprendizaje del cribado:** `DOCTYPE(ar)` NO eliminó el #8, porque Scopus lo clasifica como
*Article* aunque su título dice *"A literature review"*. **El filtro automático no basta: hay que
revisar título y resumen de cada resultado.**


### Ejecutada 2 — Scopus, 2026-09-06 (cadena ampliada con términos de CONVERSIÓN)

**Corrección aplicada:** la primera cadena se centraba en *retención*, pero el problema del proyecto
es de *conversión*. Se añadieron: donor acquisition, donor conversion, membership growth,
donor development, donor lifecycle, supporter journey, member conversion.

**Cadena:**
```
TITLE-ABS-KEY(("donor retention" OR "donor acquisition" OR "donor conversion" OR "donor churn"
 OR "membership retention" OR "membership growth" OR "donor development" OR "donor lifecycle"
 OR "supporter journey" OR "member conversion")
 AND (nonprofit OR "non-profit" OR charity OR philanthrop* OR fundraising OR museum
 OR "cultural institution" OR "arts organization"))
AND PUBYEAR > 2022 AND DOCTYPE(ar) AND LANGUAGE(english)
```

**Resultado: 18 documentos.**

#### Nuevos respecto a la primera cadena (8)

| Autor, año | Título | Revista | Cuartil | Valoración |
|---|---|---|---|---|
| Shekhtman & Barabási, 2023 | Philanthropy in art: locality, donor retention, and prestige | Scientific Reports, 13(1), 12157 | [VERIFICAR] | **CLAVE** — filantropía en ARTE, retención y **localidad** (geografía). Tenemos direcciones de los 1080. Barabási es referente en ciencia de redes |
| Song, Rashid, Li & Wang, 2025 | Predictive Decision Analytics for Membership Retention and Expansion in Martial Arts Organisations | Decision Making Applications in Management and Engineering, 8(2) | [VERIFICAR] | **CLAVE** — analítica predictiva para retención Y expansión de membresías. Dominio distinto, problema idéntico. Open access |
| Jensen, Kassow, Shaker & Sum, 2026 | Exploring the Role of Special Events in Relationship Fundraising | Nonprofit Management and Leadership | [VERIFICAR] | **ALTA** — el MAC capta amigos por eventos |
| Hansen & Dula, 2023 | What do you value? Examining gendered responses to appeal letters | Journal of Philanthropy and Marketing, 28(2), e1776 | [VERIFICAR] | **ALTA** — el sexo como variable de segmentación; lo tenemos de los 1080. Open access |
| Hoskins, VanEpps, Hoskins & Scammon, 2025 | How service encounters predict donor behavior: evidence from a university health system | Journal of Services Marketing, 39(4) | [VERIFICAR] | MEDIA |
| Pension, 2026 | Beyond Resource Exchange: Externalities in a Nonprofit Theater and University Partnership | Journal of Arts Management Law and Society | [VERIFICAR] | MEDIA — sector cultural |
| Morrison, Teare & Shier, 2026 | Strategic ambitions and operational realities: community sport and the 2026 FIFA World Cup | Sport Management Review | [VERIFICAR] | BAJA — fuera de tema |
| Woolum, 2023 | Striking for Victory: The Women's International Bowling Congress's World War II Effort | Journal of Sport History | [VERIFICAR] | **DESCARTAR** — historia deportiva, ruido |

#### Lección metodológica importante

**La cadena "amplia" NO fue un superconjunto de la primera.** Sinha et al. (2025) —el artículo más
relevante de todos— **no apareció** en la segunda, porque se cayeron los términos `"lapsed donor"`
y `"donor loyalty"` que lo capturaban.

> Ampliar una cadena cambiando términos **no garantiza conservar** lo que ya habías encontrado.
> Por eso hay que registrar cada cadena por separado y trabajar con la **unión** de resultados,
> nunca reemplazar una búsqueda por otra.

#### Balance acumulado

| | |
|---|---|
| Cadena 1 | 15 resultados |
| Cadena 2 | 18 resultados |
| **Únicos tras unión** | **~23** |
| Excluidos (revisión, fuera de tema) | 2 |
| **Con relevancia alta o clave** | **~10** |


### Abstracts leídos — 2026-09-06

> Datos extraídos **de los resúmenes en Scopus**, no de los textos completos.
> Antes de citar cualquiera de estas cifras en la tesis hay que **leer el artículo completo**
> y verificar el dato en la fuente. Cuartiles todavía sin verificar.

#### Hallazgos con dato citable

**Hesse (2025) — Nonprofit Management and Leadership, 36(1). Open access.**
*Using Machine Learning to Understand and Manage the Transformation of Peer Donors to Organizational Donors*
- Datos de encuesta, n = 706
- Entre donantes sin afiliación previa a la organización, la probabilidad de transformarse en
  donante organizacional es **14,1 %** (≈ 1 de cada 7)
- La comunicación posterior a la donación **triplicó** las probabilidades de transformación
- La confianza en la organización **no** mostró influencia
- **Random forest predijo la transformación con 79 % de exactitud**, superando ligeramente a la
  regresión logística
- Propósito declarado: identificar qué donantes tienen más probabilidad de transformarse para
  asignar esfuerzos de captación

→ **Es el precedente metodológico directo del proyecto.** Hace exactamente lo que proponemos:
predecir quién se convierte, para priorizar el esfuerzo.

**Shekhtman & Barabási (2023) — Scientific Reports, 13(1), 12157. Open access.**
*Philanthropy in art: locality, donor retention, and prestige*
- Dataset IRS e-file: **36 000 M USD** en subvenciones, 46 643 fundaciones → 48 766 receptores de
  arte, entre 2010 y 2019
- La donación sigue una **distribución de ley de potencias**: pocos donantes aportan mucho más
- **El 60 % de las subvenciones va a receptores del mismo estado del donante** → la donación al
  arte es fuertemente **local**
- **Cerca del 70 % de las relaciones donante-receptor continúan al año siguiente**
- El financiamiento correlaciona con el prestigio institucional

→ Respalda usar la **dirección** como variable de segmentación, y da cifras del sector arte.

**Jensen, Kassow, Shaker & Sum (2026) — Nonprofit Management and Leadership.**
*Exploring the Role of Special Events in Relationship Fundraising*
- Datos longitudinales de una fundación universitaria
- La asistencia repetida a eventos se asocia fuertemente con donar
- La intimidad del evento se asocia con donación de corto plazo, pero el efecto se atenúa
- **Los aportes mayores NO se predicen por eventos**, sino por el trato uno a uno con el personal
  y por la capacidad económica del donante

→ El MAC capta por eventos. Y esto respalda la cautela sobre las empresas (pregunta #12): los
aportes grandes no salen de eventos ni de sistemas, salen de relación individual.

**Hoskins, VanEpps, Hoskins & Scammon (2025) — Journal of Services Marketing, 39(4).**
*How service encounters predict donor behavior*
- 10 años de datos de un sistema de salud universitario
- La **frecuencia** de visitas ambulatorias predice positivamente la captación de nuevos donantes,
  la repetición y el monto
- Las visitas de emergencia u hospitalización tienen impacto **nulo o negativo**
- La tasa de respuesta a encuestas de satisfacción también predice captación

→ La relación se construye con interacciones **frecuentes y pequeñas**, no con eventos aislados.
Si el MAC registra visitas de los vecinos, sería una variable predictora fuerte.

**Hoskins & Hoskins (2024) — Journal of Philanthropy and Marketing, 29(2), e1864. Open access.**
*Age as a determinant of new donor acquisition and year-on-year retention*
- Dataset de 10 años de una universidad Research One
- Los prospectos **mayores se captan a tasas más altas** que los jóvenes
- Pero una vez captados, el efecto de la edad sobre la **retención es plano o negativo**
- Los donantes jóvenes sí tienen capacidad y voluntad de dar
- Recomienda **segmentar el mensaje por grupo etario**

→ Respalda usar la edad como variable, y matiza cómo: sirve para captar, no para retener.

#### Correcciones tras leer los resúmenes

**Song et al. (2025) — BAJA, no CLAVE.** Por el título parecía analítica predictiva de membresías.
El resumen revela que es sobre **evaluación de técnica de artes marciales** con CNN y BiLSTM para
reconocimiento de movimiento. La conexión con retención de miembros es indirecta.
→ Ejemplo de por qué **no se puede valorar un artículo por el título**.

**Hansen & Dula (2023).** Resultado **negativo**: no encontraron mejora significativa en la
respuesta a cartas de captación al alinear el mensaje con valores por género. Útil precisamente
por eso: advierte contra segmentar el mensaje solo por sexo.

**Chell et al. (2023) — Australasian Marketing Journal, 31(1).**
El reconocimiento en línea (insignia digital compartible) fortalece la identidad del donante
frente a un correo de agradecimiento privado, y mejora la retención.
→ Conecta directamente con el problema del **carnet digital** del MAC.

**Samek & Longfield (2023) — American Economic Journal: Applied Economics, 15(2).**
Experimento de campo con **500 000 donantes nuevos**. Los profesionales de captación predijeron
que las llamadas de agradecimiento aumentarían la retención en un **80 %**. El resultado fue un
**efecto nulo**, medido con precisión.
→ Argumento potente: la intuición de los expertos falla. Hace falta decidir con datos.

**Woolum (2023) — DESCARTAR.** Historia del bowling femenino en la Segunda Guerra Mundial.
**Morrison et al. (2026) — DESCARTAR.** Mundial FIFA 2026 y clubes deportivos comunitarios.

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
