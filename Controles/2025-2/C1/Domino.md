---
tags: [Control, Condicionales, Módulos, Funciones]
dificultad: Media
---


# Dominó

El **dominó** es un clásico juego de mesa que utiliza un conjunto de 28 fichas, cada una dividida en dos espacios con puntos (o "ojos") que van del 0 al 6, cubriendo todas las combinaciones posibles. 

**Importante:** Para este problema el dominó tendrá valores entre 1 y 7. 

Los jugadores colocan por turnos las fichas de forma que los puntos de los extremos coincidan con los de las fichas ya puestas en la mesa, siendo el objetivo ser el primero en quedarse sin fichas o tener la menor cantidad de puntos si el juego se "cierra".

- Una **ficha** se representa como un par de dígitos,
cada uno entre 1 y 7. \
  Por ejemplo el número **32** representa una ficha, que podría ser colocada en el juego como **3-2** o **2-3**.

  ![Ficha Dominó](./img/domino1.png)

- Un **juego** se representa como un entero positivo que registra los valores de las fichas en el tablero. Por ejemplo, el número **3445511337** representa las siguientes fichas en juego:

  ![Juego Dominó](./img/domino2.png) 

Se dispone del módulo `domino`, con las siguientes funciones:

| Función | Propósito | Ejemplo |
|---|---|---|
| ```primer_valor(juego)``` | Retorna el valor libre de la primera ficha. | ```primer_valor(3445511337) == 7``` |
| ```ultimo_valor(juego)``` | Retorna el valor libre de la última ficha. | ```ultimo_valor(3445511337) == 3``` |
| ```poner_inicio(ficha, juego)``` | Recibe una ficha y la pone al inicio del juego. | ```poner_inicio(71, 3445511337)``` == 3445511337**71**<br>```poner_inicio(17, 3445511337)``` == 3445511337**71**<br>```poner_inicio(26, 3445511337)``` == 3445511337 |
| ```poner_final(ficha, juego)``` | Recibe una ficha y la pone al final del juego. | ```poner_final(23, 3445511337)``` == **23**3445511337<br>```poner_final(32, 3445511337)``` == **23**3445511337<br>```poner_final(26, 3445511337)``` == 3445511337 |

Para las dos últimas funciones, notar que, si no es posible colocar la ficha, se retorna el mismo juego que se recibió sin bmodificaciones. Con esto, haga lo siguiente:

+ **(3.0p)** Escriba la función ```poner_inicio(ficha, juego)``` del módulo domino.

+ **(3.0p)** Usando el módulo domino, escriba la función ```poner_ficha(ficha, juego)```, donde ficha es el valor de dos dígitos que representa la ficha a poner, e intenta colocarla en alguno de los extremos del juego. Si la ficha se puede poner en ambos lados, usted elija uno. Si no se puede poner la ficha, se retorna el mismo juego que se recibió.

  Ejemplos:
  - ```poner_ficha(32, 3445511337)``` entrega: **23**3445511337 (se colocó la ficha 32 como 2-3 al extremo izquierdo del juego)
  - ```poner_ficha(56, 3445511337)``` entrega: 3445511337 (no se pudo colocar la ficha 5-6 en alguno de sus extremos) 
    
    Indicación: Puede usar todas las funciones del módulo domino sin necesidad de definirlas.

**NOTA: no se puede transformar el número entero a String o viceversa para resolver esta pregunta.**