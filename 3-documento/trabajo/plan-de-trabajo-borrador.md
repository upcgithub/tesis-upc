# Plan de Trabajo de Investigación — BORRADOR

> **Esto no es el entregable.** Es el borrador de contenido para revisar antes de volcarlo al
> formato oficial `plan-de-trabajo-investigacion.docx`.
>
> **Marcas:** `[DATO PENDIENTE]` = falta un número real · `[FUENTE PENDIENTE]` = falta la cita.
> Nada de esto se rellena con cifras plausibles: o el dato está verificado, o queda marcado.

Curso 1FIS0311 · 2026-25 · Entrega semana 2 (7-13 sep 2026)
Integrantes: Hans Leonel Jurado Muñoz · Alejandra Perla Camere
Asesor: MBA Ing. Julio César Zácari Ramos

---

## Tema

**Sistema de gestión y priorización de prospectos de aporte con segmentación analítica para
museos privados sin fines de lucro**

<!-- El formato pide: "Cuál será el aporte de la propuesta para solucionar un problema de un
     escenario (institución) mediante el uso de técnicas o herramientas de TI." -->

El proyecto propone un **sistema de gestión de donantes que incorpora un modelo de segmentación
analítica** para identificar y priorizar, dentro de la base de miembros de un museo, a quiénes
tienen mayor potencial de convertirse en aportantes económicos, y para dar trazabilidad al ciclo
completo del aporte.

El problema que resuelve es la **baja conversión de miembros no aportantes en aportantes** y la
**gestión manual y sin trazabilidad** de los aportes, comprobantes y credenciales, en instituciones
que dependen críticamente de las donaciones porque sus ingresos por taquilla no cubren sus costos
de operación.

La técnica de tecnologías de información aplicada es la **analítica de datos con segmentación no
supervisada**, enriquecida con fuentes de datos públicas, siguiendo el método CRISP-DM, e
implementada dentro de un sistema de gestión.

El escenario de validación es el **Museo de Arte Contemporáneo de Lima (MAC)**, museo privado sin
fines de lucro, a través de su programa *Amigos del MAC*.

### Descomposición del tema

| Componente | |
|---|---|
| **Aporte** | Sistema de gestión con modelo de segmentación analítica de prospectos |
| **Problema** | Baja conversión de miembros a aportantes y gestión sin trazabilidad del aporte |
| **Técnica** | Analítica de datos, segmentación no supervisada, enriquecimiento con datos públicos (CRISP-DM) |
| **Escenario** | Museo de Arte Contemporáneo de Lima (MAC) |

---

## Sustento

> **Estructurado con las cuatro preguntas de investigación** del material del curso
> (`U1-S1-1. Tesis, Investigación y Tema.pdf`). Falta poblarlo con datos verificados.

### ¿Qué problema se investiga y qué datos justifican su importancia?

**a) El escenario depende de las donaciones para existir.**
Los ingresos por venta de entradas del MAC cubren menos del [DATO PENDIENTE] % del costo de
operación del museo. [FUENTE PENDIENTE — dato primario del museo, requiere documento citable]

**b) La base de conversión está prácticamente inactiva.**
El programa *Amigos del MAC* cuenta con 1 080 miembros sin aporte económico ("vecinos") frente a
30 miembros aportantes (25 personas naturales y 5 organizaciones). Desde 2023, **un solo miembro
no aportante se ha convertido en aportante**, lo que representa una tasa de conversión histórica
de 0,09 %. [FUENTE PENDIENTE — dato primario del museo, requiere documento citable]

**c) La gestión es manual y sin trazabilidad.**
El registro de miembros, los aportes, los comprobantes de pago y las credenciales se administran
por correo electrónico, sin sistema. La emisión de una credencial digital toma **2 días** y se
elabora manualmente. Ni el museo ni el aportante tienen certeza documentada de la fecha de pago.
[FUENTE PENDIENTE — dato primario del museo]

**d) El problema no es exclusivo del escenario.**
[DATO PENDIENTE — evidencia sectorial sobre dependencia de donaciones en museos]
[DATO PENDIENTE — evidencia sobre tasas de retención y conversión de donantes]
[FUENTE PENDIENTE — informes primarios, no citas de blogs]

### ¿Para qué y para quiénes se resuelve?

- **El museo**, que podría sostener y ampliar su programación cultural y educativa.
- **Los aportantes**, que hoy carecen de constancia y seguimiento de su aporte.
- **El público**, beneficiario final de la programación que las donaciones financian.
- **Otros museos privados sin fines de lucro** con el mismo problema: la solución se diseña para
  ser aplicable a esa clase de institución, no solo al escenario de validación.

### ¿Dónde está la información y quién la posee?

La información primaria la posee el MAC Lima, a través de su área de crecimiento, y es accesible
para el equipo de proyecto. Comprende: padrón de miembros (1 080 registros con antigüedad, edad,
sexo y dirección), registro de aportantes desde 2023, correspondencia de aportes corporativos y
registros de emisión de credenciales.

La información secundaria se obtendrá de bases indexadas (Scopus, Web of Science) y de fuentes
institucionales del sector cultural.

### ¿Cómo se puede resolver y por qué no basta lo existente?

[PENDIENTE — argumentar por qué un CRM comercial no resuelve el problema:
 justificar con literatura, no con opinión]

---

## Objetivo general

> Implementar un sistema de gestión y priorización de prospectos de aporte basado en segmentación
> analítica para la captación y fidelización de donantes en museos privados sin fines de lucro,
> a fin de incrementar la conversión de miembros no aportantes y reducir el tiempo de gestión
> administrativa del aporte.

---

## Objetivos específicos

1. **Determinar** el diagnóstico de la situación actual del proceso de gestión de miembros,
   aportes y credenciales, mediante el análisis de los registros y flujos vigentes del museo.

2. **Diseñar** el modelo de segmentación de miembros y la arquitectura del sistema de gestión y
   priorización de prospectos de aporte.

3. **Elaborar** el sistema de gestión y priorización aplicando el modelo de segmentación sobre la
   base de miembros del escenario.

4. **Verificar** el cumplimiento de los indicadores de éxito mediante la validación de la solución
   en un escenario real.

---

## Referencias

[PENDIENTE — se completan al cerrar el sustento. Norma APA-7.
 Criterios obligatorios: artículos científicos ≤3 años, Q1/Q2, de aporte, revista indexada;
 tesis, libros e informes ≤5 años.]

---

## Pendientes para cerrar este documento

| # | Qué falta | Responsable |
|---|---|---|
| 1 | Documento citable del museo que respalde los datos primarios (miembros, aportantes, conversiones, tiempos, cobertura de taquilla) | Alejandra |
| 2 | Evidencia sectorial sobre dependencia de donaciones en museos | búsqueda |
| 3 | Evidencia sobre retención y conversión de donantes, de fuente primaria | búsqueda |
| 4 | Argumento con literatura de por qué un CRM comercial no resuelve el problema | búsqueda |
| 5 | Cobertura de la taquilla sobre el costo de operación del museo | Alejandra |
| 6 | Confirmación del alcance con el asesor (pregunta #12) | Hans |
