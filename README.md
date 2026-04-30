# TFM - Violencia de Género en España

## Descripción

Este proyecto tiene como objetivo analizar la incidencia territorial de la violencia de género en España mediante la integración de fuentes de datos oficiales y el desarrollo de un modelo analítico basado en técnicas de aprendizaje supervisado.

El trabajo forma parte de un Trabajo de Fin de Máster (TFM) en Ciencia de Datos y combina ingeniería de datos, análisis exploratorio y modelado predictivo.

---

## Arquitectura

Se ha implementado una arquitectura tipo Lakehouse en Databricks basada en las siguientes capas:

RAW: ingesta de datos originales (CSV, Excel)
CLEAN: limpieza, normalización y tipificación
PREPROCESS: integración de datasets (joins por provincia y año)
ANALYTICAL: dataset final listo para análisis y modelado

Ver diagrama en: docs/arquitectura_sistema.png

---

## Dataset final

Observaciones: 156
Provincias: 52
Periodo: 2021–2023
Unidad de análisis: provincia-año

Variables principales:

denuncias
víctimas
órdenes de protección
quebrantamientos
renta media
tasas de actividad, empleo y paro
variables derivadas (tasas por 100k, ratios, etc.)

---

## Fuentes de datos

- https://datos.gob.es/es/catalogo/ea0040772-violencia-de-genero
- https://www.ine.es
- https://www.poderjudicial.es/cgpj/es/Temas/Estadistica-Judicial/Estudios-e-Informes/Violencia-sobre-la-Mujer/
- https://www.poderjudicial.es/cgpj/es/Temas/Estadistica-Judicial/Estadistica-por-temas/Datos-penales--civiles-y-laborales/Violencia-domestica-y-Violencia-de-genero/Violencia-Domestica-y-Violencia-de-Genero--explotacion-estadistica-del-Registro-Central-para-la-Proteccion-de-las-Victimas-de-la-Violencia-Domestica-/
- https://www.ine.es/dynt3/inebase/index.htm?padre=11249&capsel=11251
- https://www.ine.es/dynt3/inebase/index.htm?padre=7062&capsel=7071
---

## Estructura del repositorio

- notebooks/ → notebooks del proyecto
- data/final/ → dataset final
- docs/ → memoria del TFM

---

## Tecnologías

- Databricks
- Apache Spark (PySpark)
- Delta Lake
- Python
- Power BI

---
## Modelado

Se han desarrollado modelos de aprendizaje supervisado para analizar la variable objetivo:

Regresión logística
Random Forest

Consideraciones:

Prevención de leakage temporal
Evaluación mediante train-test split estratificado
Análisis de multicolinealidad
Interpretabilidad de resultados
---

## Autor

Visnu Rivero
