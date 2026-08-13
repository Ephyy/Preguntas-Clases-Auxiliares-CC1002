---
tags: [Condicionales, Funciones, Programa Interactivo]
---

# Cuidando la Salud 

Un día Clara, en sus clases de programación aplicada a la biomedicina, se encontró con una temática súper interesante. Uno de los indicadores más utilizados para ver si una persona está con sobrepeso o no es el Índice de Masa Corporal (IMC), que se obtiene con la siguiente formula:

$$ IMC = \frac{peso}{altura^2}\left[\frac{kg}{m^2}\right] $$

Por lo que luego de esta clase, Clara se propuso la misión de hacer un programa computacional que motive a las personas a tener consciencia de su estado de salud, para lo cual le ayudaremos con lo siguiente:

1. Cree la función ```imc(peso, altura)```, que recibe dos números positivos que son el peso (en kg) y
altura (en m) de una persona, y retorna un texto dependiendo del valor del 𝐼𝑀𝐶:

   - Menos de 18.5 → `"Peso bajo"`
   - Entre 18.5 y 24.9 → `"Peso normal"`
   - Entre 25.0 y 29.9 → `"Sobrepeso"`
   - Entre 30.0 y 34.9 → `"Obesidad Leve"`
   - Entre 35.0 y 39.9 → `"Obesidad Moderada"`
   - 40.0 o más → `"Obesidad Severa"`

   Ejemplos:
   - ```imc(65, 1.70)``` entrega ```"Peso normal"```
   - ```imc(85, 1.75)``` entrega ```"Sobrepeso"```


1. Cree un programa interactivo, donde con ayuda de la función anterior, construya un programa de acuerdo al siguiente diálogo de ejemplo:

    ```python
    Vamos a calcular tu IMC y ver tu estado de salud 

    Ingrese peso (kg): ___
    Ingrese altura (m): ___

    Tu estado de salud es: ___
    ```

    - Indicación: Puede asumir que los valores a ingresar serán numéricos, pero no necesariamente valores mayores que 0. Maneje adecuadamente este escenario adverso antes de ejecutar el flujo esperado del programa anterior.