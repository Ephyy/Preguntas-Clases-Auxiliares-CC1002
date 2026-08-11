---
tags: [Recursión, Programa Interactivo]
---

# Números Originarios

Una propiedad interesante que tienen los números enteros no negativos, es la de obtener su numero originario. Para un entero N <= 9, su numero originario se define como si mismo. Mientas que para un entero N >= 10, su numero originario se define como la multiplicación de sus dígitos. Si el resultado de esta multiplicación es mayor a 9, entonces se multiplican los dígitos de este resultado. Esto se repite hasta obtener un resultado menor o igual a 9, que corresponder´a al numero originario de N.

Ejemplo: el numero originario de 367 es 2, pues la multiplicación de los dígitos de 367 es 126, y la multiplicación de los dígitos de 126 es 12, y la multiplicación de los dígitos de 12 es 2.

En este ejercicio, crearemos una función que nos permita obtener el numero originario de un entero, y luego obtener los números originarios de cierto tipo en un rango dado.

1. Cree una función recursiva llamada ```multiplicarDigitos(n)```, que dado un numero entero no negativo `n`, entregue como resultado la multiplicación entre los dígitos de `n`.
   
2. Cree una función recursiva llamada ```originario(n)```, que dado un numero entero no negativo `n`, entregue su numero originario, de acuerdo a la descripción anterior.

3. Cree una función recursiva llamada ```listaOriginarios(a, b, n)``` que muestra en pantalla todos los números entre `a` y `b`, cuyo numero originario sea `n`. Ejemplo:

    ```python
    >>> listaOriginarios(1,33,4)
    4
    14
    22
    27
    >>> listaOriginarios(15,21,4)
    >>> listaOriginarios(9,33,9)
    9
    19
    33
    ```