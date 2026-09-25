# Datos para Todos
### Alfabetización digital con datos abiertos del municipio

**Autora:** Sara Sandino
**Concurso Datos Abiertos de la Comunidad de Castilla y León 2026** · Categorías Ideas y Recurso Didáctico

---

## Presentación

Datos para Todos es un recurso didáctico abierto para talleres de alfabetización digital de personas adultas. Enseña a buscar, descargar, organizar, visualizar e interpretar datos abiertos usando información cercana al alumnado: empleo, formación y centros docentes de Castilla y León.

Está dirigido especialmente a personas en búsqueda de empleo, mayores de 45 años, población rural y colectivos con menor acceso a competencias digitales. No requiere conocimientos previos de informática ni de programación: el itinerario básico se realiza con hoja de cálculo, con una ampliación opcional en Python para grupos avanzados.

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
├── taller1_que_son_datos_abiertos/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   └── notebook_taller1.ipynb
├── taller2_buscar_informacion_cerca/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   └── notebook_taller2.ipynb
├── taller3_ordenar_tabla_sin_miedo/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   └── notebook_taller3.ipynb
├── taller4_del_dato_al_grafico/
│   ├── guia_alumnado.md
│   ├── guia_facilitacion.md
│   └── notebook_taller4.ipynb
├── taller5_interpretar_sin_precipitarse/
│   ├── guia_alumnado.md
│   └── guia_facilitacion.md
├── taller6_mi_municipio_en_datos/
│   ├── guia_alumnado.md
│   └── guia_facilitacion.md
├── rubricas/
│   └── rubricas_evaluacion.md
└── accesibilidad/
    └── guia_accesibilidad.md
```

## Los 6 talleres

| Taller | Título | Dataset JCyL | Duración |
|---|---|---|---|
| 1 | ¿Qué son los datos abiertos? | Catálogo de datasets del portal | 60 min |
| 2 | Buscar información útil cerca de mí | Ofertas de Empleo, Formación del ECYL | 90 min |
| 3 | Ordenar una tabla sin miedo | Oferta de estudios de FP | 90 min |
| 4 | Del dato al gráfico | Directorio de Centros Docentes | 90 min |
| 5 | Interpretar sin sacar conclusiones precipitadas | Reutiliza datos de talleres anteriores | 60 min |
| 6 | Mi municipio en datos (proyecto final) | A elección del participante | 90-120 min |

Todos los datasets provienen del [Portal de Datos Abiertos de la Junta de Castilla y León](https://datosabiertos.jcyl.es) y son explotables desde el [portal de análisis de datos](https://analisis.datosabiertos.jcyl.es).

## Requisitos técnicos

- **Itinerario básico**: Excel, LibreOffice Calc o Google Sheets. No requiere instalación adicional ni conocimientos previos de informática.
- **Ampliación opcional (Python)**: para grupos con más autonomía técnica, cada taller con datos incluye también un notebook de ejemplo. Se recomienda [Google Colab](https://colab.research.google.com) si no hay Python instalado en los equipos.

## Principios de diseño

- **Sin barrera de programación**: el itinerario básico no requiere ningún conocimiento técnico previo.
- **Enfoque local**: cada grupo trabaja con datos de su propia provincia o municipio.
- **Lenguaje claro**: instrucciones numeradas, vocabulario sencillo, capturas de pantalla de apoyo.
- **Accesibilidad**: materiales imprimibles, tipografía legible, alternativa textual para gráficos (ver `accesibilidad/guia_accesibilidad.md`).
- **Aprendizaje crítico**: cada taller distingue entre un dato, una interpretación razonable y una conclusión que los datos no permiten sostener.

