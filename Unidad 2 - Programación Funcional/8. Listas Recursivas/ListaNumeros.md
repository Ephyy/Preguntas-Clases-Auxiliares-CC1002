---
tags: [Recursión]
---

# Listas de Números
En esta sección trabajaremos creando funciones para listas de números. Tendremos de ejemplo la siguiente lista:

```python
L = lista(5, lista(-3, lista(2, lista(-8, listaVacia))))
```

1. Cree la función recursiva ```sumar2(L)```, que recibe una lista de números de largo par, y entrega una lista, en la que los números de la lista original, fueron sumados de 2 en 2. Ejemplo: 
   - ```sumar2(L)``` entrega ```lista(2, lista(-6, listaVacia))```
  que es el resultado de sumar 5 + -3 y 2 + -8

2. Cree la función recursiva ```estDecreciente(L)```, que recibe una lista de números, y entrega ```True``` si es que la secuencia de números de la lista es estrictamente decreciente, y ```False``` si no.
   - Por ejemplo, ```estDecreciente(L)``` entrega ```False```.
   - Pero, si tenemos ```L2 = lista(553, lista(238, lista(109, lista(1, listaVacia))))```. \
   Entonces ```estDecreciente(L2)``` entrega ```True```.

3. Cree la función recursiva ```contarCaidas(L)```, que recibe una lista de números (de al menos 2 elementos), y entrega la cantidad de veces que, de dos números consecutivos en la lista, el siguiente número en la secuencia es menor al anterior.
Por ejemplo, si tenemos la lista: ```L3 = lista(2, lista(3, lista(5, lista( 3, lista(4, lista(1, lista(3, listaVacia)))))))``` \
Entonces ```contarCaidas(L3)``` entrega ```2```, porque hubo una caída entre 5 y 3, y luego entre 4 y 1