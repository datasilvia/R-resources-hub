# 🖥️ Introducción a Shiny

**Shiny** es un paquete de R que permite crear aplicaciones web interactivas directamente desde R.

---

## 🧠 ¿Para qué sirve?

Con Shiny puedes:

- Crear dashboards interactivos  
- Construir aplicaciones web  
- Visualizar datos en tiempo real  
- Compartir análisis sin necesidad de saber JavaScript  

---

## 🚀 Ejemplo básico

```r
library(shiny)

ui <- fluidPage(
  titlePanel("Mi primera app"),
  sliderInput("num", "Elige un número:", 1, 100, 50),
  textOutput("resultado")
)

server <- function(input, output) {
  output$resultado <- renderText({
    paste("Has elegido:", input$num)
  })
}

shinyApp(ui = ui, server = server)
```

---

## 🧩 Cómo funciona

Shiny tiene dos partes:

- **UI (User Interface)** → lo que ve el usuario  
- **Server** → la lógica de la aplicación  

---

## ✨ Ventajas

- No necesitas conocimientos de frontend  
- Muy potente para prototipos  
- Ideal para data science  

---

## ⚠️ Limitaciones

- Puede ser lento con grandes volúmenes de datos  
- No sustituye a frameworks web completos  
- Escalar aplicaciones complejas puede ser difícil  

---

## 🌐 Cómo compartir una app

Puedes desplegar tu app en:

- Posit Connect (de pago)  
- shinyapps.io  
- tu propio servidor  

---

## 💡 Resumen

- Shiny permite crear apps web con R  
- Es ideal para dashboards y visualización
  
- Muy usado en análisis de datos  

---
