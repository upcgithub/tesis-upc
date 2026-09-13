# Búsqueda: pronóstico de afluencia de visitantes en museos

- **Fecha:** 2026-09-13 · **Base:** Scopus (proxy UPC)
- **Tema:** MAC Anticipa — sistema predictivo de afluencia de visitantes con series temporales
  y aprendizaje automático para museos con datos limitados

## Cadenas ejecutadas

### Cadena 1 — amplia (descartada por ruido)

```
TITLE-ABS-KEY(("visitor forecasting" OR "visitor prediction" OR "attendance forecasting"
 OR "attendance prediction" OR "visitor demand" OR footfall OR "visitor arrival*"
 OR "visitor flow") AND (museum* OR "cultural institution*" OR "cultural heritage"
 OR gallery OR "heritage site*"))
AND PUBYEAR > 2022 AND DOCTYPE(ar) AND LANGUAGE(english)
```
**49 resultados.** Demasiado ruido: capturaba diseño de exposiciones e impacto económico del
turismo, porque `"visitor flow"` y `footfall` son muy generales sin exigir método predictivo.

### Cadena 2 — refinada ✅ la buena

```
TITLE-ABS-KEY((forecast* OR predict*) AND (visitor* OR attendance OR footfall)
 AND (museum* OR "cultural institution*" OR "heritage site*" OR "cultural tourism")
 AND ("machine learning" OR "deep learning" OR "time series" OR "neural network*"
      OR ARIMA OR LSTM))
AND PUBYEAR > 2022 AND DOCTYPE(ar) AND LANGUAGE(english)
```
**24 resultados**, los 24 de tipo Article. Añadir la exigencia de método predictivo
(`"machine learning" OR ... OR ARIMA OR LSTM`) fue lo que eliminó el ruido.

## Cribado

| Etapa | N |
|---|---|
| Identificados (cadena 2) | 24 |
| Descartados por tema | 10 |
| Descartados por revista sin cuartil verificable | 4 (pendiente confirmar) |
| **Candidatos con relevancia alta o clave** | **6** |
| Ya conocidos del sustento | 1 (Tian 2025, PLOS ONE) |

### Cuartiles verificados en SCImago — 2026-09-13

| Revista | Año del artículo | Cuartil | ¿Cumple? |
|---|---|---|---|
| Journal of Outdoor Recreation and Tourism | 2023 | **Q2** · Tourism, Leisure & Hospitality Mgmt *(subió a Q1 en 2024-2025)* | ✅ |
| Sustainability (Switzerland) | 2023 | **Q1** · Geography, Planning & Development | ✅ |
| PLOS ONE | 2025 | **Q1** · Multidisciplinary · SJR 0,726 | ✅ |
| **ShodhKosh: Journal of Visual and Performing Arts** | 2025 | **sin SJR y sin cuartil** · H-index 1 | ❌ |
| Scientific Reports | 2025 | [VERIFICAR] | — |
| Journal of Tourism Futures | 2026 | [VERIFICAR] | — |
| Innovative Infrastructure Solutions | 2026 | [VERIFICAR] | — |
| International Journal of Tourism Research | 2026 | [VERIFICAR] | — |

---

## Candidatos CLAVE

### 1. Madden, Lukoseviciute, Ramsey, Panagopoulos & Condell (2023)
**Forecasting daily foot traffic in recreational trails using machine learning**
*Journal of Outdoor Recreation and Tourism*, 44, 100701 · 11 citas · Cuartil [VERIFICAR]

Pronostica **afluencia DIARIA** con aprendizaje automático, usando datos históricos de sensores
de conteo electrónico junto con datos meteorológicos. Introduce por primera vez los *Tourism
Climate Indexes* en modelos de pronóstico. Tres senderos del área atlántica de Europa.

→ **Es el único de todo el corpus que trabaja el horizonte diario**, que es justo el que propone
MAC Anticipa. El dominio (senderos, no museos) es su limitación, pero metodológicamente es el
precedente más cercano. También aporta la idea de variables meteorológicas como regresores.

