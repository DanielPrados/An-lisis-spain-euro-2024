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

## 📊 Fuente de datos

Los datos utilizados en este proyecto proceden de **StatsBomb** y corresponden a los eventos registrados durante los partidos disputados por España en la Eurocopa 2024.

El conjunto de datos contiene información detallada sobre las acciones desarrolladas durante los encuentros, incluyendo:

* Pases y su precisión.
* Tiros y goles.
* Expected Goals (xG).
* Regates.
* Duelos.
* Despejes.
* Localización espacial de las acciones.
* Información temporal de los eventos.

A partir de estos datos se realizaron los procesos de limpieza, transformación y análisis necesarios para construir las visualizaciones y animaciones incluidas en el proyecto.

> **Fuente:** StatsBomb — datos de eventos de la Eurocopa 2024.


## 🛠️ Tecnologías utilizadas

El proyecto ha sido desarrollado principalmente utilizando:

* **R**
* **R Markdown**
* **ggplot2** — visualización de datos.
* **gganimate** — visualizaciones y animaciones dinámicas.
* **ggsoccer** — representación de acciones sobre el terreno de juego.
* **dplyr** — manipulación y transformación de datos.
* **tidyr** — organización y transformación de datos.
* **readr** — importación de datos.
* **ggrepel** — posicionamiento de etiquetas en gráficos.
* **gifski** — generación de archivos GIF.

---

## 📊 Análisis realizado

El proyecto aborda diferentes dimensiones del rendimiento de España durante la Eurocopa 2024.

### ⚽ Pases

Se analiza la cantidad y precisión de los pases realizados por los jugadores, incluyendo su estandarización en función de los minutos disputados para facilitar las comparaciones entre jugadores.

También se estudia la **distribución espacial de los pases** sobre el terreno de juego.

### 🎯 Tiros y goles esperados

Se estudian los disparos realizados durante el torneo y su localización en el campo.

Además, se utiliza la métrica **xG (Expected Goals)** para analizar la calidad de las ocasiones generadas y su evolución a lo largo de los partidos.

### 🏃 Regates

Se analiza la distribución de los regates realizados y completados por los jugadores, así como su localización sobre el terreno de juego.

### 🤝 Duelos

Se estudian los duelos disputados y ganados por los jugadores españoles, utilizando representaciones espaciales para identificar las zonas del campo donde se producen con mayor frecuencia.

### 🛡️ Despejes

Se analiza la distribución de los despejes realizados por España durante el torneo y las zonas del campo en las que se producen.

### 🗺️ Análisis espacial

Una parte importante del proyecto consiste en representar las acciones directamente sobre el terreno de juego.

Se utilizan diferentes mapas y representaciones espaciales para identificar:

* Zonas de mayor concentración de acciones.
* Distribución de pases.
* Localización de disparos.
* Distribución de regates.
* Localización de duelos.
* Zonas de realización de despejes.

### 🔴 Comparación con los rivales

Los datos de España se comparan con los de sus rivales a lo largo de la competición para estudiar diferentes aspectos del rendimiento y del comportamiento de los equipos.

---

## 🎞️ Visualizaciones animadas

El proyecto incorpora **visualizaciones animadas mediante `gganimate`**, permitiendo representar de forma dinámica la evolución de determinadas acciones sobre el terreno de juego.

Entre ellas se encuentra una recreación animada del **gol de Mikel Oyarzabal frente a Inglaterra en la final de la Eurocopa 2024**, representando los movimientos de los jugadores, la trayectoria del balón y la finalización de la jugada.

Estas visualizaciones permiten complementar los análisis estáticos y facilitar la interpretación de determinadas secuencias de juego.

---

## 📁 Estructura del repositorio

```text
analisis-spain-euro-2024/
│
├── README.md
│
├── report/
│   ├── Trabajo_Final_EC.Rmd
│   └── Trabajo_Final_EC.html
│
└── data/
    ├── pases_espana.csv
    ├── minutos_jugadores_espana.csv
    ├── tiros_espana.csv
    ├── regates_espana.csv
    ├── duelos_espana.csv
    └── despejes_espana.csv
```

---

## ▶️ Reproducción

Para reproducir el análisis:

1. Clonar o descargar el repositorio.
2. Abrir el archivo `Trabajo_Final_EC.Rmd` situado en la carpeta `report/`.
3. Instalar las librerías necesarias si no están disponibles.
4. Ejecutar el documento mediante **Knit** en RStudio.

El documento R Markdown contiene tanto el código utilizado para el análisis como las visualizaciones generadas.

---

## 👥 Autores

Proyecto desarrollado conjuntamente por:

* **Ricard Castillo Moustakim**
* **Elena Fernández Caro**
* **Carlos Jiménez Ortega**
* **Daniel Prados Serrano**
* **Lourdes María Vargas Gamez**
* **Mateo Vega Pueyo**

---

## 👤 Contribución personal

Mi participación en el proyecto incluyó:

* Participación en el desarrollo y revisión de gran parte del análisis.
* Desarrollo de una parte significativa de las visualizaciones y del código del proyecto.
* Desarrollo íntegro de las **visualizaciones animadas mediante `gganimate`**.
* Revisión, depuración y refinamiento del código y de las representaciones gráficas.
* Revisión general del informe y de los resultados obtenidos.

---

## 🎓 Contexto académico

Este proyecto fue desarrollado como parte de un **trabajo académico de análisis y visualización de datos**, utilizando herramientas del ecosistema de R para explorar y representar datos relacionados con el fútbol.

El proyecto combina programación, análisis de datos, estadística y visualización para estudiar el rendimiento de la Selección Española durante la **UEFA Euro 2024**.

---

## 📄 Documentación

El análisis completo, junto con el código utilizado para generar las visualizaciones, se encuentra disponible en:

```text
report/Trabajo_Final_EC.Rmd
```

También se incluye una versión HTML renderizada del informe:

```text
report/Trabajo_Final_EC.html
```

---

## 🎯 Objetivo

El objetivo principal del proyecto es mostrar cómo las técnicas de **análisis y visualización de datos pueden utilizarse para estudiar el rendimiento deportivo**, transformando datos de eventos de fútbol en representaciones visuales que permitan identificar patrones, tendencias y comportamientos sobre el terreno de juego.

En este caso, el análisis se centra en el recorrido de **España durante la Eurocopa 2024**, utilizando los datos para explorar cómo se desarrolló su juego y cómo se comportó frente a sus rivales.

## 📈 Algunas visualizaciones

- Pases hacia delante España vs. Croacia: 
<img width="672" height="480" alt="image" src="https://github.com/user-attachments/assets/3b476e8a-0d13-4cea-9eed-8eb88d701659" />

- xG acumulado por minuto en semifinal y final: 
<img width="850" height="450" alt="xg_espana_euro2024" src="https://github.com/user-attachments/assets/ff51a47b-881d-49df-95f8-15d829a4d279" />

- Gol de Lamine Yamal vs. Francia: <img width="950" height="620" alt="gol_lamine_yamal" src="https://github.com/user-attachments/assets/92487496-8121-452f-b7b8-68a9573a16a7" />


