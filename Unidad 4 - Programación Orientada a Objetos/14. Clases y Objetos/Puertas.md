---
tags: [Clases y Objetos]
---

# Concursos y Sorteos 🚪🚪💰

En el concurso de las puertas, se tiene un conjunto de `N` puertas, donde:

- En una de ellas, al azar, se esconde un gran premio (como un auto, una casa o mucho dinero).
- En una cantidad de `T` puertas (`1 <= T < N`) se esconde una trampa, que al encontrarla, automáticamente termina el concurso sin posibilidad de llevarse un premio.
- En las puertas restantes se esconde un premio monetario menor.

Entonces la idea de este concurso, es ir abriendo puertas, y decidir si arriesgarse o no a abrir una siguiente puerta, ya que podría contener un premio, o bien, ser una trampa que termina el concurso y dejando el premio en 0.

Vamos a construir una Clase, que nos permita modelar este tipo de concurso. La tabla de métodos es la siguiente:

| Método | Significado |
|---|---|
| ```P = Puertas(10, 3)``` | Crea un concurso de las puertas, con 10 puertas, y 3 de ellas quedan con una trampa. |
| ```P.abrirPuerta(2)``` | Abre la puerta número 2. Dependiendo del contenido de la puerta, entrega el string: ```"premio"```, ```"gran premio"``` o ```"trampa"```. |
| ```P.puertasCerradas()``` | Entrega una lista con los números de puertas (numeradas de 1 a 10) que no han sido abiertas aún. |
| ```P.termino()``` | Entrega ```True``` si el concurso llegó a un estado final (se abrió la puerta del super premio o una trampa), o ```False``` si no. |

Al respecto:

1. Use los métodos de la clase anterior en un programa interactivo, que permita jugar al concurso de las puertas, de acuerdo al siguiente ejemplo:

    ```python
    Cantidad de puertas? 10
    Cantidad de trampas? 3
    
    Puertas disponibles: [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
    Abrir la puerta numero? 7
    
    En la puerta habia un .... premio!
    
    Puertas disponibles: [1, 2, 3, 4, 5, 6, 8, 9, 10]
    Abrir la puerta numero? __
    
    ... # luego de abrir varias puertas más
    
    Puertas disponibles: [1, 3, 4, 8]
    Abrir la puerta número? 8
    
    En la puerta habia una... trampa!
    Lo sentimos, has perdido :c
    ```
    
    Notas:
    - Si se ingresa un 0 como número de puerta a abrir, significa que la persona no quiere arriesgarse, y se retira

2. Implemente el método constructor de la Clase.

    Suponga que la Clase se representa internamente como:
    
    - `self.Puertas`: Lista de tamaño ```N```, que almacena los números de ```1``` a ```N```. Esta lista guarda los números de puertas que no se han abierto aún. 
    - `self.Trampas`: lista de números de puerta donde se encuentra una trampa.
    - `self.Premio`: Número entero que indica la puerta donde se esconde el premio mayor.