### 2. Tian, Wang, Tan, Na & Kim (2025)
**Utilizing unstructured data to predict the art museum visitor numbers using deep learning approaches**
*Scientific Reports*, 15(1), 41684 · Open Access · Cuartil [VERIFICAR]

Predice el número de visitantes de **museos de ARTE** combinando datos estructurados con datos
textuales no estructurados de sitios web y contenido de visitantes, procesados con PLN. Evalúa
**ocho arquitecturas** de aprendizaje profundo (Transformer, LSTM, CNN, GAN, entre otras);
el **Transformer** obtuvo el mejor desempeño. Propone además un Balanced Scorecard adaptado a
museos con cuatro dimensiones estratégicas.

→ **El escenario más cercano: museos de arte.** El MAC es un museo de arte contemporáneo.
Mismo primer autor que el Tian et al. (2025) de PLOS ONE ya citado en el sustento.

### 3. Budak & Yayla (2026)
**A rolling-origin ensemble forecasting framework for tourism revenue: elastic net and CatBoost — the case of Türkiye (2002–2024)**
*Journal of Tourism Futures* · Article in Press · Cuartil [VERIFICAR]

Marco de pronóstico con **validación rolling-origin (ventana expansiva)**, comparando Elastic Net
y CatBoost contra un **ARIMA de referencia**. Elastic Net obtuvo el mejor desempeño fuera de
muestra (R² = 0,894; RMSE = 4,02; MAE = 2,80) y el ARIMA(2,1,2) quedó sustancialmente por debajo.
Usa **valores SHAP** para interpretabilidad. Entre los predictores dominantes están los
**visitantes a museos**.

→ **Es el plano metodológico del proyecto**: validación temporal con origen móvil, comparación
contra un modelo de referencia, y explicabilidad con SHAP. Exactamente los tres pilares de
MAC Anticipa.

### 4. Ababneh, Ababne & Romani Sala (2026)
**Predicting visitors to Jerash using ARIMA and the impact of visitors on the integrity of the Hadrian's Arch structure**
*Innovative Infrastructure Solutions*, 11(6), 301 · 2 citas · Cuartil [VERIFICAR]

Usa **ARIMA** para predecir visitantes a un sitio patrimonial a seis años vista. El modelo
seleccionado fue un **ARIMA(0,2,1) no estacional sobre datos anuales**. Dato relevante:
*"Monthly data and seasonal models were also analyzed, but the seasonal models did not
demonstrate success."* Vincula el pronóstico con la gestión de riesgo y capacidad de carga.

→ Precedente en método clásico sobre patrimonio. **Y una advertencia útil:** en su caso los
modelos estacionales mensuales fracasaron. Conviene tenerlo presente al elegir el modelo de
referencia estacional del proyecto.

---

## Candidatos de apoyo

### 5. Castellana et al. (2024)
**Exploring Apulia's Regional Tourism Attractiveness through the Lens of Sustainability: A Machine Learning Approach and Counterfactual Explainability Process**
*Sustainability*, 16(15), 6287 · 4 citas · Cuartil [VERIFICAR] *(Sustainability fue Q1/Q2 en 2023)*

Red neuronal artificial para predecir el flujo turístico entrante en Apulia, con selección de
modelo por RMSE. Aplica un modelo **contrafactual multiobjetivo (MOC)** y el gráfico de
importancia de variables de Garson.

→ Aporta a la parte de **explicabilidad**: importancia de variables y análisis contrafactual.

### 6. Masini, Bacci, Petrucci, Francini & Bertaccini (2026)
**A Visitor-Centric Recommender System for Florentine Museums**
*International Journal of Tourism Research*, 28(4), e70407 · Cuartil [VERIFICAR]

Sistema de recomendación con arquitectura de dos torres sobre datos de la FirenzeCard.
Menciona como capa superior un agente de aprendizaje por refuerzo para **gestionar flujos de
visitantes y aliviar la aglomeración**.

→ Relevancia media: es recomendación, no pronóstico de afluencia. Útil como contexto de
gestión de flujos en museos.

---

## Descartados

