# Desafío TelecomX LATAM Parte 2:
Esta rama del repositorio contiene la segunda parte de desafío TelecomX, Vamos a mantener toda la primera parte del proyecto y ademas, se agregara nuevos preprocesamientos y análisis.

> **Proyecto Práctico de Data Science con Python**

Este proyecto forma parte del **Challenge Alura Store 2**. El objetivo principal es aplicar técnicas de análisis descriptivo y procesos `ETL` para resolver un problema de negocio real. 

## Propósito del Proyecto
La empresa enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes.
El propósito de este proyecto es recopilar, procesar y analizar los datos, utilizando Python y sus principales bibliotecas para extraer información valiosa. A partir de un análisis, se podrá avanzar en modelos predictivos y desarrollar estrategias para reducir la evasión.

## Tecnologías y Herramientas
* **Lenguaje:** Python 3
* **Manipulación de Datos:** Pandas, Numpy, JSON, SKLEARN
* **Visualización:** Matplotlib, Seaborn

## Estructura del Análisis

### 1. Extracción y Limpieza de Datos - Parte 1 del proyecto
Los datos se encuentran almacenados en un archivo JSON
* Se utilizó **Pandas** para la extracción de los datos.
* La biblioteca JSON se usa para normalizar y convertir en un **DataFrame** la base de datos.
* Limpieza de los datos nulos y datos que no aportan nada para nuestro entrenamiento

### Correlación y selección de variables.

Se analizan la Correlación de los datos con la variable que contiene la información de si el cliente cancelo sus servicios o no es el caso. Ademas, se eliminan columnas que no deberían aportar nada a los modelos.

### Modelación predictiva.

* Los datos se separan para el entrenamiento.
* Se crean dos modelo, uno que requiere datos normalizados (Regresión Logística) y otro que no lo requiere (Árbol de decisión).
* Se evalúan los modelos con diferentes métricas.

### Interpretación y Conclusiones
 *Se realiza un análisis de las variables mas importantes para los modelos. 
 *Se da un pequeño informe sobre los resultados obtenidos.


**Para saber mas del proyecto, lea el archivo de Informe_final.md**