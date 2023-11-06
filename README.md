# Título: Identificar pérdidas de energía no técnicas, mediante la reducción de casos de fraude, utilizando datos recopilados de inspecciones en un período de dos años.
## Documentación: Especialización en Analítica & Ciencia de Datos
## Autores: _Susana Álvarez, Luis Román_ 

### Requisitos

Asegúrate de tener instalado lo siguiente:

- tener Git : https://git-scm.com/
- Visual Studio : https://code.visualstudio.com/


## INTRODUCCIÓN

> Este repositorio contiene el notebook usado para el reprocesamiento de los datos crudos en la identificación de las perdidas no  técnicas de consumo de energía. La data original contiene 9105 registros y 377 variables numéricas. Para abordar este proyecto se usará 68 variables de interés. En la detección de instalaciones fraudulentas.

### Comandos de Git para descargar el proyecto:

```
git clone https://github.com/SusanaAlvarezC/Monografia
cd Monografia/
code .
```

#### Comandos de Git para contribuir con el proyecto:

* Para subir cambios al repositorio colaborativo, ir a Git Bash y ejecutar los siguientes comandos:
```
git add .
git commit -m "Descripción de tus cambios"
git push
```

## Ejecutar el script desde el navegador

https://colab.research.google.com/drive/1TIZTtkm0YYHBBmEIBcGBPnVyRyhJh_t0?usp=drive_link

1. Copia el anterior enlace en tu navegador.
2. Tener una cuenta de Google para usar Colab:


## Implementación

Se utilizó la librería “requests” en Python para hacer una solicitud HTTP a la ubicación del conjunto de datos en GitHub y usarlo en el procesamiento de datos crudos. Y así convertir el contenido descargado a un objeto StringIO para poder leerlo como archivo .CSV


## Tratamiento de datos

Para la manipulacion de los datos se usaron las librerias pandas, numpy, math, matplotlib y seaborn de Python para realizar una limpieza de datos, eliminando los valores atípicos, imputando los valores faltantes y remplazandolos por la media. También se implementaron gráficos de dispersión y matriz de correlación para observar como se comportaban la variables.   


## Hallazgos

?
