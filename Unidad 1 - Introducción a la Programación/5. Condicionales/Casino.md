---
tags: [Condicionales, Funciones, Programa Interactivo]
---

# El casino de dudosa legalidad 🎲🎲

En el piso -2 del casino 🍝 de la facultad, hay un casino 🎰, en donde se hacen diversos tipos de apuestas de dudosa ética, como poner en juego décimas para los controles o dinero para el almuerzo de un estudiante. Uno de estos juegos consiste en apostar al resultado del lanzamiento de dos dados, en donde dependiendo del resultado:

- Si el valor en ambos dados es el mismo (ej: en ambos se obtuvo un 3), entonces se gana `2.0x` veces lo apostado.

  - En particular, si en ambos dados se obtuvo un 4, entonces se gana `4.0x` veces lo apostado (ya que aprobaste milagrosamente).

- Si la diferencia entre los valores de los dados es exactamente 2 (ej: un 3 y un 5), entonces se gana `1.5x` lo apostado.

- En cualquier otro caso, lo pierdes todo 😥 

Para estudiar que tan probable es que pueda ganar en este juego, decide programar algunas funciones y programas, que permitan emular este juego, sin poner en riesgo sus finanzas y sus décimas. Para ello:

1. Cree una función llamada ```lanzarDado()```, la cual no recibe parámetros, pero entrega aleatoriamente un número entero entre 1 y 6, que representa el lanzamiento de un dado. Ejemplo:

     - ```lanzarDado()``` podría entregar ```3```

2. Cree un programa interactivo, que simule el casino de acuerdo a los siguientes diálogos:


    ```python 
    >>  Ingrese monto a apostar: 3000

      Al lanzar los dados se obtuvo... 2 y 4
      Has ganado 4500 pesos 🤑
    ```
    ```python 
    >>  Ingrese monto a apostar: 4000
    
      Al lanzar los dados se obtuvo... 1 y 6
      Lo has perdido todo 😥
    ```

    Indicaciones:
    - Recuerde pedir el monto a apostar mediante ```input()```
    - Revise adecuadamente todas las condiciones y escenarios posibles de respuesta.