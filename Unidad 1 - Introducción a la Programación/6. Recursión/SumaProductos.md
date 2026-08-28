---
tags: [Recursión]
---

# Suma Productos

En TikTok ha salido un nuevo desafío, que consiste en multiplicar rápidamente los dígitos de dos números **enteros** del mismo tamaño. En concreto, lo que hay que hacer es que al aparecer los dos números, hay que calcular la suma de los productos de sus dígitos.

Es decir, que si tenemos los números 1234 y 5678, deberá obtener:

$$sumaProductos(1234, 5678) = 1 ⋅ 5 + 2 ⋅ 6 + 3 ⋅ 7 + 4 ⋅ 8  $$

$$  = 70 $$

Por lo que, para ayudarse en este desafío, se propone a crear la función recursiva ```sumaProductos(A, B)```, que recibe dos números enteros positivos A y B, y entrega la suma de los productos de sus dígitos, siguiendo la idea anterior. Por ejemplo:

- ```sumaProductos(1234,5678)``` entrega ```70```
- ```sumaProductos(333, 111)``` entrega ```9```