# Guía de Traducción al Español de DatoCMS

Esta guía define las reglas para garantizar consistencia en las traducciones al español de la interfaz de DatoCMS.

## Reglas Fundamentales

- **"Tú" informal** en toda la interfaz (nunca "usted" o "vosotros")
- **Términos técnicos en inglés** (build, deploy, webhook, adapter, schema, hook, payload, sandbox)
- **Concordancia verbal y de género** adecuada
- **"por favor"** siempre dos palabras (nunca "porfavor")

## Reglas de Disambiguación

### Unpublish/Unpublishing (IMPORTANTE)

El término se **traduce** consistentemente como **"despublicar"**:

| Inglés       | Español                    |
| ------------ | -------------------------- |
| Unpublish    | Despublicar                |
| Unpublishing | Despublicación             |
| Unpublished  | Despublicado/Sin publicar  |

| ✅ Correcto                        | ❌ Incorrecto                         |
| --------------------------------- | ------------------------------------ |
| Despublicar el registro           | Anular la publicación del registro   |
| No se pudo despublicar            | No se pudo quitar la publicación     |
| Registros despublicados           | Publicación de registros anulada     |

**Nunca usar** "anular la publicación", "quitar publicación", o variantes similares.

### Estado "Updated" (IMPORTANTE)

El estado "Updated" en inglés significa **"Cambios sin publicar"**, NO "Actualizado":

| Inglés             | ✅ Español correcto       | ❌ Español incorrecto |
| ------------------ | ------------------------ | -------------------- |
| Unpublished changes | Cambios sin publicar     | Actualizado          |
| Updated            | Cambios sin publicar     | Actualizado          |

Este estado indica que hay cambios guardados que aún no se han publicado.

### Record vs Entry

Usar **siempre** "registro" para traducir "record" o "entry":

| ✅ Correcto                      | ❌ Incorrecto                    |
| ------------------------------- | ------------------------------- |
| No se pudo eliminar el registro | No se pudo eliminar la entrada  |
| No se pudo publicar el registro | No se pudo publicar la entrada  |

### Títulos de Diálogos de Confirmación

Para títulos de diálogos que piden confirmación, usar el **infinitivo** con signos de interrogación:

| Tipo                    | Ejemplo                          |
| ----------------------- | -------------------------------- |
| Diálogo de confirmación | "¿Eliminar este registro?"       |
| Diálogo de confirmación | "¿Cancelar la publicación?"      |
| Diálogo de confirmación | "¿Despublicar registros hijos?"  |

**IMPORTANTE**: En español, los signos de interrogación van al **inicio** (¿) y al **final** (?).

| ✅ Correcto                    | ❌ Incorrecto              |
| ----------------------------- | ------------------------- |
| ¿Eliminar filtro?             | Eliminar filtro           |
| ¿Quitar referencias?          | Quitar referencias?       |
| ¿Eliminar traducción {locale}? | Eliminar traducción {locale} |

Para **botones de acción**, usar el **infinitivo**:

| Tipo   | Ejemplo      |
| ------ | ------------ |
| Botón  | "Publicar"   |
| Botón  | "Eliminar"   |
| Botón  | "Despublicar"|

### Patrón para Mensajes de Error

Usar **siempre** el patrón "No se pudo + infinitivo" (forma impersonal):

| ✅ Correcto                    | ❌ Incorrecto              |
| ----------------------------- | ------------------------- |
| No se pudo guardar            | No pudimos guardar        |
| No se pudo eliminar           | Imposible eliminar        |
| No se pudo cargar             | Error en la carga         |
| No se pudieron publicar       | No pudimos publicar       |

**Nunca usar** la primera persona del plural ("No pudimos...").

### Puntuación en Mensajes

| Tipo de mensaje      | Puntuación                | Ejemplo                              |
| -------------------- | ------------------------- | ------------------------------------ |
| **Error/Fallo**      | Signo de exclamación `!`  | "¡No se pudo guardar el registro!"   |
| **Éxito con acción** | Signo de exclamación `!`  | "¡Registro guardado con éxito!"      |
| **Éxito neutro**     | Sin puntuación o punto    | "Registro guardado con éxito"        |
| **Descripción/Info** | Punto `.`                 | "Este campo es obligatorio."         |
| **Label de UI**      | Sin puntuación            | "Guardar registro"                   |

**Regla general**: Los mensajes de error llevan **siempre** `!` para indicar urgencia.

**IMPORTANTE**: En español, el signo de exclamación va al **inicio** (¡) y al **final** (!).

### Expand/Collapse

Para acciones de expansión y contracción de elementos de UI:

- **"Expand"** → **"Expandir"** (infinitivo) / **"Expande"** (imperativo informal)
- **"Collapse"** → **"Contraer"** (infinitivo) / **"Contrae"** (imperativo informal)

| Inglés       | Español (infinitivo) |
| ------------ | -------------------- |
| Expand       | Expandir             |
| Expand all   | Expandir todo        |
| Collapse     | Contraer             |
| Collapse all | Contraer todo        |

**Nunca traducir** "expand" como "desplegar" ni "collapse" como "comprimir" o "cerrar".

### Heading vs Título

- **"Heading"** (H1-H6 en editor de texto) → **"Encabezado"**
- **"Title"** (campo título, título de página) → **"Título"**

| Inglés      | Español          |
| ----------- | ---------------- |
| Heading 1   | Encabezado 1     |
| Heading 2   | Encabezado 2     |
| Title field | Campo de título  |
| Page title  | Título de página |

### Listas (Bulleted/Numbered)

- **Bulleted list** → **Lista con viñetas** (no "Lista de puntos")
- **Numbered list** → **Lista numerada**

### Environment

El término **"environment"** se **traduce** como **"entorno"**:

| Inglés              | Español                  |
| ------------------- | ------------------------ |
| Current environment | Entorno actual           |
| Switch to           | Cambiar a                |
| Sandbox environment | Entorno sandbox          |
| Primary environment | Entorno principal        |

## Glosario

```
"Add" → "Agregar" o "Añadir"
"Block" → "Bloque"
"Custom asset storage" → "Almacenamiento de assets personalizado"
"DatoCMS Support" → "Soporte de DatoCMS"
"DatoCMS-hosted assets" → "Assets alojados en DatoCMS"
"Delete asset collection" → "Eliminar colección de assets"
"direct download URL" → "URL de descarga directa"
"dragging and dropping" → "arrastrando y soltando"
"Editor's Preferences" → "Preferencias del editor"
"Environment fast-fork" → "Fast-fork del entorno"
"Error reporter" → "Reporte de errores"
"Facebook video" → "Video de Facebook"
"Field appearance plugin" → "Plugin de apariencia del campo"
"File type" → "Tipo de archivo"
"information" → "información"
"internet connection" → "conexión a internet"
"item" → "registro"
"locales" → "idiomas"
"Menu item" → "Elemento de menú"
"Permissions" → "Permisos"
"platform" → "plataforma"
"private" → "privado"
"project" → "proyecto"
"publicly accessible" → "accesible públicamente"
"Read-only mode" → "Modo de solo lectura"
"restricted" → "restringido"
"scheduled maintenance" → "mantenimiento programado"
"Selected" → "Seleccionados"
"selected" → "seleccionado"
"selector" → "selector"
"sidebar" → "barra lateral"
"tags" → "etiquetas"
"Upload endpoint" → "Endpoint de carga"
"User account" → "Cuenta de usuario"
"video platform" → "plataforma de video"
"video provider" → "proveedor de video"
"Vimeo URL" → "URL de Vimeo"
"YouTube URL" → "URL de YouTube"
```
