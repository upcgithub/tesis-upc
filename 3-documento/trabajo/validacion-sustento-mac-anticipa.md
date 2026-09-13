# Validación del sustento — MAC Anticipa

Verificación del documento `Plan_de_Trabajo_Investigacion_MAC_Anticipa_Semana_2.docx`
realizada el **2026-09-13** contra las fuentes primarias.

**Método:** cada referencia se buscó por DOI en Scopus (proxy UPC), se leyó el resumen en el sitio
del editor, y se verificó el cuartil en SCImago para el año de publicación del artículo.
El informe del Ministerio de Cultura se descargó y se buscaron las cifras en el texto.

---

## Resumen

| | |
|---|---|
| Referencias verificadas | **5 de 5** |
| Referencias inexistentes o con datos falsos | **0** |
| Artículos que cumplen Q1/Q2 | **2 de 2** |
| Afirmaciones sobre los artículos que son correctas | **3 de 3** |
| Imprecisiones detectadas | **2** |
| Riesgos de criterio | **3** |

**Veredicto: el sustento es sólido.** No hay ninguna referencia inventada ni ninguna cifra
falsa. Las dos imprecisiones son menores y se corrigen con una frase cada una.

---

## 1. Referencias verificadas

### ✅ Bravo, Alarcón, Valdivia & Serquén (2023)

| | |
|---|---|
| Título | Application of Machine Learning Techniques to Predict Visitors to the Tourist Attractions of the Moche Route in Peru |
| Autores | Jessie Bravo, Roger Alarcón, Carlos Valdivia, Oscar Serquén — Universidad Nacional Pedro Ruiz Gallo, Lambayeque, Perú |
| Publicación | *Sustainability*, 2023, 15(11), 8967 |
| DOI | 10.3390/su15118967 — **resuelve correctamente** |
| Tipo | **Article** · Open Access · 24 citas en Scopus |
| Indexado en Scopus | **Sí** |
| **Cuartil 2023 (SJR)** | **Q1 en Geography, Planning and Development** · Q2 en las otras 6 categorías |
| **¿Cumple el criterio del curso?** | **Sí** — ≤3 años (2023), Q1, artículo de aporte, revista indexada |

**Verificación de la afirmación del sustento:**

> *"Bravo et al. (2023) compararon regresión lineal, KNN, árbol de decisión y random forest para
> predecir visitantes en la Ruta Moche con datos peruanos; la regresión lineal obtuvo el mejor
> desempeño en su conjunto de datos."*

El resumen dice textualmente: *"Four algorithms are evaluated: linear regression, KNN regression,
decision tree, and random forest"* y *"for both the prediction of national and foreign tourists,
the best algorithm is linear regression"*.

**✅ La afirmación es exacta.**

*Dato adicional útil:* usó datos públicos oficiales más TripAdvisor y Google Trends, de enero 2011
a mayo 2022.

### ✅ Tian, Wang, Wang & Lee (2025)

| | |
|---|---|
| Título | Enhancing museum visitor forecasting using deep learning and sentiment analysis: A transformer-based approach for sustainable management |
| Autores | Ziyi Tian, Xiao Wang, Yan Wang, Jae Ho Lee |
| Publicación | *PLOS ONE*, 2025, 20(11), e0335623 |
| DOI | 10.1371/journal.pone.0335623 — **resuelve correctamente** |
| Tipo | **Article** · Open Access · 2 citas en Scopus |
| Indexado en Scopus | **Sí** |
| **Cuartil 2025 (SJR)** | **Q1** en Multidisciplinary · SJR 0.726 · H-index 500 |
| **¿Cumple el criterio del curso?** | **Sí** |

**Verificación de la afirmación del sustento:**

> *"Tian et al. (2025) evaluaron siete algoritmos para museos e informaron que la integración de
> datos estructurados y variables externas puede mejorar la precisión."*

El resumen confirma **siete algoritmos**: Linear Regression, Random Forest, RNN, GAN, CNN, LSTM y
Transformer. Y que *"incorporating sentiment data significantly enhances forecasting precision"*.

**✅ La afirmación es correcta**, pero omite información importante → ver imprecisión #2.

### ✅ Ministerio de Cultura del Perú (2025). Memoria Anual 2024

| | |
|---|---|
| URL | Resuelve correctamente · PDF de **206 páginas** |
| Ubicación de los datos | **Tabla 22**, pág. ~64 |

**Verificación de las cifras, una por una:**

| Dato del sustento | En el documento | ✓ |
|---|---|---|
| 56 museos | *"Actualmente, el Ministerio de Cultura cuenta con 56 museos a nivel nacional"* | ✅ |
| 1 787 261 visitas | `TOTAL … 1,787,261 … 100.0%` | ✅ |
| 57,6 % adultos | `Adulto … 1,029,760 … 57.6%` | ✅ |
| 25,7 % niños | `Niño … 459,717 … 25.7%` | ✅ |

**Las cuatro cifras son exactas.**

### ✅ Hyndman & Athanasopoulos (2021)

3.ª edición, prefacio de mayo de 2021, OTexts. **No existe 4.ª edición.**
La versión en línea se actualiza de forma continua — última actualización registrada: 23/07/2026.
→ Ver riesgo #1.

