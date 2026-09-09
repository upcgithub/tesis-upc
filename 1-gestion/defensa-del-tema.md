# Defensa del tema ante el asesor

> Preparación para la reunión con el MBA Ing. Julio César Zácari Ramos.
> Mapea cada decisión del tema contra el criterio exacto del material oficial del curso,
> y lista los puntos débiles con su respuesta preparada.
>
> Fuentes: `U1-S1-1. Tesis, Investigación y Tema.pdf` · `_Lineamientos cursos Capstone 2026-25 (SIA-PI1).pdf`
> · `_Plan de Trabajo de Investigación (Entrega Semana 2).docx`

**Tema:** Sistema de gestión y priorización de prospectos de aporte con segmentación analítica
para museos privados sin fines de lucro
**Escenario:** Museo de Arte Contemporáneo de Lima (MAC), programa *Amigos del MAC*

---

## Parte A — Cómo el tema cumple cada criterio

### A.1 Las cuatro preguntas del tema

> *"El tema de tesis se refiere a: ¿Qué se desea resolver? → Problema. ¿Qué se propone para
> resolver? → Aporte. ¿Con qué se pretende resolver? → Técnica. ¿Dónde se probará la propuesta?
> → Escenario."* — U1-S1-1

| Pregunta | Nuestra respuesta | Verificación del requisito |
|---|---|---|
| ¿Qué se desea resolver? | Baja conversión de miembros no aportantes en aportantes, y gestión manual sin trazabilidad del aporte | *"Debe ser de interés por algún sector empresarial, gubernamental, social, científico, ingenieril"* → sector cultural sin fines de lucro |
| ¿Qué se propone? | Sistema de gestión con modelo de segmentación analítica que prioriza prospectos | *"Debe corresponder a la carrera de Ing. de Sistemas"* → sistema de información con componente analítico |
| ¿Con qué? | Analítica de datos, segmentación no supervisada, enriquecimiento con datos públicos, CRISP-DM | *"Debe corresponder a Tecnologías de Información"* → línea **Datos: Business Intelligence, Data Analytics, Minería de Datos, Data Science** de los lineamientos |
| ¿Dónde se validará? | MAC Lima, programa Amigos del MAC | *"El escenario debe ser representativo"* → museo privado sin fines de lucro con programa de membresía |

**Frase de defensa:** *"El tema responde las cuatro preguntas del material: qué resolvemos, qué
proponemos, con qué técnica, y dónde lo validamos. Ninguna quedó abierta."*

### A.2 La fórmula del título

> *"[Aporte] para solucionar [Problema] usando [Técnica] a ser validado en [Contexto o escenario]"*

Desglose del título propuesto:

```
Sistema de gestión y priorización de prospectos de aporte   ← APORTE
con segmentación analítica                                   ← TÉCNICA
para museos privados sin fines de lucro                      ← CLASE DE ESCENARIO
```

El escenario concreto (MAC) va en el cuerpo, no en el título, **a propósito** — ver A.4.

### A.3 Las cuatro características de validez

> U1-S1-1: *"La Tesis: Características (Para ser válidas)"*

**ORIGINALIDAD** — *"No puede haber dos tesis iguales: con el mismo problema, la misma propuesta,
la misma técnica y el mismo escenario"*

La combinación problema (conversión de miembros no aportantes) × propuesta (sistema con
segmentación) × técnica (segmentación no supervisada con enriquecimiento externo) × escenario
(museos privados sin fines de lucro) no aparece en la literatura revisada. La búsqueda en Scopus
sobre el cruce museos × analítica × donantes devuelve muy pocos resultados, y eso está registrado
en `2-fuentes/busquedas/`.

**APORTE** — *"Es la contribución de la aplicación, adaptación o mejora del conocimiento... La
propuesta debe tener novedad y mejores resultados que la literatura"*

