# Título: Identificar pérdidas de energía no técnicas, mediante la reducción de casos de fraude, utilizando datos recopilados de inspecciones en un período de dos años.
## Documentación: Especialización en Analítica & Ciencia de Datos
## Autores: _Susana Álvarez, Luis Román_ 

## INTRODUCCIÓN

> Este repositorio contiene el notebook usado para el procesamiento de los datos crudos en la identificación de las perdidas no técnicas de consumo de energía. Durante el proceso de limpieza de datos, se llevó a cabo una significativa reducción del conjunto original que constaba de 377 variables numéricas y 9105 registros, quedando finalmente con 68 variables y 9101 registros. Las estrategias empleadas se centraron en:

    * Tratamiento de valores nulos.
    * Eliminación de duplicados y variables numéricas con valores en 0.
    * Remoción de aquellas variables que mostraban una alta correlación.


## EJECUCIÓN CÓDIGO

### Ejecutar el script desde colaboratory

1. Ingrese al siguiente enlace: [https://colab.research.google.com/drive/1TIZTtkm0YYHBBmEIBcGBPnVyRyhJh_t0?usp=drive_link](https://colab.research.google.com/drive/1TWlhyVF5E8TiixklycfyGWNnayIAZoiZ?usp=sharing)
2. Ejecute linea por linea para seguir la secuencia de código

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
