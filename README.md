# Desafío TelecomX LATAM:

> **Proyecto Práctico de Data Science con Python**

Este proyecto forma parte del **Challenge Alura Store 2**. El objetivo principal es aplicar técnicas de análisis descriptivo y procesos `ETL` para resolver un problema de negocio real. 

## Propósito del Proyecto
La empresa enfrenta una alta tasa de cancelaciones y necesita comprender los factores que llevan a la pérdida de clientes.
El propósito de este proyecto es recopilar, procesar y analizar los datos, utilizando Python y sus principales bibliotecas para extraer información valiosa. A partir de un análisis, se podrá avanzar en modelos predictivos y desarrollar estrategias para reducir la evasión.

## Tecnologías y Herramientas
* **Lenguaje:** Python 3
* **Manipulación de Datos:** Pandas, Numpy, JSON
* **Visualización:** Matplotlib, Seaborn

## Estructura del Análisis

### 1. Extracción y Limpieza de Datos
Los datos se encuentran almacenados en un archivo JSON
* Se utilizó **Pandas** para la extracción de los datos.
* La biblioteca JSON se usa para normalizar y convertir en un **DataFrame** la base de datos.

### 2. Porcentaje de evasión

Se grafican la cantidad de clientes que cancelaron y su plan, versus los clientes que permanecieron con su plan.

### 3. Análisis de evasión
El estudio se centró en comparar el comportamiento de los clientes (Evasión) con respecto diferentes variables:

* Género del cliente 
* Método de pago
* Cargo Total.
* Tipo de contrato.
* Tiempo de contrato.

### 4. Matriz de correlación

Se analiza la correlación que existe entre diferentes variables y la evasión de los clientes.

### 5. Informa

Se presenta un informe con los hallazgos más relevantes del desafío.