Se **adapta** un conocimiento existente —modelos de segmentación y predicción de conversión de
donantes— a un dominio donde no se ha aplicado: museos con base amplia de miembros sin aporte.
Precedente metodológico: Hesse (2025) logra 79 % de exactitud prediciendo conversión de donantes
con random forest, en un dominio distinto.

**PROFUNDIDAD** — *"La tesis de grado corresponde a la aplicación o adaptación de un conocimiento
para poder resolver un problema"*

Es exactamente aplicación y adaptación, que es el nivel que el documento exige para el grado de
ingeniero. No se pretende conocimiento nuevo de frontera.

**VALIDACIÓN** — *"El aporte alcanza los objetivos, resuelve el problema, mejora resultados
(costos, tiempo, eficiencia, otros)"*

Se validará contra líneas base medibles del propio escenario. La más sólida y ya conocida:
la emisión de una credencial digital toma **2 días** de forma manual.

**SOSTENIBILIDAD** — *"El aporte se debe mantener en el tiempo, argumentado (Teorías, razonamiento
lógico, trabajos previos), sustentado en fuentes válidas"*

El modelo se sostiene sobre literatura indexada, no sobre intuición. Y el sistema queda operable
por el propio museo, sin dependencia del equipo de tesis.

### A.4 La abstracción del problema

> *"El problema en lo posible debe ser abstraído de la organización. El aporte se hace para
> resolver el problema independientemente de la organización."*
> *"La solución propuesta servirá para todas las organizaciones similares que tengan ese problema.
> → Se crea un mercado para el aporte."*

**Cómo se cumplió, en concreto:** el título dice *"museos privados sin fines de lucro"*, no
*"el MAC"*. El MAC es el escenario **de validación**, no el objeto de la tesis.

**Y hubo una decisión deliberada aquí que conviene explicar si pregunta.** Se evaluó decir
*"instituciones culturales"* (más amplio) y se acotó a *"museos privados"*, por dos razones:

1. Los museos comparten el modelo de "Amigos del museo" —membresía anual con beneficios— que es
   justo lo que se modela. Un teatro tiene abonados a temporada; una orquesta, suscripciones.
   La relación con el donante es estructuralmente distinta.
2. Validando en un solo museo, afirmar aplicabilidad a toda institución cultural sería una
   sobreafirmación difícil de sostener.

**Frase de defensa:** *"Acotamos la clase de organización para que la afirmación sea defendible
con una sola validación, no para reducir el trabajo — el trabajo es el mismo."*

### A.5 Factibilidad

> U1-S1-1: *"El escenario lo requiere (Negocio) · Puede ser usado/operado por el escenario
> (Organización) · Se va a contar con la infraestructura TI · Contar con el presupuesto"*
> Lineamientos: *"Información real disponible para: el análisis de la situación problemática; el
> desarrollo o elaboración de la solución; la validación de la solución terminada en un escenario real"*

| Requisito | Estado |
|---|---|
| El escenario lo requiere | Sí. Los ingresos por taquilla no cubren la operación y los aportes son necesarios para funcionar |
| Puede operarlo la organización | Sí. El área de crecimiento del museo es la que hoy hace el proceso a mano |
| Información para el **análisis** | Sí. Padrón de 1 080 miembros con antigüedad, edad, sexo y dirección; registro de aportantes desde 2023 |
| Información para el **desarrollo** | Sí. Los mismos datos, más la correspondencia de aportes |
| Información para la **validación** | Sí. Las renovaciones son por aniversario, distribuidas todo el año, así que hay casos dentro de la ventana de PI-2 |
| Acceso real | Sí. Una integrante del equipo trabaja en el área de crecimiento del museo |
| Usuario especialista | En gestión. Se está tramitando la conformidad de un gerente del museo |

**Este es el punto más fuerte de la propuesta.** La factibilidad suele ser lo que hunde estos
proyectos, y aquí está resuelta con acceso directo.

### A.6 De dónde salió la idea

