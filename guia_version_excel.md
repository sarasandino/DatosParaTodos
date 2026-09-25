# Guía versión Excel / Hoja de cálculo

### Instrucciones paso a paso para los Talleres 1 a 4 usando Excel, LibreOffice Calc o Google Sheets

Esta es la **vía principal y obligatoria** del itinerario "Datos para Todos". No requiere conocimientos previos de informática ni de programación. Cualquiera de estos tres programas funciona igual de bien; las capturas y nombres de menú aquí descritos corresponden a Excel, pero se indica la equivalencia en LibreOffice Calc y Google Sheets cuando el nombre del botón cambia.

Antes de empezar cada taller, descarga el dataset correspondiente siguiendo el enlace de la tabla de descarga del `README.md` y guárdalo en la carpeta `datos/` de ese taller.

---

## Taller 1 · ¿Qué son los datos abiertos?

**Dataset:** Ofertas de Empleo (`ofertas_empleo.csv`)

1. Abre Excel y ve a **Datos → Obtener datos → Desde un archivo → Desde texto/CSV** (en LibreOffice Calc: **Archivo → Abrir** y selecciona el CSV directamente; en Google Sheets: **Archivo → Importar → Subir**).
2. Selecciona el archivo `ofertas_empleo.csv` que descargaste en la carpeta `datos/`.
3. Cuando aparezca la vista previa, comprueba que el separador de columnas está en **punto y coma (;)** y no en coma, porque los CSV de la Junta de Castilla y León usan punto y coma. Pulsa **Cargar**.
4. Observa la tabla: cada fila es una oferta de empleo, cada columna es un dato sobre esa oferta (título, provincia, localidad, fecha).
5. **Actividad 1:** cuenta cuántas filas tiene la tabla mirando el número de la última fila en la columna izquierda de Excel.
6. **Actividad 2:** usa **Ctrl+Mayús+L** (o el botón **Datos → Filtro**) para activar los filtros en la cabecera. Haz clic en la flecha de la columna "Provincia" y marca solo tu provincia.
7. **Actividad 3 (exploración libre):** entra en [analisis.datosabiertos.jcyl.es](https://analisis.datosabiertos.jcyl.es), busca el Catálogo de datasets del portal y explora libremente qué otros temas de datos existen (salud, transporte, cultura), sin necesidad de descargar nada.

## Taller 2 · Buscar información útil cerca de mí

**Datasets:** Ofertas de Empleo (`ofertas_empleo.csv`) + Formación del ECYL (`formacion_ecyl.csv`)

### Parte A — Ofertas de Empleo

1. Importa `ofertas_empleo.csv` siguiendo los mismos pasos del Taller 1.
2. Filtra por tu provincia y, dentro del filtro, añade una segunda condición filtrando por localidad si quieres afinar más.
3. Usa **Ctrl+F** (Buscar) para localizar una palabra clave en los títulos de las ofertas, por ejemplo "auxiliar" o "administrativo".

### Parte B — Formación del ECYL

1. Importa `formacion_ecyl.csv` en una hoja nueva del mismo archivo (botón **+** al pie de las pestañas en Excel, o **Insertar hoja** en Calc).
2. Filtra por tu provincia igual que en la Parte A.
3. **Actividad de cierre:** compara ambas hojas y anota si hay algún curso de formación relacionado con alguna de las ofertas de empleo que encontraste en la Parte A.

## Taller 3 · Ordenar una tabla sin miedo

**Dataset:** Oferta de estudios de Formación Profesional (`oferta_fp.csv`)

1. Importa `oferta_fp.csv` siguiendo el mismo procedimiento de los talleres anteriores.
2. Selecciona toda la tabla (**Ctrl+A** dentro del rango de datos) y ve a **Datos → Ordenar**.
3. Ordena primero por la columna "Provincia" de A a Z, y añade un segundo criterio de ordenación por "Familia profesional" pulsando **Añadir nivel** dentro del mismo cuadro de diálogo.
4. **Actividad:** identifica cuál es la familia profesional con más centros que la ofrecen en tu provincia, simplemente contando las filas repetidas tras ordenar.
5. Practica deshacer el orden (**Ctrl+Z**) y volver a ordenar por otro criterio, para perder el miedo a "romper" la tabla: ordenar nunca borra datos, solo cambia el orden de las filas.

## Taller 4 · Del dato al gráfico

**Dataset:** Directorio de Centros Docentes (`directorio_centros.csv`)

1. Importa `directorio_centros.csv` siguiendo el mismo procedimiento de los talleres anteriores.
2. Crea una tabla dinámica: selecciona los datos y ve a **Insertar → Tabla dinámica** (en Calc: **Insertar → Tabla dinámica**; en Sheets: **Insertar → Tabla dinámica**).
3. Arrastra el campo "Provincia" a **Filas** y el mismo campo "Provincia" (o cualquier otro) a **Valores**, configurado como **Recuento**, para obtener el número de centros por provincia.
4. Con la tabla dinámica seleccionada, ve a **Insertar → Gráfico** y elige **Gráfico de columnas**.
5. Ajusta el título del gráfico y los ejes desde el panel de **Diseño de gráfico** o haciendo doble clic sobre cada elemento del gráfico.
6. **Actividad de cierre:** añade un segundo gráfico filtrando solo los centros públicos (usando el filtro de la tabla dinámica) y compáralo visualmente con el gráfico del total de centros. Reflexiona sobre qué preguntas deja sin responder el gráfico, algo que trabajaremos en el Taller 5.

---

## Consejos generales para toda la guía

- Si un CSV se abre con todos los datos en una sola columna, revisa que el separador seleccionado en el asistente de importación sea punto y coma (`;`) y no coma (`,`).
- Guarda tu archivo de trabajo con un nombre distinto al del CSV original (por ejemplo, `taller1_trabajo.xlsx`), para no perder el CSV de partida si necesitas volver a importarlo.
- Si algo sale mal, **Ctrl+Z** deshace la última acción. No hay ningún paso de esta guía que borre datos de forma irreversible.
- Todas las capturas de pantalla de apoyo para cada paso están en la carpeta correspondiente de cada taller, dentro de `guia_alumnado.md`.
