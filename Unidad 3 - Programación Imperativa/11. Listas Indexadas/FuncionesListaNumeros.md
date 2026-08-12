---
tags: [Listas Indexadas, Ciclos Iterativos]
---

# Funciones Listas de Números

Dada una lista de números enteros positivos, cree las siguientes funciones:

1. La función ```menores(L, n)```, que dada una lista de números, cuenta cuantos elementos en `L` son menores o iguales a `n`. Ejemplo:

    ```python
    >>> L = [1, 5, 7, 3, 2, 1, 9, 8, 6]
    >>> menores(L,3)
    4
    ```

2. La función ```incrementar(L, k)```, que dada una lista de números, modifique la lista, sumándole `k` a todos los números en ella. Ejemplo:

    ```python
    >>> L = [1, 5, 7, 3, 2, 1, 9, 8, 6]
    >>> incrementar(L,5)
    >>> print(L)
    [6, 10, 12, 8, 7, 6, 14, 13, 11]
    ```

3. La función ```soloPares(L)```, que dada una lista de números, entregue una nueva lista solo con los números pares. Ejemplo:

    ```python
    >>> L = [1, 5, 7, 3, 2, 1, 9, 8, 6]
    >>> L = soloPares(L)
    >>> print(L)
    [2, 8, 6]
    ```