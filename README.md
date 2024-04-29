# VegetableImage
Tags: Python, TensorFlow, Neural Networks, Vegetable Image Dataset


<br>

---




## Introducción

### **Objetivo**

En este proyecto, se **evaluarán y compararán 2 estrategias** para la **Clasificación de Imágenes** empleando el **`Vegetable Image Dataset`**.

La propuesta de solución estará basada en **Redes Neuronales Convolucionales** (**CNNs**).




#### **Pipeline**

1.   **Carga** del conjunto de datos

2.   **Inspección** del conjunto de datos

3.   **Acondicionamiento** del conjunto de datos

4.   Desarrollo de la **arquitectura** de red neuronal y **entrenamiento** de la solución

5.   **Monitorización** del proceso de **entrenamiento** para la toma de decisiones

6.   **Evaluación** del modelo predictivo y planteamiento de la siguiente prueba experimental




### **Estrategia 1: Entrenar desde Cero (From Scratch)**

La primera estrategia a comparar será una **Red Neuronal Profunda**.

Se expondrán la Arquitectura y los Hiperparámetros utilizados, y se aplicarán técnicas de **Regularización** para la mejora del rendimiento de la Red Neuronal tales como *weight regularization*, *dropout*, *batch normalization*, *data augmentation*, etc.


### **Estrategia 2: Usar Red Pre-entrenada**

La segunda estrategia utilizará una **Red Pre-entrenada** con el dataset **`ImageNet`**, llevando a cabo tareas de ***Transfer Learning*** y ***Fine-Tuning*** para resolver la tarea de clasificación.

Se compararán al menos **2 tipos de Arquitecturas** entre las disponibles: VGGs, ResNet50, Xception, InceptionV3, InceptionResNetV2, MobileNetV2, DenseNet, ResNet. Y se seleccionará la que mayor precisión proporcione.
(Información sobre las arquitecturas disponibles en https://keras.io/applications/).

De forma similar al procedimiento en la Estrategia 1, también se aplicarán técnicas de **Regularización** para la mejora del rendimiento de la Red Neuronal tales como *weight regularization*, *dropout*, *batch normalization*, *data augmentation*, etc.



<br>

---



## **Descripción**

La siguiente información es extraída del repositorio de Kaggle donde se almacena el **`Vegetable Image Dataset`** original (https://www.kaggle.com/datasets/misrakahmed/vegetable-image-dataset).


### **Dataset: Vegetable Image Dataset**

Clasificación y reconocimiento de vegetales



### **Contexto**

-  El experimento inicial se realiza con 15 tipos de hortalizas comunes en todo el mundo. Las verduras elegidas para el experimento son: judía, calabaza amarga, calabaza de botella, berenjena, brécol, col, pimiento, zanahoria, coliflor, pepino, papaya, patata, calabaza, rábano y tomate. Se utiliza un total de **21000** imágenes de **15 clases**, cada una de las cuales contiene 1400 imágenes de tamaño $224×224$ y en formato `*.jpg`.

-  El conjunto de datos se divide en un 70% para el entrenamiento, un 15% para la validación y un 15% para las pruebas.



### **Contenido**

Este dataset contiene 3 carpetas:

- **`train`**: 15000 imágenes
- **`test`**: 3000 imágenes
- **`validation`**: 3000 imágenes

Cada una de las carpetas anteriores contiene subcarpetas para distintos vegetales en las que están presentes las imágenes de los vegetales/hortalizas respectivos.

De acuerdo con lo anterior, las 15 clases son las siguientes:

**`Y = ['Bean', 'Bitter Gourd', 'Bottle Gourd', 'Brinjal', 'Broccoli', 'Cabbage', 'Capsicum', 'Carrot', 'Cauliflower', 'Cucumber', 'Papaya', 'Potato', 'Pumpkin', 'Radish', 'Tomato']`**


<br>

---



## **Ejecución**

*No será posible ejecutar todos los modelos en una misma sesión de Colab.*

- Lo anterior se debe a las limitaciones con la memoria RAM. Incluso, *tampoco es posible* ejecutar todos los modelos en una misma sesión usando una cuenta de Colab Pro.

Por lo tanto, debido a esta limitantes, se han incluido para cada modelo, las **instrucciones** para su correcta ejecución desde el entorno de **Google Colab**, que básicamente consisten (salvo que se especifique otra cosa) en ejecutar las Secciones:

1. Carga del Dataset.
2. Inspección del Dataset
3. Y en ocasiones el Acondicionamiento del Dataset.

Luego, se continuaría con la Sección específica del modelo que se desea ejecutar.


















