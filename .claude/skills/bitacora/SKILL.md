---
name: bitacora
description: Registra el avance de una sesión de trabajo y actualiza el estado del proyecto. Úsala al cerrar una sesión, cuando Hans diga "guarda el avance", "cierra por hoy", o al retomar el trabajo tras varios días para reconstruir dónde se quedó. También cubre las actas de asesoría.
---

# Bitácora y actas

Un proyecto de tres semestres tiene huecos de semanas. Esto es lo que permite retomar en 2 minutos
en vez de 40.

## Al CERRAR una sesión

**1.** Crear o ampliar `1-gestion/bitacora/YYYY-MM-DD.md`:

```markdown
# YYYY-MM-DD — Semana N

## Hecho
- …

## Decisiones tomadas
- Qué se decidió y **por qué**.

## Bloqueos / dudas
- …

## Siguiente paso concreto
- Una sola acción específica. No "avanzar el cap. 2".
```

🟨 El campo *"decisiones y por qué"* es criterio propio, no exigencia del curso. Rinde cuando el
asesor pregunta *"¿por qué elegiste esta técnica y no aquella?"* seis semanas después.

**2.** Si surgió una duda de criterio → llevarla a `1-gestion/preguntas-abiertas.md` (regla 🟦11).

**3.** Actualizar `1-gestion/CONTEXTO.md` §11: semana actual, tema, próximo entregable, asesor.

**4.** Commit:
```bash
git add -A && git commit -m "bitácora YYYY-MM-DD: <resumen corto>"
```

## Al RETOMAR

1. Leer `1-gestion/CONTEXTO.md` §11
2. Leer las **2 últimas** entradas de `1-gestion/bitacora/`
3. Revisar `cronograma.md`: qué semana es y qué toca
4. Revisar `preguntas-abiertas.md`: ¿alguna sigue bloqueando?
5. Resumirle a Hans en 3 líneas: dónde quedó, qué falta, qué toca ahora

## Actas de asesoría 🟥

Distinto de la bitácora. Son **artefacto de gestión evaluado** — el curso exige actas de reunión
(*"Planificación vs ejecución, actas de reunión, etc."*) y el asesor debe registrar el informe
semanal de asesorías.

Van en `1-gestion/asesorias/YYYY-MM-DD-acta.md`, sobre `_plantilla-acta.md`.

Después de cada asesoría:
- ¿Respondió alguna pregunta abierta? → cerrarla en `preguntas-abiertas.md` con la respuesta
- ¿Cambió alguna regla o criterio? → actualizar `CONTEXTO.md`
- ¿Dio un formato oficial nuevo? → guardarlo en `3-documento/formatos-oficiales/`
