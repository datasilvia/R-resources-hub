# 📦 Guía de packages de R

Una guía rápida para entender qué son los paquetes de R, cómo instalarlos y cuáles usar según el tipo de tarea.

---

## 🧠 ¿Qué es un package en R?

Un **package** es una colección de funciones, datos y documentación que amplía las capacidades de R.

R ya incluye funciones básicas, pero los packages permiten trabajar de forma más cómoda con:

- limpieza de datos
- visualización
- modelos estadísticos
- machine learning
- reporting
- conexión con APIs
- aplicaciones interactivas

---

## 📥 Cómo instalar un package

La forma más común es instalarlo desde CRAN:

```r
install.packages("nombre_del_paquete")
```

Por ejemplo:

```r
install.packages("tidyverse")
```

Después de instalarlo, hay que cargarlo:

```r
library(tidyverse)
```

---

## 🧰 Packages esenciales

| Package | ¿Para qué sirve? | Cuándo usarlo |
|---|---|---|
| `tidyverse` | Colección de paquetes para data science | Casi siempre |
| `dplyr` | Manipulación de datos | Filtrar, ordenar, agrupar |
| `ggplot2` | Visualización de datos | Crear gráficos |
| `readr` | Importar datos | Leer CSV |
| `tidyr` | Ordenar y transformar datos | Reformatear tablas |
| `stringr` | Trabajar con texto | Limpiar strings |
| `lubridate` | Fechas y horas | Trabajar con fechas |
| `shiny` | Apps web interactivas | Crear dashboards/apps |
| `rmarkdown` | Informes reproducibles | Crear documentos con código |

---

## 🧭 Packages según tarea

### 🧹 Limpieza y transformación de datos

- `dplyr`
- `tidyr`
- `janitor`
- `stringr`

### 📊 Visualización

- `ggplot2`
- `plotly`
- `leaflet`
- `highcharter`

### 📥 Importar y exportar datos

- `readr`
- `readxl`
- `writexl`
- `jsonlite`
- `DBI`

### 📅 Fechas y texto

- `lubridate`
- `stringr`
- `forcats`

### 📈 Estadística y modelado

- `stats`
- `broom`
- `caret`
- `tidymodels`

### 🤖 Machine Learning

- `tidymodels`
- `caret`
- `randomForest`
- `xgboost`

### 🌐 APIs, scraping y web

- `httr2`
- `rvest`
- `jsonlite`

### 🖥️ Apps y dashboards

- `shiny`
- `shinydashboard`
- `flexdashboard`

### 📄 Reporting

- `rmarkdown`
- `knitr`
- `quarto`

---

## ⭐ Recomendación para principiantes

Si estás empezando, no intentes aprender todos los packages a la vez.

Empieza con:

1. `tidyverse`
2. `dplyr`
3. `ggplot2`
4. `readr`
5. `shiny`

Con eso ya puedes hacer muchísimos proyectos reales.

---

## 🧪 Ejemplo básico

```r
install.packages("tidyverse")
library(tidyverse)

datos <- read_csv("data.csv")

datos_limpios <- datos %>%
  filter(!is.na(variable)) %>%
  group_by(categoria) %>%
  summarise(total = sum(valor))
```

---

## 📚 Guías relacionadas

- [Qué es CRAN](../que-es-cran.md)
- [Qué es tidyverse](../que-es-tidyverse.md)
- [Introducción a Shiny](../intro-a-shiny.md)

---

## 🚧 En progreso

Esta guía irá creciendo con explicaciones más detalladas de cada package.