| # | Motivo |
|---|---|
| Lai, Tian & Zhang (2026) — índice de sentimiento en imágenes de patrimonio | Sentimiento, no afluencia |
| Wu et al. (2026) — detección de caídas con YOLOv11 en galería | Seguridad, no afluencia |
| Wang et al. (2026) — modelo antiempañamiento de vitrinas | Conservación |
| Tian, You & Wang (2026) — GazeNet, simulación de atención visual | Diseño de exposición |
| Luo (2026) — comportamiento de turistas con GNN | Comportamiento individual, no afluencia agregada |
| Nie (2025) — LSTM para interés de visitantes | Recomendación |
| Li & Liu (2025) — random forest para tours adaptativos | Recomendación |
| Philippopoulos et al. (2025) — posicionamiento RSSI interior | Localización |
| Yao et al. (2025) — retrofit bajo en carbono de museos | Eficiencia energética |
| Sharpe et al. (2025) — cámaras trampa y ciencia ciudadana | Fuera de tema |
| Crettaz von Roten (2024) — audiencias de divulgación científica | Fuera de tema |
| Hou & Paidi (2025) — comportamiento turístico Gran Muralla | Segmentación, no pronóstico |
| Feng, Wang & Zou (2024) — Gran Canal, satisfacción de visitantes | Satisfacción, no afluencia |

### ⚠️ Revista a verificar antes de usar

**Shodhkosh Journal of Visual and Performing Arts** aparece **cuatro veces** (#9, #10, #11, #12),
todas de 2025 y todas sobre analítica predictiva en instituciones culturales:

- *Managing contemporary art institutions with predictive insights* — el título más cercano
  al escenario de todo el corpus
- *Predicting exhibition success with neural networks*
- *Predictive analytics for photo exhibition planning*
- *Intelligent systems for digital exhibition design*

**❌ VERIFICADO Y DESCARTADO (2026-09-13).** La revista figura en SCImago —India,
Granthaalayah Publications and Printers, categoría Visual Arts and Performing Arts— pero
**no tiene valor SJR ni cuartil asignado**, y su **H-index es 1**. Donde Sustainability o
PLOS ONE muestran su tarjeta «SJR · Q1», esta revista simplemente no la tiene.

Sin cuartil, **los cuatro artículos quedan fuera del estado del arte** por criterio del curso
(Q1 o Q2, revista indexada).

Es una lástima: *Managing contemporary art institutions with predictive insights* tenía el título
más cercano al escenario del MAC de todo el corpus. Pero la sospecha inicial —cuatro artículos
casi idénticos, misma revista, mismo año, cero citas— resultó fundada.

> **Aprendizaje:** un resultado puede aparecer en Scopus y aun así no cumplir el criterio.
> Estar indexado en Scopus y tener cuartil SJR son cosas distintas.

---

## Lo que este corpus dice sobre la brecha

Ninguno de los 24 hace lo que propone MAC Anticipa:

| Trabajo | Horizonte | Unidad | Escenario |
|---|---|---|---|
| Madden et al. (2023) | **diario** ✓ | senderos recreativos | Europa atlántica |
| Tian et al. (2025) *Sci Rep* | anual | museos de arte ✓ | panel |
| Tian et al. (2025) *PLOS ONE* | anual | museos ✓ | 323 museos coreanos |
| Ababneh et al. (2026) | anual | sitio patrimonial | Jerash |
| Bravo et al. (2023) | mensual | atractivos turísticos | Ruta Moche, Perú |
| Budak & Yayla (2026) | anual | ingresos turísticos | Türkiye |

**El cruce vacío: horizonte diario o semanal × una sola institución pequeña × datos limitados y
registro manual.** Eso es exactamente lo que ocupa el proyecto, y ahora está documentado.

## Pendientes de esta búsqueda

1. Verificar cuartiles en SCImago de las 6 revistas candidatas
2. Verificar el cuartil de *Shodhkosh* y decidir si sus 4 artículos entran o se descartan
3. Ejecutar la misma cadena en **Web of Science** — indexa distinto y puede traer otros
4. Ampliar hacia pronóstico con series cortas y datos limitados, que es la parte de la brecha
   que aún no tiene respaldo
