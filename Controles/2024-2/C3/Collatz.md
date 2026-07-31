---
tags: [Control, Listas Indexadas, Programa Interactivo]
---

# Conjetura de Collatz [C3 2024-2]

La Conjetura de Collatz es uno de los más famosos problemas no resueltos de la matemática. Dado un entero N ≥ 1, el problema consiste en generar la siguiente secuencia de transformaciones:
  - Si N es par, divida el número por 2.
  - Si N es impar, multiplique el número por 3 y luego sume 1.
  - La secuencia termina cuando N = 1.
  
Por ejemplo, para N = 19, se tiene la secuencia: 19, 58, 29, 88, 44, 22, 11, 34, 17, 52, 26, 13, 40, 20, 10, 5, 16, 8, 4, 2, 1. Para N = 20, se tiene la secuencia: 20, 10, 5, 16, 8, 4, 2, 1.

Note que la secuencia para N = 19 tiene 21 pasos, mientras que para N = 20 la secuencia tiene 8 pasos. La conjetura plantea que, para cualquier valor posible de N, siempre se llegará a 1. Si bien aún no se ha demostrado formalmente esta proposición, se ha verificado empíricamente que es válida (al menos) hasta $N = 2.95 \times 10^{20}$.

+ **(3.0 ptos.)** Escriba la función ```collatz(N)```, tal que dado un N entero positivo cualquiera, devuelva una lista con todos los pasos de la secuencia de Collatz desde N hasta que termina en 1. Por ejemplo, ```collatz(20)``` devuelve ```[20,10,5,16,8,4,2,1]``` y ```collatz(1)``` devuelve ```[1]```.
  
+ **(3.0 ptos.)** Escriba un programa que le solicite a una persona un número N. Luego el programa, para todos los números entre 1 y N, debe calcular la cantidad de pasos de su secuencia de Collatz. Por último, el programa debe mostrar en líneas separadas, el número N y su cantidad de pasos respectiva, pero mostrándolos **en orden ascendente de número de pasos**.
  
  Ejemplo (note que el resultado está ordenado por la cantidad de pasos):

  ```python
  >> Hasta? 20
  N Pasos
  1 1
  2 2
  4 3
  8 4
  16 5
  5 6
  10 7
  3 8
  20 8
  6 9
  12 10
  13 10
  17 13
  11 15
  7 17
  14 18
  15 18
  9 20
  18 21
  19 2
  ```