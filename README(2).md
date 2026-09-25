# Datos para Todos
### Alfabetización digital con datos abiertos del municipio

**Autora:** Sara Sandino González
**Licencia:** Creative Commons Attribution 4.0 International (CC BY 4.0)
**Concurso Datos Abiertos de la Comunidad de Castilla y León 2026** · Categorías Ideas y Recurso Didáctico

---

## Presentación

Datos para Todos es un recurso didáctico abierto para talleres de alfabetización digital de personas adultas. Enseña a buscar, descargar, organizar, visualizar e interpretar datos abiertos usando información cercana al alumnado: empleo, formación y centros docentes de Castilla y León.

Está dirigido especialmente a personas en búsqueda de empleo, mayores de 45 años, población rural y colectivos con menor acceso a competencias digitales. **No requiere conocimientos previos de informática ni de programación**: el itinerario básico se realiza íntegramente con hoja de cálculo (Excel, LibreOffice Calc o Google Sheets), con una ampliación opcional en Python para grupos con más autonomía técnica.

## Dos formas de hacer el mismo taller

Este recurso tiene, para cada uno de los Talleres 1 a 4, dos vías paralelas que llegan al mismo resultado de aprendizaje:

| Vía | Para quién | Dónde está |
|---|---|---|
| **Hoja de cálculo (principal)** | Todo el grupo, sin excepción; es la vía obligatoria del itinerario | [`guia_version_excel.md`](guia_version_excel.md), en la raíz del repositorio |
| **Python / Jupyter (opcional)** | Solo para quien quiera curiosear con código, nunca obligatorio | Archivo `notebook_tallerN.ipynb` dentro de la carpeta de cada taller |

**Empieza siempre por `guia_version_excel.md`**: ahí está explicado paso a paso, actividad por actividad, exactamente qué botones y menús usar en Excel o LibreOffice Calc para completar cada taller. Los notebooks de Python son un extra, no un requisito, y usan los mismos datasets que la guía de Excel para mantener la coherencia del itinerario.

Los Talleres 5 y 6 **no tienen notebook propio**, y es una decisión de diseño, no un olvido: el Taller 5 reutiliza tablas ya trabajadas en talleres anteriores sin introducir dataset ni código nuevo, y el Taller 6 es un proyecto libre en el que cada participante elige su dataset, por lo que reutilizaría el notebook del taller correspondiente si quisiera hacer su proyecto final en Python.

## A quién va dirigido

| Perfil | Contexto de uso |
|---|---|
| Personas desempleadas o en búsqueda de empleo | Bibliotecas públicas, centros de educación de personas adultas, oficinas de empleo |
| Personas mayores de 45 años | Aulas de mayores, centros sociales, asociaciones de barrio |
| Población rural | Telecentros municipales, ayuntamientos, agentes de desarrollo local |
| Colectivos con menor acceso a competencias digitales | Entidades sociales, ONG, programas de inclusión digital |

## Estructura del repositorio

```
datos-para-todos/
├── README.md
├── LICENSE.md
├── guia_version_excel.md        (vía principal: instrucciones paso a paso para Excel/Calc)
├── taller1_que_son_datos_abiertos/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   ├── notebook_taller1.ipynb   (ampliación opcional en Python; Parte A + Parte B)
│   └── datos/                   (ofertas_empleo.csv, catalogo_datasets.csv)
├── taller2_buscar_informacion_cerca/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   ├── notebook_taller2.ipynb   (ampliación opcional en Python; Parte A + Parte B)
│   └── datos/                   (ofertas_empleo.csv, formacion_ecyl.csv)
├── taller3_ordenar_tabla_sin_miedo/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   ├── notebook_taller3.ipynb   (ampliación opcional en Python)
│   └── datos/                   (oferta_fp.csv)
├── taller4_del_dato_al_grafico/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   ├── notebook_taller4.ipynb   (ampliación opcional en Python)
│   └── datos/                   (directorio_centros.csv)
├── taller5_interpretar_sin_precipitarse/
│   ├── guia_alumnado.md
│   └── guia_facilitacion.md     (sin notebook: reutiliza datos de talleres anteriores)
├── taller6_mi_municipio_en_datos/
│   ├── guia_alumnado.md
│   └── guia_facilitacion.md     (sin notebook: proyecto libre, sin dataset fijo)
├── rubricas/
│   └── rubricas_evaluacion.md
└── accesibilidad/
    └── guia_accesibilidad.md
```

Las carpetas `datos/` de los Talleres 1 a 4 no incluyen los CSV ya descargados en el repositorio, para evitar que se desactualicen respecto a la fuente original: varios de estos datasets (Ofertas de Empleo, Formación del ECYL) se actualizan a diario. Cada participante, o el facilitador antes de la sesión, descarga ahí el archivo correspondiente siguiendo el enlace indicado en la guía de alumnado de cada taller.

## Los 6 talleres y los 5 datasets del proyecto

