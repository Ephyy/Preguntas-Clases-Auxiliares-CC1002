---
tags: [Recursión]
titulo: Números Primos (Variante 2)
---

# Números Primos (Variante 2)

El objetivo de la siguiente pregunta es realizar un programa que entregue un String que contenga los números primos en un determinado rango. Para ello se le propone a usted seguir los siguientes pasos:

a) Cree una función recursiva de encabezado ```factorEnRango``` que recibe como parámetros dos enteros, $k$ y $n$. Esta función debe entregar verdadero si es que algún número en el rango $[k, n − 1]$ divide a $n$, y falso en el caso contrario.

Por ejemplo, ```factorEnRango(2, 4)``` entrega ```True```, debido a que 2 divide a 4. En cambio ```factorEnRango(4, 17)``` entrega ```False```, ya que no existe un número entre [4,16] que divida exactamente a 17.

b) Usando la función `factorEnRango`, cree una función de encabezado `esPrimo` que recibe como parámetros un entero $n$, y debe retornar ```True``` si es que el número n es primo, o ```False``` en el caso contrario.

Como ejemplo, ```esPrimo(2)``` debe entregar True, y ```esPrimo(4)```
debe entregar False

c) Finalmente usando la función `esPrimo`, cree una función recursiva de encabezado `primosEnRango` que recibe como parámetros dos enteros, $x$ e $y$, la cual entrega un string con los números primos en el intervalo cerrado [x, y] separados por espacios.

Un ejemplo de ello es que ```primosEnRango(2, 10)``` debe entregar como resultado `"2 3 5 7"` y ```primosEnRango(20, 22)``` debe entregar `""` ya que no hay primos en ese intervalo.
