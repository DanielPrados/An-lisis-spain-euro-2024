# 🔴 El dominio de "La Roja" en la Eurocopa 2024

### Del campo a los gráficos

Análisis y visualización de datos de la **Selección Española durante la UEFA Euro 2024**, desarrollado en **R y R Markdown** como proyecto académico de análisis visual de datos.

El proyecto explora diferentes dimensiones del juego mediante técnicas de visualización y análisis de datos, utilizando información de eventos de los partidos para estudiar el rendimiento de España y sus rivales.

---

## 📌 Descripción del proyecto

El fútbol genera una gran cantidad de datos por partido: posiciones, pases, disparos, regates, duelos y diferentes acciones realizadas por los jugadores.

El objetivo de este proyecto es transformar estos datos en **visualizaciones capaces de proporcionar información interpretable sobre el comportamiento de los equipos dentro del campo**.

A lo largo del análisis se estudian diferentes aspectos del juego de España durante la Eurocopa 2024, combinando análisis estadístico, representación espacial y visualización dinámica.

Entre otros aspectos, se analiza:

* ⚽ Generación de ocasiones y **goles esperados (xG)**.
* 🎯 Evolución temporal del xG durante los partidos.
* 🏃 Regates completados y su distribución.
* 🔄 Pases y precisión de pase.
* 📍 Distribución espacial de los pases.
* 🗺️ Zonas de mayor concentración de acciones.
* 🥅 Distribución espacial de los disparos.
* 🤝 Duelos ganados.
* 🛡️ Despejes.
* 🔴 Comparación entre España y sus rivales.
* 🎞️ Visualizaciones animadas para estudiar la evolución temporal de las acciones.

---

## 🛠️ Tecnologías utilizadas

El proyecto ha sido desarrollado principalmente con **R**, utilizando:

* **R Markdown** — elaboración del informe y documentación del análisis.
* **ggplot2** — creación y personalización de visualizaciones.
* **gganimate** — generación de visualizaciones animadas.
* **ggsoccer** — representación de acciones sobre un campo de fútbol.
* **dplyr** — transformación y manipulación de datos.
* **tidyr** — organización y transformación de estructuras de datos.
* **readr** — importación de datos.
* **ggrepel** — colocación de etiquetas evitando solapamientos.
* **gifski** — renderizado de animaciones en formato GIF.

---

## 📊 Análisis realizado

### Fundamentos de visualización con `ggplot2`

El proyecto comienza introduciendo los principales conceptos de la *Grammar of Graphics*, mostrando progresivamente el uso de:

* `ggplot()`
* `aes()`
* `geom_*`
* `facet_*`
* `scale_*`
* `theme_*`

A partir de estos elementos se construyen visualizaciones cada vez más elaboradas.

### ⚽ Pases

Se analiza el volumen y precisión de los pases, incluyendo una estandarización por 90 minutos para facilitar la comparación entre jugadores.

También se estudia espacialmente la distribución de los pases de jugadores como **Lamine Yamal**, representando sus trayectorias directamente sobre el campo.

### 🎯 Goles esperados (xG)

Se estudia la generación de ocasiones mediante la métrica **xG**, tanto a nivel individual como a través de su evolución temporal durante diferentes partidos de España.

La evolución acumulada del xG permite comparar el desarrollo ofensivo de los equipos a lo largo de cada encuentro.

### 🏃 Regates

Se analiza el número de regates completados por 90 minutos, identificando valores extremos mediante diagramas de caja y destacando determinados jugadores mediante etiquetas.

### 🗺️ Análisis espacial

Mediante `ggsoccer` se representan diferentes acciones directamente sobre un campo de fútbol, permitiendo estudiar dónde se concentran los pases, disparos y otras acciones.

También se emplean mapas de densidad bidimensional para analizar la distribución espacial de determinadas acciones durante los partidos.

### 🇪🇸 España frente a sus rivales

Se comparan diferentes métricas entre España y sus rivales durante la competición, incluyendo:

* Pases completados.
* Regates completados.
* Duelos ganados.
* Despejes.
* Distribución espacial de los pases.
* Generación de ocasiones.

El análisis permite estudiar diferentes dimensiones del rendimiento colectivo de España y contextualizar sus resultados durante la competición.

---

## 🎞️ Visualizaciones animadas

Una de las partes del proyecto consiste en la utilización de **`gganimate`** para representar la evolución temporal de las acciones futbolísticas.

Las animaciones permiten incorporar una dimensión temporal que no puede observarse de la misma manera en una representación estática, facilitando el estudio de la progresión de los eventos sobre el terreno de juego.

> Las visualizaciones animadas fueron desarrolladas por Daniel Prados Serrano.

---

## 📁 Estructura del repositorio

```text
euro-2024-spain-analysis-r/
│
├── README.md
├── report/
│   ├── Trabajo_Final_EC.Rmd
│   └── Trabajo_Final_EC.html
│
├── data/
│   ├── pases_espana.csv
│   ├── minutos_jugadores_espana.csv
│   ├── tiros_espana.csv
│   ├── regates_espana.csv
│   ├── duelos_espana.csv
│   └── despejes_espana.csv
```

---

## ▶️ Reproducción

Para reproducir el análisis es necesario disponer de **R** y de los paquetes utilizados en el proyecto.

Los datos deben encontrarse en la carpeta `data/` y las rutas utilizadas en los scripts deben ser relativas al repositorio.

Una vez instaladas las dependencias, el informe puede generarse ejecutando el archivo:

```text
report/Trabajo_Final_EC.Rmd
```

desde RStudio mediante la opción **Knit**.

---

## 👥 Autores

Proyecto académico desarrollado de forma colaborativa por:

* Ricard Castillo Moustakim
* Elena Fernández Caro
* Carlos Jiménez Ortega
* Daniel Prados Serrano
* Lourdes María Vargas Gamez
* Mateo Vega Pueyo

### Contribución personal

**Daniel Prados Serrano**

* Revisión y supervisión general de gran parte del proyecto.
* Desarrollo de una parte del análisis y las visualizaciones.
* Desarrollo de las visualizaciones animadas mediante `gganimate`.
* Revisión y refinamiento del código y de las representaciones gráficas.

> La contribución indicada refleja únicamente las tareas desarrolladas dentro del proyecto y no implica que el trabajo completo sea individual.

---

## 🎓 Contexto académico

Este repositorio contiene un **proyecto académico grupal** realizado como parte de una actividad de análisis y visualización de datos mediante R y R Markdown.

El proyecto se publica con fines **educativos y de portfolio**, manteniendo la autoría de todos los integrantes del grupo.

---

## 📄 Documentación

El análisis completo se encuentra disponible en el informe desarrollado en **R Markdown**, donde se explican tanto los conceptos utilizados como el código y la interpretación de las visualizaciones.

---

## 🚀 Objetivo del proyecto

El proyecto busca mostrar cómo los datos de eventos futbolísticos pueden transformarse en **visualizaciones útiles para analizar el rendimiento de un equipo**, pasando de datos estructurados a representaciones estadísticas, espaciales y temporales.

Más allá de las estadísticas individuales, el objetivo final es utilizar los datos para obtener una visión global del comportamiento de España durante la **Eurocopa 2024**.
