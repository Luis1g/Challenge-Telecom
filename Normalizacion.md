# **Normalización en modelos lineales**
--- 

La **Regresión Logística** (y los modelos lineales en general) calcula una suma ponderada de las variables de entrada. El modelo intenta encontrar el mejor valor para cada coeficiente ($\beta$) en la ecuación:

$$z = \beta_0 + \beta_1x_1 + \beta_2x_2 + ... + \beta_nx_n$$

Entonces, ¿Por qué necesitamos normalizar los datos para el modelo de Regresión Logística?

1. Comparabilidad de coeficientes: Si tenemos una variable Cargos_Totales que va de 0 a 8,000 y una variable Antigüedad que va de 0 a 72, el modelo tendrá que asignar un coeficiente muy pequeño a los cargos y uno muy grande a la antigüedad solo para equilibrar las escalas. Al normalizar, todas las variables tienen valores en el mismo rango (por ejemplo, de 0 a 1), permitiéndote decir con seguridad: "La variable con el coeficiente más alto es la más importante".

2. Convergencia del Gradiente: Para entrenar el modelo, se utiliza un algoritmo llamado Descenso de Gradiente. Si las escalas son distintas, el espacio de búsqueda se vuelve una elipse muy alargada y "curva", lo que hace que el algoritmo oscile y tarde mucho más en encontrar el mínimo error. Con datos normalizados, el espacio es circular y el modelo llega a la solución óptima mucho más rápido.


A diferencia de la logística, el **Árbol de Decisión** no multiplica las variables por pesos. Su funcionamiento se basa en reglas de partición.

* Selección por orden: El árbol busca el mejor punto de corte en cada variable basándose en la ganancia de información (o Índice Gini). Por ejemplo, dirá: "Si Cargos_Totales > 500, ve a la izquierda".

* Invariancia a transformaciones monótonas: Si multiplicas todos los Cargos_Totales por 1,000, el árbol simplemente moverá su punto de corte de 500 a 500,000. La estructura del árbol y la lógica de la decisión no cambian en absoluto.

* Aislamiento de variables: Cada nodo del árbol analiza una sola variable a la vez. No intenta combinar Cargos con Antigüedad en una sola ecuación matemática, por lo que no le importa si una está en miles y la otra en decimales.

---