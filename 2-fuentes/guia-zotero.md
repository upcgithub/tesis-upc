# Guía de Zotero para la tesis

## Por qué

Son **24 artículos**, y las mismas referencias se necesitan en **dos formatos**: APA-7 en el
documento de tesis, IEEE en el paper.

```
APA-7:  Zhang, L., & Kumar, R. (2024). Federated learning for privacy.
        IEEE Access, 12, 45-62. https://doi.org/10.1109/ACCESS.2024.1234

IEEE:   [1] L. Zhang and R. Kumar, "Federated learning for privacy,"
        IEEE Access, vol. 12, pp. 45-62, 2024.
```

A mano son 48 transcripciones y 48 oportunidades de error. Con gestor, cambiar de formato es un
desplegable.

> La Biblioteca UPC da soporte a **Zotero, Mendeley y EndNote Web** — los tres son válidos.
> Esta guía usa Zotero (gratis, sin límite local, exporta `.bib` limpio). Mendeley es del mismo
> dueño que Scopus, así que importa algo mejor desde ahí; si prefieres ese, el flujo es equivalente.

---

## 1. Instalación

1. Descargar Zotero de [zotero.org/download](https://www.zotero.org/download/) (versión de escritorio)
2. Instalar el **Zotero Connector** en el navegador (misma página)
3. Al instalar Zotero, el **plugin de Word** se añade solo.
   Comprobar: abrir Word → debe aparecer una pestaña **Zotero**.
   Si no está: Zotero → *Editar → Configuración → Citar → Procesadores de texto → Instalar*

## 2. Organizar la biblioteca

Crear una colección `Tesis-SIA` y, dentro, subcolecciones por sección:

```
Tesis-SIA
├── Cap1-contexto        fuentes del sector (pueden ser ≤5 años, no necesariamente Q1/Q2)
├── Cap2-estado-arte     los 24 artículos Q1/Q2 de aporte
└── Descartados          los que se revisaron y no cumplieron criterios
```

Guardar los descartados **también** sirve: documenta el cribado del capítulo 2.1 y evita
revisar dos veces el mismo artículo.

## 3. Importar desde Scopus

1. En Scopus, ejecutar la búsqueda y marcar los resultados
2. **Export → BibTeX** o **RIS** → se descarga un archivo
3. En Zotero: *Archivo → Importar* → seleccionar el archivo
   *(o, con el Connector instalado, el icono de la barra del navegador los captura directamente)*
4. Verificar que los metadatos llegaron completos, sobre todo **DOI** y **páginas**

Desde **Web of Science** el flujo es el mismo: *Export → BibTeX*.

## 4. Registrar el cuartil

Zotero no trae el cuartil. Hay que añadirlo a mano, y es obligatorio (`CONTEXTO.md` §5):

1. Buscar el journal en [scimagojr.com](https://www.scimagojr.com/)
2. Anotar el cuartil **y el año** (cambia entre años)
3. En Zotero, añadir una **etiqueta** al ítem: `Q1-2024` o `Q2-2024`
4. Los que salgan Q3/Q4 → mover a la subcolección `Descartados`

Así puedes filtrar por etiqueta y ver de un vistazo si los 24 cumplen.

## 5. Exportar a `biblioteca.bib`

1. Clic derecho en la colección `Tesis-SIA` → **Exportar colección**
2. Formato **BibTeX**, marcar *Exportar notas* si quieres conservar anotaciones
3. Guardar como `2-fuentes/biblioteca.bib` (sobrescribe el existente)

Repetir cada vez que se añadan artículos, para que el `.bib` no quede desfasado.

🟨 *Opcional:* el plugin **Better BibTeX** genera claves de cita estables
(`zhang2024federated` en vez de una clave aleatoria) y puede mantener el `.bib` sincronizado solo.
Útil si el `.bib` se va a exportar muchas veces.

## 6. Citar en Word

1. Pestaña **Zotero** → *Document Preferences* → estilo **American Psychological Association 7th edition**
2. *Add/Edit Citation* → buscar el artículo → insertar. Queda `(Zhang & Kumar, 2024)`
3. Para cita textual, añadir la página en el diálogo de la cita → `(Zhang & Kumar, 2024, p. 8)`
4. Al final del documento: *Add/Edit Bibliography* → la lista se genera y **se mantiene sola**

Si borras una cita del texto, desaparece de la lista de referencias. Eso resuelve el bloqueante
de *"cada cita está en las referencias y cada referencia se cita"* de la skill `revisar-entregable`.

## 7. Cambiar a IEEE para el paper

En el documento del paper: pestaña Zotero → *Document Preferences* → estilo **IEEE** → Aceptar.
Las citas y toda la bibliografía se reescriben.

**No cambiar el estilo del documento de tesis**: ese va en APA-7 (regla 🟥6 de `CLAUDE.md`).

---

## Lo que Zotero NO resuelve

- **No verifica que el artículo sea de aporte y no una revisión.** Eso se filtra en la búsqueda
  con `DOCTYPE(ar)` y se comprueba leyendo.
- **No trae el cuartil.** Paso 4, a mano.
- **No garantiza que los metadatos estén bien.** Scopus a veces exporta páginas o DOI incompletos:
  revisar antes de fichar.
- **No lee los artículos por ti.** La ficha de `2-fuentes/fichas/` sigue siendo trabajo de lectura.
