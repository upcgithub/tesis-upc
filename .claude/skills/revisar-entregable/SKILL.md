---
name: revisar-entregable
description: Audita un entregable contra los criterios oficiales antes de enviarlo (Plan de Trabajo, TB1, TB2, TB3, DD, informes de artículos). Úsala cuando Hans diga que va a entregar, que se acerca una fecha, o pida revisar un documento antes de subirlo.
---

# Revisión previa a la entrega

Ejecutar la revisión completa y reportar hallazgos por gravedad. **No dar visto bueno si algo del
bloque de bloqueantes falla.**

## Paso 1 — Identificar qué se entrega 🟥

De `1-gestion/cronograma.md`:

| Entrega | Sem | Peso | Alcance | Documento |
|---|---|---|---|---|
| Plan de Trabajo | 2 | — | Tema, sustento, objetivos, referencias | según formato oficial |
| TB1 | 7 | 20 % | Hasta capítulo **2.2** | 2 días antes |
| TB2 | 11 | 20 % | **Capítulo 2 completo** | 2 días antes |
| TB3 | 15 | 30 % | **Capítulo 3 (Diseño)** | 3 días antes |
| DD | 15 | 30 % | Evaluación de Desempeño — ABET | día de la clase 15 |

> ⚠️ El contenido de TB3 tiene una **discrepancia entre documentos oficiales**
> (pregunta #1 en `preguntas-abiertas.md`). Criterio vigente: manda la línea de tiempo.
> Si aún no hay respuesta del asesor, **recordárselo a Hans al revisar**.

**Primero de todo:** verificar que se está usando el **formato oficial del profesor**
(`6-material-oficial/`), no un formato improvisado (regla 🟥3).

## Paso 2 — Bloqueantes 🟥

- [ ] **Ninguna referencia inventada.** Cada cita tiene entrada en `biblioteca.bib`, DOI real y PDF
      en `2-fuentes/pdfs/`. Listar todo `[VERIFICAR]` pendiente.
- [ ] **Criterios de fuente:** artículos del estado del arte ≤3 años, Q1/Q2, de aporte, indexados.
      Libros/tesis/informes ≤5 años.
- [ ] **Cada cita del texto está en las referencias, y cada referencia se cita en el texto.**
- [ ] Estructura de secciones idéntica a la exigida (`CONTEXTO.md` §3).
- [ ] Se usó el formato oficial del entregable.

> El anexo de uso de IA está **pendiente de definir** con el asesor (pregunta #2). Recordarlo aquí
> hasta que se resuelva: es un anexo evaluado y no se puede reconstruir a última hora.

## Paso 3 — Coherencia 🟥

Recorrer la cadena y reportar eslabones rotos:

```
situación problemática → problemas formulados → objetivos específicos
  → indicadores de éxito → estado del arte → brecha → diseño del aporte
```

- [ ] ¿Cada problema formulado tiene al menos un objetivo específico que lo ataca?
- [ ] ¿Cada objetivo específico tiene un indicador de éxito medible?
- [ ] ¿Los indicadores usan las métricas que el estado del arte mostró que usa la comunidad?
- [ ] ¿La brecha del 2.4 justifica exactamente el aporte del capítulo 3?
- [ ] ¿El título conserva los 4 componentes: aporte, problema, técnica, escenario?
- [ ] ¿El problema está abstraído de la organización?

## Paso 4 — Forma 🟥

- [ ] APA-7 en el documento / IEEE en el paper, sin mezclar
- [ ] Citas textuales con número de página
- [ ] Tablas y figuras numeradas, con título y **fuente**
- [ ] Sin marcadores olvidados: `TODO`, `[VERIFICAR]`, `_(por definir)_`
- [ ] Redacción académica impersonal; ortografía revisada
- [ ] Nombre de archivo y formato de entrega según lo pedido por el asesor

## Paso 5 — Congelar la entrega 🟦

```bash
cp -R 3-documento/trabajo/<lo-entregado> 3-documento/entregas/<TBx>-YYYY-MM-DD/
git add -A && git commit -m "entrega <TBx>: <alcance>"
git tag <TBx>-2026-25
```

Permite después mostrar **qué cambió entre entregas**, que es lo que pide la gestión del proyecto
(*"planificación vs ejecución"*).

## Paso 6 — Recordatorios de plazo 🟥

- El documento se entrega **2 o 3 días ANTES** de la sustentación, no el mismo día.
- **No hay postergaciones.** Planificar contra la fecha del documento.
- El **60 % de la nota** se decide en la semana 15 (TB3 + DD).