> *"Algunas fuentes para ideas de investigación: Problemas en la sociedad · Documentos ·
> Experiencias individuales y colectivas · **Observación de hechos**"*

La idea salió de la **observación directa de un hecho**: el proceso manual por correo que una
integrante del equipo ejecuta y padece. Es una de las fuentes que el material lista expresamente.

### A.7 Las preguntas de investigación estructuran el sustento

> El material plantea cuatro: **¿Qué? ¿Para qué o quiénes? ¿Dónde? ¿Cómo?**

El sustento del Plan de Trabajo está literalmente organizado con esas cuatro preguntas como
subsecciones. No es una redacción libre: sigue el instrumento del curso.

Y sobre *"Buscar información cuantitativa relevante que justifique la importancia del problema"*:
el dato ancla es primario y del escenario — **1 conversión en 1 080 miembros desde 2023,
equivalente a 0,09 %**.

### A.8 Objetivos SMART y la estructura de cuatro

> Lineamientos: *"Los objetivos deben estar alineados a Objetivos SMART"* y *"Se sugiere que sean
> enmarcados en 4 objetivos específicos orientados a entregables medibles... Obtener los resultados
> o diagnóstico del análisis · Diseñar · Construir/desarrollar/implementar · Validar"*

| # | Nuestro objetivo | Verbo del ejemplo oficial | Estructura sugerida |
|---|---|---|---|
| 1 | **Determinar** el diagnóstico de la situación actual | *Determinar* | Diagnóstico del análisis |
| 2 | **Diseñar** el modelo de segmentación y la arquitectura | *Diseñar* | Diseñar la propuesta |
| 3 | **Elaborar** el sistema aplicando el modelo | *Elaborar* | Construir/desarrollar |
| 4 | **Verificar** el cumplimiento de los indicadores | *Verificar* | Validar la solución |

Los cuatro verbos son **los mismos del ejemplo oficial** del PDF (modelo de seguridad con
blockchain y PLN), y la secuencia es la que sugieren los lineamientos.

### A.9 La técnica pertenece a las líneas admitidas

> Lineamientos, sección III: *"Datos: Business Intelligence, Data Analytics, Big Data, Minería de
> Datos, Data Science"*

La segmentación analítica con enriquecimiento de datos externos cae de lleno en la línea **Datos**.
No es una técnica traída de otra disciplina que haya que justificar.

### A.10 El método de elaboración

> Lineamientos, sección II: *"a. Desarrollo de Soluciones – Ágil – Cascada"*

Se opta por **Desarrollo de Soluciones**, porque hay construcción de software. Los lineamientos
piden además, para casos con modelos: *"Extracción y análisis de las características de datos, que
permitan la preparación de la información para entrenamiento... entrenamiento y verificación del
modelo"*, y que *"las historias de usuario o casos de uso deberán hacer referencia al modelo cuando
lo utilicen"*. El diseño lo contempla.

---

## Parte B — Los puntos débiles, y cómo responderlos

> Léelos antes de la reunión. Si los planteas tú primero, ganas credibilidad;
> si los saca él y no tienes respuesta, la pierdes.

### B.1 «¿Por qué no compran un CRM comercial?»

**Es la pregunta más probable y la más peligrosa.** Salesforce Nonprofit Cloud, DonorPerfect y
Bloomerang existen y son productos maduros.

**Respuesta honesta:** el aporte de la tesis **no es el CRM**. Es el modelo de segmentación que
prioriza prospectos dentro de una base de miembros que **nunca han aportado**, usando solo
variables demográficas. Los CRM comerciales gestionan la relación con donantes **existentes**;
no resuelven a quién de 1 080 personas sin historial de donación conviene dirigirse.

**Estado real:** este argumento todavía **no está respaldado con literatura**. Está pendiente
como hueco #4 del sustento. Si el asesor insiste, lo honesto es decir que se está construyendo
la evidencia, no improvisar.

