# Reto Arca Continental
---

## En que consiste
<center>
     
Este repositorio contiene archivos utilizados para resolver la problemática que se nos planteo por parte de la empresa Arca Continental, donde el objetivo era crear un framework, en donde aplicaramos nuestros conocimiento de Inteligencia Artifical, para crear anuncios que se pudieran colocar en tiendas de México, para esto, nuestra solución plantea lo siguiente:

El usuario inicia el proceso en una interfaz intuitiva, generando prompts a través de la aplicación.
ChatGPT-3.5, modificado con una fórmula mejorada para la generación de prompts efectivos, responde
proporcionando sugerencias creativas.
En la siguiente etapa, el usuario revisa y selecciona el prompt más adecuado, junto con el token del objeto
a formar (por ejemplo, “sks - coca-cola” o “sfk - sprite”). Esta combinación se convierte en la entrada precisa
para el modelo de generación de imágenes.
La interfaz de usuario Automatic1111 entra en juego, sirviendo como plataforma para ingresar los prompts
y tokens seleccionados. Aquí, se inicia el modelo entrenado específicamente para la generación de imágenes
de botellas de refresco, utilizando la potente tecnología SDXL (Stable Diffusion XL).
El resultado de este proceso es una imagen generada, que el usuario tendrá que transferir a Microsoft
Designer para su edición y personalización. En este paso, los usuarios pueden realizar modificaciones, agregar
texto u otros elementos gráficos según sus necesidades específicas.

</center>

---
## Miembros

**César Alejandro Cruz Salas**

**Francisco José Joven Sánchez**

**David Emiliano Mireles Cárdenas**

**Marlon Brandon Romo López**

**Mario Javier Soriano Aguilera**
---
#### **Recopilación de potenciales modelos generativos**: 9 de octubre del 2023
En esta parte se hizo lo siguiente: 
*  Plantear los Objetivos de las investigacion:
      * Analizar la eficacia y versatilidad de la metodología propuesta para la creación de
        anuncios publicitarios
      * Evaluar la precisión y capacidad de adaptación del chatbot en la definición detallada
        de la disposición de elementos visuales y textuales en el anuncio.
      * Investigar la eficiencia y calidad de los modelos generativos en la creación de la
        plantilla del fondo del anuncio, la representación de productos a exhibir y la
        generación de texto específico.

*  Los requerimentos para los modelos investigados fueron:
      * Ingresar datos de entrada iniciales: El usuario debe introducir usando lenguaje natural
        los datos descriptivos del resultado que se desea.
      * Seleccionar resultados del proceso de imagen: El usuario seleccionará entre las opciones
        producidas para el tercer paso que consiste en generar varias imágenes que pueden encajar con
        la descripción del diseño del producto.
      * Corregir apartados del anuncio: El usuario será capaz de modificar la imagen final
        siempre y cuando esto esté dentro de las capacidades del programa para llenar espacios vacíos.
      * Que los modelos sean Open-Source para poder modificarlos y usarlos libremente.

  * Mejores modelos:
      * GPT-2: Chatbot de gran modelo de lenguaje preentrenado de OpenAI.
      * Llama-2: Llama 2 es un modelo de lenguaje grande (LLM) desarrollado por Meta AI.
      * Microsoft-Designer: Microsoft Designer es una aplicación de diseño gráfico para crear contenido profesional.
      * Stable Diffusion SDXL: Este modelo es de los más recientes lanzados por Stable Diffusion, está entrenado con 
        muchos más parámetros y su característica es que es capaz de hacer letras correctamente en la generación de 
        imagen.
  
**Nota:** Para saber mas acerca de esta investigacion ir a la carpeta de Docs del repositorio.

### **Propuesta de solución al reto**: 15 de octubre del 2023

* Arquitectura de la Solución
La solución propuesta es la siguiente:
     - El usuario presenta una idea general.
     - El chatbot permite la especificación precisa de la disposición de elementos visuales
       y textuales.
     - Dos modelos generativos se utilizan en paralelo: uno para crear la plantilla del
       anuncio y otro para generar las imágenes necesarias, como productos, personas o
       fondos.
     - Un modelo adicional genera el texto específico del anuncio.
       
**Nota:** Para saber mas acerca de la primera solucion planetada ir a la carpeta de Docs al archivo de "Propuesta de solución al reto" del repositorio.

### **Primer MVP**
En la carpeta de nombre Primer_MVP_models, se pueden encontrar los notebooks utilizados para los primeros modelos de prueba, en donde se propuso usar LLama-2 como chatbot, el modelo SDXL para generar las imágenes de los productos asi como de de los fondos de los anuncios, y finalmente se encuentra un notebook que utiliza fontjoy como creador y editor de texto. 

**Nota:** Para saber mas acerca del primer mvp favor de ir en la carpeta de Docs al arhivo de "Primer MVP" del repositorio.

### **Segundo MVP y entrega final**

* En esta etapa terminamos de hacer las pruebas y encontramos los mejores modelos:
     * Chatgpt-3.5: Se cambio a chatgpt-3.5 debido a que es un modelo que gana en todas las métricas a llama-2 y no          requiere hosting.
     * Stable-difussion (SDXL): Se mantuvo el uso de SDXL, para generar las images se hizo fine-tuning al modelo con         el entrenamiento Dreambooth-LoRA, se utilizó un script para poder usar los LoRA en AUTOMATIC1111. Se                   entrenaron un total de 4 modelos LoRA, para Coca-cola,Sprite, fanta y fondos para el anuncio.
     * Automatic111: Proponemos AUTOMATIC1111 como graphical user interface (GUI).
     * STEFANN: Con esta combinación de redes neuronales, se puede modificar el texto de las imágenes generadas con SDXL.
     * Microsofts Designer: Uso de Microsoft Designer para agregar texto, quitar fondos de imágenes, juntar los              fondos con las imagenes de los productos y refinamientos que se tengan que implementar en el anuncio.

**Nota:** Se recomienda ir a la carpeta de "Entrega Final" al ar pdf con el mismo nombre,para ver toda la propuesta de solución y resultados.






      






