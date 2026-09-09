# Análisis del problema — nota de trabajo

> Base para el **capítulo 1: Definición del proyecto**. Construido con el método exacto de
> `6-material-oficial/2026-25-seminario-investigacion/clase-02/U1-S2-1.Definición del problema.pdf`:
> hechos y factores → síntomas → causas → efectos → diagnóstico → pronóstico → formulación.
>
> **Estado:** los hechos son datos primarios del escenario (falta documento citable).
> **Las causas son hipótesis**, no hallazgos: el análisis con datos aún no se ha hecho.

---

## 1. Hechos y factores

| Hecho | Valor | Fuente |
|---|---|---|
| Miembros vecinos sin aporte económico | 1 080 | Primaria MAC — [FUENTE PENDIENTE] |
| Aportantes personas naturales | 25 | Primaria MAC — [FUENTE PENDIENTE] |
| Aportantes organizaciones | 5 | Primaria MAC — [FUENTE PENDIENTE] |
| Conversiones vecino → aportante desde 2023 | **1** (0,09 %) | Primaria MAC — [FUENTE PENDIENTE] |
| Cobertura de la taquilla sobre el costo de operación | < 50 % | Primaria MAC — [DATO PENDIENTE] |
| Emisión de credencial digital | 2 días, manual | Primaria MAC — [FUENTE PENDIENTE] |
| Soporte de la gestión | correo electrónico | Primaria MAC |
| Datos disponibles de los 1 080 | antigüedad, nombre, dirección, teléfono, edad, sexo | Primaria MAC |
| Registro de aportantes personas | Excel desde 2023 | Primaria MAC |
| Registro de aportantes empresa | disperso en correo | Primaria MAC |
| Periodicidad del aporte | anual; renovación en el aniversario de cada aportante | Primaria MAC |
| Mecanismo de captación actual | eventos | Primaria MAC |

## 2. Síntomas

- La base de 1 080 miembros no genera aportantes nuevos
- Ni el museo ni el aportante tienen certeza documentada de la fecha de pago
- La información está dispersa entre correos, un Excel y fotografías de comprobantes
- No existe seguimiento individual del ciclo de vida de cada miembro
- La emisión de credenciales es lenta y poco personalizada

## 3. Causas posibles — **hipótesis a validar**

| # | Causa | Cómo se validaría |
|---|---|---|
| C1 | No existe un registro único y estructurado de miembros, lo que impide segmentar | Auditoría del estado actual de los datos |
| C2 | No hay criterio de priorización: los 1 080 se tratan como un bloque homogéneo | Entrevista con el área de crecimiento |
| C3 | El esfuerzo de captación se concentra en eventos masivos, no en contacto dirigido | Registro de acciones de captación |
| C4 | No hay trazabilidad del aporte, por lo que no se puede medir ni dar seguimiento | Revisión del proceso actual |
| C5 | El proceso manual consume el tiempo del área, que no queda para captación | Medición de tiempos del proceso |
| C6 | El reconocimiento al aportante es lento y genérico | Ya medido: 2 días, manual |

## 4. Efectos

- El museo depende de **30 aportantes** para cubrir más de la mitad de su operación
- La concentración es crítica: una baja entre las 5 empresas tendría impacto desproporcionado
- El potencial de 1 080 personas ya vinculadas al museo queda sin aprovechar
- La experiencia débil del aportante compromete su renovación

## 5. Árbol de problema

```
        EFECTO      Sostenibilidad financiera del museo comprometida
                                      ▲
      PROBLEMA      La base de aportantes no crece: 0,09 % de conversión
                                      ▲
        ┌─────────────────────────────┼─────────────────────────────┐
        │                             │                             │
       C1 + C4                       C2 + C3                       C6
   Sin registro                 Sin criterio de              Reconocimiento
   estructurado ni              priorización;                lento y genérico
   trazabilidad                 captación masiva
        │                             │                             │
   No se puede                  Los 1 080 se                 Vínculo débil
   segmentar                    tratan igual                 con el aportante
```

**Cadena causal:** sin datos ordenados no se puede segmentar; sin segmentar no se puede
priorizar; sin priorizar, no se convierte a nadie.

> **Matiz honesto.** La falta de trazabilidad (C4) afecta sobre todo a los **30 que ya aportan**
> —su renovación— más que a la conversión de los 1 080. Ahí actúa como problema propio, no solo
> como causa. Se resuelve tratando la trazabilidad como **causa y como requisito de la solución**,
> lo que mantiene una sola cadena causal y evita que el proyecto se ensanche.

## 6. Diagnóstico

**Causas que el proyecto se propone resolver:** C1, C2, C4 de forma directa; C3 y C6 de forma
indirecta. **C5 no se ataca directamente**, pero mejora como consecuencia.

## 7. Pronóstico — ¿qué ocurrirá si la situación continúa?

La base de aportantes no crecerá, la dependencia de un grupo muy reducido se mantendrá, y
cualquier deserción —especialmente entre las organizaciones— comprometerá directamente la
operación del museo, que ya no cubre sus costos con la taquilla.

## 8. Formulación del problema

Como exige el documento: en modo de pregunta, incluyendo problema, técnica y escenario,
y cuya respuesta sea la propuesta de solución.

> **¿De qué manera un modelo de segmentación analítica, incorporado en un sistema de gestión de
> donantes, podría incrementar la conversión de miembros no aportantes en aportantes en museos
> privados sin fines de lucro?**

### Problemas específicos a resolver

1. Ausencia de un registro estructurado que permita caracterizar y segmentar a los miembros
2. Ausencia de criterio para priorizar a quién dirigir el esfuerzo de captación
3. Ausencia de trazabilidad del aporte, el comprobante y la credencial

---

## Pendientes de este análisis

| # | Qué falta |
|---|---|
| 1 | Documento citable del museo que respalde los hechos |
| 2 | Validar las causas C1-C5 con datos y entrevista, no solo por observación |
| 3 | Elaborar el árbol de problema formal (o Ishikawa) con la información del análisis |
| 4 | Cuantificar el efecto: ¿cuánto representa el aporte de las 5 empresas frente al total? |
| 5 | Antecedentes: qué soluciones existen en el mercado y por qué no se ajustan |
