---
tags: [Funciones, Programa Interactivo]
---

# Pizzas

En la pizzería «Pizzas infinitas», donde no hay límite para el sabor, tienen la particularidad de que puedes elegir el radio que quieras que tenga tu pizza. Así es, puedes pedir pizzas de 17.5cm, 22.8cm o incluso 3.14cm, y obviamente el precio de la pizza aumenta con su tamaño, pero también aumenta la felicidad de sus clientes.

Luigi, el dueño del local, tiene la siguiente formula para calcular la cantidad de salsa a utilizar en una pizza:

$$ Salsa = \pi \cdot ln(r + 1)^{2} \cdot 10 $$

1. Al respecto, cree la función llamada ```salsa(r)```, que calcula la cantidad de salsa a utilizar, en función del radio $r$ de la pizza. Redondee el resultado final a 2 decimales.

2. Haga un programa interactivo, estableciendo el siguiente dialogo:

    ```python
    Ingrese el radio (cm) de la pizza: ___
    Necesitas [cantidad salsa] de salsa para la pizza.
    ```