### B.2 «¿Segmentar 1 080 registros con 5 variables es aporte suficiente?»

Es la pregunta #12 de `preguntas-abiertas.md`, y conviene **plantearla tú mismo**.

**Argumentos a favor:** Sinha et al. (2025), en *Journal of Business Research*, aborda exactamente
si se pueden usar perfiles comunitarios como alternativa al historial de donación. Shekhtman &
Barabási (2023) muestran que el 60 % de la filantropía en arte es local, lo que da fundamento a
usar la dirección. Hoskins & Hoskins (2024) validan la edad como predictor de captación.

**Refuerzo previsto:** enriquecer la dirección con datos socioeconómicos públicos por distrito,
lo que añade dimensiones sin depender de datos que el museo no tiene.

### B.3 Con una sola conversión histórica no hay aprendizaje supervisado

**Dilo tú antes de que lo pregunte.** Con 1 caso positivo en 1 080 no se puede entrenar un
clasificador supervisado. Por eso la técnica es **segmentación no supervisada**, que no requiere
casos etiquetados.

Que hayas descartado el aprendizaje supervisado por una razón técnica correcta demuestra criterio.

### B.4 La muestra de aportantes es pequeña

30 aportantes —25 personas y 5 empresas— es poco para cualquier análisis estadístico sobre
**aportantes**. Por eso el eje del proyecto son los **1 080 no aportantes**, donde sí hay volumen.

### B.5 Los aportes son anuales y la validación dura 4 meses

Riesgo real de que no se pueda medir nada. **Mitigación:** las renovaciones son por aniversario,
no todas en la misma fecha, así que en cuatro meses vencen alrededor de un tercio. Y los
indicadores principales son de proceso —tiempo de emisión de credencial, trazabilidad,
completitud de datos— que se miden en semanas.

### B.6 El sustento aún no tiene datos citables del museo

Los lineamientos exigen *"información primaria cuantitativa referenciada"*. Los números del MAC
son primarios pero **todavía no hay documento que los respalde**. Está pendiente y es tarea del
equipo conseguirlo del museo.

### B.7 Las empresas: alcance por definir

Ver pregunta #12. Hay título de repliegue preparado si el asesor considera que la prospección
corporativa no es viable. Y hay un dato de la literatura que respalda su cautela: Jensen et al.
(2026) encuentran que los aportes mayores **no** se predicen por eventos ni sistemas, sino por
trato uno a uno y capacidad económica del donante.

---

## Parte C — Lo que NO puedes afirmar todavía

Decir de más aquí es lo que más rápido destruye la credibilidad.

| No afirmes | Porque |
|---|---|
| Que tal artículo es Q1 o Q2 | **Ningún cuartil está verificado** en SCImago todavía |
| Cifras del sector museos | La capa 1 de búsqueda no se ha ejecutado |
| Que la conversión del MAC (0,09 %) es peor que el 14,1 % de la literatura | **No son poblaciones comparables**: los de Hesse ya habían donado una vez |
| Que el modelo alcanzará cierta exactitud | No hay datos procesados todavía |
| Que un CRM comercial no sirve | Aún sin respaldo en literatura |

---

## Parte D — Preguntas para hacerle tú

Llevar preguntas propias demuestra preparación. Las cuatro con más impacto:

1. **¿Segmentar 1 080 registros con variables demográficas es aporte suficiente, o espera mayor profundidad técnica?** (pregunta #12)
2. **¿Incluimos la prospección de empresas como objetivo secundario con validación por experto, o acotamos solo a la conversión de miembros?** (#12)
3. **¿Confirma el enfoque de Desarrollo de Soluciones con método ágil?** (#11)
4. **¿Hay formato oficial para el informe de análisis de artículos de la semana 6?** (#3)

Y las administrativas, que tienen plazo encima: el canal de entrega de las dos cartas (#7) y el
Site del Proyecto con su código (#8), que vencen en la **semana 3**.
