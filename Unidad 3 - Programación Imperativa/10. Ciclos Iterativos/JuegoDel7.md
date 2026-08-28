---
tags: [Ciclos Iterativos, Programa Interactivo]
---
# El Juego del 7 7️⃣

Junto a un grupo de amigas y amigos de la U, quieren sacarse un 7 en el próximo control, pero como no quieren estudiar, entonces se ponen a procrastinar jugando el juego del 7.

Este juego consiste en que en un círculo, una persona parte diciendo el número 1, luego la siguiente persona dice el siguiente número (2), y así sucesivamente. Lo interesante es cuando el número a decir es un múltiplo de 7, o contiene un 7, en cuyo caso, en vez de decir el número, hay que aplaudir. Por ejemplo, para los primeros 20 números, las personas tendrían que decir:

```text
1 -> 2 -> 3 -> 4 -> 5 -> 6 -> *clap* -> 8 -> 9 -> 10 -> 11 -> 12 -> 13 -> *clap*
-> 15 -> 16 -> *clap* -> 18 -> 19 -> 20
```

Como a usted no le gusta perder, ha decidido crear un programa que le ayude a saber qué es lo que tiene que decir cuando le toque su turno. Al respecto:

+ Escriba un programa interactivo, que le pregunte a una persona por un número entero `N` mayor que 1, y el programa debe imprimir en pantalla la secuencia de números de `1` a `N`, en donde los números dentro de la secuencia que sean múltiplos o contengan un 7, se debe imprimir un `*clap*` en vez del número. Por ejemplo:

  ```python
  Numero? 9
  1
  2
  3
  4
  5
  6
  *clap*
  8
  9
  ```

  Su solución **debe usar el mecanismo de ciclos while**.

+ (Propuesto 1) Resolver el mismo problema anterior, pero ahora como una función de nombre ```secuencia7(N)```, que recibe un número entero mayor que 1, y entrega una lista que contiene la secuencia de `1` a `N`.

  Por ejemplo:

  ```python
  secuencia7(9)
  ```

  entrega:

  ```python
  [1, 2, 3, 4, 5, 6, "*clap*", 8, 9]
  ```

+ (Propuesto 2) Agregar al programa o función, el criterio de que también hay que decir `*clap*`, si la suma de los dígitos del número es múltiplo de 7.