### ⚠️ Museo de Arte Contemporáneo de Lima (2026)

Citado como *"Registros internos de visitantes y descripción del proceso de consolidación
[Base de datos y comunicación interna no publicadas]"*.

**No verificable externamente** — es dato primario, y así debe ser. Pero es el mismo pendiente de
siempre: hace falta un documento del museo que lo respalde. → Ver riesgo #3.

---

## 2. Imprecisiones a corregir

### ⚠️ #1 — «los 56 museos registraron 1 787 261 visitas»

**Dice el sustento:**
> *"En 2024, los 56 museos administrados por el Ministerio de Cultura registraron 1 787 261 visitas"*

**Dice la fuente**, al pie de la Tabla 22:
> *"Fuente: OGETIC - Infocultura. Datos corresponden a **Museos y Salas de Exposición**."*

La cifra de visitas cubre **museos y salas de exposición**, no solo los 56 museos. Son dos datos
distintos del informe que el sustento fusionó en una sola frase.

**Corrección sugerida:**
> *"En 2024, los museos y salas de exposición del Ministerio de Cultura registraron 1 787 261
> visitas, de las cuales el 57,6 % correspondió a adultos y el 25,7 % a niños. El Ministerio
> administra 56 museos a nivel nacional (Ministerio de Cultura, 2025)."*

### ⚠️ #2 — Lo que el sustento omite de Tian et al.

El resumen dice tres cosas que el sustento no menciona y que **cambian la lectura**:

| Lo que dice el paper | Por qué importa |
|---|---|
| El modelo ganador fue el **Transformer** | El sustento no lo dice. Es un modelo complejo, no un método simple |
| Los datos son un **panel de 323 museos coreanos** (2023), con predicción **anual** | **MAC Anticipa propone predicción diaria o semanal de UN museo.** No es el mismo problema |
| Las "variables externas" son específicamente **análisis de sentimiento** de noticias y comentarios de usuarios | El sustento lo generaliza a "variables externas", que es más vago |

**Esto no invalida la cita — la refuerza.** Que nadie haga pronóstico de horizonte corto para un
solo museo pequeño **es parte de la brecha**. Pero hay que decirlo explícitamente, no dejar que
parezca que Tian resuelve el mismo problema.

**Sugerencia:** añadir una frase del tipo *"…aunque su unidad de análisis es el total anual de un
panel de 323 museos, no la serie diaria o semanal de una sola institución."*

### ✅ Una inferencia que sí está bien hecha

> *"Ambos estudios respaldan la comparación empírica de modelos, pero también indican que la
> técnica ganadora depende de los datos disponibles."*

**Correcto y bien fundamentado:** en Bravo ganó la regresión lineal (modelo simple); en Tian ganó
el Transformer (modelo complejo). Dos ganadores distintos en dos conjuntos de datos distintos.
La conclusión se sostiene.

---

## 3. Riesgos de criterio

### ⚠️ #1 — Hyndman está en el límite de antigüedad

El criterio para libros es **≤ 5 años**. La 3.ª edición es de **2021**, o sea exactamente 5 años.
Está en el borde.

**A favor de mantenerlo:** es la referencia estándar mundial en pronóstico de series temporales,
y la versión en línea se actualiza continuamente (última: julio de 2026).
**Riesgo:** si el asesor cuenta estricto, queda fuera.

**Mitigación:** citar la versión en línea con fecha de consulta, o reforzar con un artículo
reciente de metodología de pronóstico.

### ⚠️ #2 — Solo hay 2 artículos científicos

Para el Plan de Trabajo de la semana 2 puede bastar. Pero el estado del arte necesita **24**, y
ninguno de los 23 que se encontraron para el tema anterior sirve: eran sobre retención de donantes.

**Hay que rehacer la búsqueda completa** para el tema nuevo.

### ⚠️ #3 — Los datos del MAC siguen sin documento citable

*"superan los 45 000 visitantes anuales y alrededor de 8 000 participaciones en actividades
públicas gratuitas"* están citados como comunicación interna no publicada. Es admisible en APA,
pero los lineamientos piden *"información primaria cuantitativa referenciada"* y el asesor puede
pedir evidencia.

---

## 4. Lo que el sustento hace bien y conviene conservar

Dos frases destacan por su honestidad epistémica, y son justo lo que un jurado valora:

> *"La frecuencia real de errores de registro todavía no ha sido medida y se evaluará en el
> diagnóstico."*

> *"El proyecto no afirmará pérdidas económicas ni errores de dotación sin medirlos; comprobará
> primero la variabilidad de la serie y el error de métodos de referencia."*

Declarar lo que **no** se va a afirmar sin medir es una señal de rigor. No lo quiten.

---

## 5. Acciones

| # | Acción | Prioridad |
|---|---|---|
| 1 | Corregir la frase de los 56 museos (imprecisión #1) | Alta — es un error factual |
| 2 | Añadir el matiz sobre la unidad de análisis de Tian (imprecisión #2) | Alta |
| 3 | Conseguir documento citable del MAC | Alta — depende de terceros |
| 4 | Rehacer la búsqueda de literatura para el tema nuevo | Alta — hacen falta 24 artículos |
| 5 | Decidir qué hacer con Hyndman (mantener, citar en línea, o reforzar) | Media |
