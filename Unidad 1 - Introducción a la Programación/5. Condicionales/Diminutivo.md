---
tags: [Condicionales]
---

# Diminutivo

Un numero a se dice diminutivo de otro numero b, si cada uno de los dígitos de a es menor estricto a cada uno de los dígitos de b que están en la misma posición. Por ejemplo, 112 es diminutivo de 343, pero no de 521.

Cree la función ```diminutivo(a, b)```, donde a y b son números enteros, cada uno de 3 cifras, y verifica si a es diminutivo de b, siguiendo el siguiente comportamiento:

- Si cada dígito de a, es estrictamente menor a los de b, entonces la función debe mostrar
“correcto!” en la pantalla, y retornar ```True```
- En caso contrario, debe mostrar “incorrecto! $[d_{a}]$ es mayor o igual a $[d_{b}]$”, en donde $d_{a}$ y $d_{b}$ son los dígitos de a y b respectivamente en donde no se cumple la condición. Además, la función debe retornar ```False```.