| Taller | Título | Dataset(s) JCyL | Notebook Python | Duración |
|---|---|---|---|---|
| 1 | ¿Qué son los datos abiertos? | Ofertas de Empleo (ejemplo guiado) + Catálogo de datasets del portal (exploración libre) | Sí | 60 min |
| 2 | Buscar información útil cerca de mí | Ofertas de Empleo + Formación del ECYL | Sí | 90 min |
| 3 | Ordenar una tabla sin miedo | Oferta de estudios de Formación Profesional | Sí | 90 min |
| 4 | Del dato al gráfico | Directorio de Centros Docentes | Sí | 90 min |
| 5 | Interpretar sin sacar conclusiones precipitadas | Reutiliza datos de talleres anteriores | No | 60 min |
| 6 | Mi municipio en datos (proyecto final) | A elección del participante, incluyendo cualquiera de los 5 anteriores | No (reutiliza notebook del dataset elegido) | 90-120 min |

Los **5 conjuntos de datos** citados en la memoria del proyecto (Ofertas de Empleo, Formación del ECYL, Oferta de FP, Directorio de Centros Docentes y Catálogo de datasets del portal) están efectivamente integrados en el recurso: los 4 primeros como dataset principal de un taller, y el Catálogo como herramienta de descubrimiento en el Taller 1 y como recurso transversal para el proyecto final del Taller 6.

Todos los datasets provienen del [Portal de Datos Abiertos de la Junta de Castilla y León](https://datosabiertos.jcyl.es) y son explotables desde el [portal de análisis de datos](https://analisis.datosabiertos.jcyl.es).

## Dónde descargar cada dataset

| Dataset | Archivo(s) a subir a `datos/` | Enlace de descarga |
|---|---|---|
| Ofertas de Empleo | `ofertas_empleo.csv` | [analisis.datosabiertos.jcyl.es/explore/dataset/ofertas-de-empleo](https://analisis.datosabiertos.jcyl.es/explore/dataset/ofertas-de-empleo/) |
| Catálogo de datasets del portal | `catalogo_datasets.csv` | [analisis.datosabiertos.jcyl.es/explore/dataset/catalogo-de-datos](https://analisis.datosabiertos.jcyl.es/explore/dataset/catalogo-de-datos/) |
| Formación del ECYL | `formacion_ecyl.csv` | [datosabiertos.jcyl.es/.../formacion-empleo](https://datosabiertos.jcyl.es/web/jcyl/set/es/empleo/formacion-empleo/1284354357765) |
| Oferta de estudios de FP | `oferta_fp.csv` | [datosabiertos.jcyl.es/.../oferta-formacion-profesional](https://datosabiertos.jcyl.es/web/jcyl/set/es/educacion/oferta-formacion-profesional/1285065645144) |
| Directorio de Centros Docentes | `directorio_centros.csv` | [analisis.datosabiertos.jcyl.es/explore/dataset/directorio-de-centros-docentes](https://analisis.datosabiertos.jcyl.es/explore/dataset/directorio-de-centros-docentes/) |

En los enlaces del portal de **análisis** (`analisis.datosabiertos.jcyl.es`), usa el botón **Exportar → CSV**. En los enlaces del portal **general** (`datosabiertos.jcyl.es`), la ficha del dataset tiene botones directos de descarga en varios formatos; pulsa el de **CSV**. Renombra siempre el archivo descargado exactamente como indica la columna "Archivo(s) a subir", porque los notebooks y las rutas del código esperan ese nombre exacto.

## Requisitos técnicos

- **Itinerario básico (obligatorio)**: Excel, LibreOffice Calc o Google Sheets. No requiere instalación adicional ni conocimientos previos de informática. Procedimiento completo en [`guia_version_excel.md`](guia_version_excel.md).
- **Ampliación opcional (Python)**: para grupos con más autonomía técnica. Cada notebook incluye una celda inicial para comprobar los nombres reales de las columnas del CSV descargado, ya que pueden variar según el formato de exportación del portal. Se recomienda [Google Colab](https://colab.research.google.com) si no hay Python instalado en los equipos.

## Principios de diseño

- **Sin barrera de programación**: el itinerario básico no requiere ningún conocimiento técnico previo.
- **Enfoque local**: cada grupo trabaja con datos de su propia provincia o municipio.
- **Lenguaje claro**: instrucciones numeradas, vocabulario sencillo, capturas de pantalla de apoyo.
- **Accesibilidad**: materiales imprimibles, tipografía legible, alternativa textual para gráficos (ver `accesibilidad/guia_accesibilidad.md`).
- **Aprendizaje crítico**: cada taller distingue entre un dato, una interpretación razonable y una conclusión que los datos no permiten sostener.

## Licencia

Este recurso se publica bajo licencia **CC BY 4.0**. Puede copiarse, redistribuirse, adaptarse y usarse con cualquier fin, incluso comercial, mencionando la autoría original y enlazando a este repositorio. Los datos de origen conservan sus licencias propias del Portal de Datos Abiertos de la Junta de Castilla y León.

## Autoría

Proyecto presentado al Concurso de Datos Abiertos de la Comunidad de Castilla y León 2026, categorías Ideas y Recurso Didáctico, por Sara Sandino González (saragsandino@gmail.com).
