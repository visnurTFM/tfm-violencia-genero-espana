# TFM - Violencia de Género en España

## Descripción

Este proyecto tiene como objetivo la construcción de un dataset analítico para el estudio de la violencia de género en España mediante la integración de múltiples fuentes de datos públicas.

El desarrollo se ha realizado en Databricks utilizando Apache Spark y una arquitectura de datos tipo lakehouse.

---

## Arquitectura

Se ha implementado una arquitectura en capas:

RAW → CLEAN → PREPROCESS → ANALYTICAL

- RAW: datos originales
- CLEAN: limpieza y normalización
- PREPROCESS: integración de datasets
- ANALYTICAL: dataset final

---

## Dataset final

- 208 observaciones
- 52 provincias
- Periodo: 2021–2024
- Unidad de análisis: provincia-año

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

---

## Autor

Visnu Rivero
