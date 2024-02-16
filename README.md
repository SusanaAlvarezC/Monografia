Laboratory I - Dimensionality Reduction. Machine Learning II


Data structures (properties of lists, tuples, dicts, built-in modules...)
- Classes
- Packages and modules

# Title: Laboratory I - Dimensionality Reduction. Machine Learning II
## Prerequisites: Data structures (properties of lists, tuples, dicts, built-in modules. Classes, Packages and modules

## INTRODUCTION

> This workshop is structured into ten thematic areas, each focusing on different aspects of data analysis and machine learning. We will start by generating random rectangular matrices and performing basic matrix operations. Then, we will move on to image processing, where we will manipulate and analyze facial images. Following that, we will dive into the implementation of unsupervised learning algorithms, including Singular Value Decomposition (SVD), Principal Component Analysis (PCA), and t-distributed Stochastic Neighbor Embedding (t-SNE).:

    * Tratamiento de valores nulos.
    * Eliminación de duplicados y variables numéricas con valores en 0.
    * Remoción de aquellas variables que mostraban una alta correlación.

Sábana original de datos: https://github.com/SusanaAlvarezC/Monografia/blob/main/consumos_energia.csv 

## EJECUCIÓN CÓDIGO

### Ejecutar el script desde colaboratory

1. Ingrese al siguiente enlace: [https://colab.research.google.com/drive/1TIZTtkm0YYHBBmEIBcGBPnVyRyhJh_t0?usp=drive_link](https://colab.research.google.com/drive/1TWlhyVF5E8TiixklycfyGWNnayIAZoiZ?usp=sharing)
2. Ejecute linea por linea para seguir la secuencia de código

Código: https://github.com/SusanaAlvarezC/Monografia/blob/main/Monograf%C3%ADaDetecci%C3%B3nFraudes.ipynb

## COLABORACIÓN 

### Requisitos

Se debe tener instalado lo siguiente:

- Git : https://git-scm.com/
- Visual Studio : https://code.visualstudio.com/

### Comandos de Git para descargar el proyecto:

```
git clone https://github.com/SusanaAlvarezC/Monografia
cd Monografia/
code .
```

### Comandos de Git para contribuir con el proyecto:

* Para subir cambios al repositorio colaborativo, ir a Git Bash y ejecutar los siguientes comandos:
```
git add .
git commit -m "Descripción de cambios"
git push
```

## Implementación

Se utilizó la librería “requests” en Python para hacer una solicitud HTTP a la ubicación del conjunto de datos en GitHub y usarlo en el procesamiento de datos crudos. Y así convertir el contenido descargado a un objeto StringIO para poder leerlo como archivo .CSV


### Tratamiento de datos

Para la manipulacion de los datos se usaron las librerias pandas, numpy, math, matplotlib y seaborn de Python para realizar una limpieza de datos, eliminando los valores atípicos, imputando los valores faltantes y remplazandolos por la media. También se implementaron gráficos de dispersión y matriz de correlación para observar como se comportaban la variables.   


### Hallazgos

En el tratamiento de datos se evidenció que la variable de salida "was_fraud" presenta un sobre muestreo. Por tal motivo se igualó la variable minoritaria para balancear el número de muestras entre las diferentes clases y así poder entrenar mejor el modelo seleccionado.


Resultado despúes del tratamienteo de datos: https://github.com/SusanaAlvarezC/Monografia/blob/main/resultado_final_consumos.csv
