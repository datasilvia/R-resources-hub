# 🧹 ¿Qué es tidyverse?

**tidyverse** es una colección de paquetes de R diseñada para trabajar con datos de forma más clara, coherente y eficiente.

Es uno de los ecosistemas más importantes en data science con R.

---

## 🧠 ¿Por qué es importante?

Antes de tidyverse, muchas operaciones en R eran:

- menos intuitivas
- más difíciles de leer
- inconsistentes entre funciones

tidyverse soluciona esto con:

👉 una forma de trabajar más lógica y uniforme

---

## 📦 ¿Qué incluye tidyverse?

Cuando instalas:

```r
install.packages("tidyverse")
```

Obtienes varios paquetes, entre ellos:

- `dplyr` → manipulación de datos  
- `ggplot2` → visualización  
- `readr` → importar datos  
- `tidyr` → transformar datos  
- `stringr` → trabajar con texto  
- `forcats` → factores  

---

## 🧩 Ejemplo básico

```r
library(tidyverse)

datos <- read_csv("data.csv")

datos %>%
  filter(!is.na(variable)) %>%
  group_by(categoria) %>%
  summarise(total = sum(valor))
```

---

## ✨ Ventajas

- Código más legible  
- Funciones coherentes entre sí  
- Ideal para análisis de datos  
- Muy utilizado en el mundo profesional  

---

## ⚠️ Consideraciones

- No sustituye a todo R (es un ecosistema dentro de R)  
- Puede ocultar cómo funciona R internamente  

---

## 💡 Resumen

- tidyverse = conjunto de paquetes para data science  
- Hace R más fácil de usar
  
- Es una de las herramientas más importantes para trabajar con datos  

---
