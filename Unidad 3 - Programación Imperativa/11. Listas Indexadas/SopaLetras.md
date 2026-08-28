---
tags: [Listas Indexadas, Ciclos Iterativos]
---

# Sopa de Letras 🍲

El día de ayer, usted estaba muy aburrido(a) estudiando para el control fome del viernes. Para hacer más amena su velada, decidió hacer una sopa de letras. Al ver los resultados de sus artes culinarias, tuvo una idea muy entretenida (?), de modelar una sopa de letras como una lista de `string`, como la siguiente:

```python
L = ['a', 'b', 'r', 'a', 'c', 'a', 'd', 'a', 'b', 'r', 'a']
```

Y con esto, se le ocurrió crear las siguientes funciones, que operan con listas de letras como la anterior:

1. Escriba una función ```contarLetras(L, letra)``` que cuenta la cantidad de veces que se repite `letra` dentro de la lista `L`.

    En el ejemplo, ```contarLetras(L, 'a')``` entregaría ```5```.

2. Escriba la función ```unicidad(L)```, que dada una lista de letras, modifica la lista, dejando solo 1 aparición de cada letra. Por ejemplo:

    ```python
    >>> L = ['a', 'b', 'r', 'a', 'c', 'a', 'd', 'a', 'b', 'r', 'a']
    >>> unicidad(L)
    >>> print(L)
    ['a','b','r','c','d']
    ```

3. Escriba la función ```invertir(L)``` que toma una lista de letras como la del ejemplo, y entrega una nueva lista, con los elementos invertidos de esa lista.

    Ejemplo:

    ```python
    L = ['a', 'b', 'r', 'a', 'c', 'a', 'd', 'a', 'b', 'r', 'a']
    invertir(L)
    # ['a', 'r', 'b', 'a', 'd', 'a', 'c', 'a', 'r', 'b', 'a']
    ```

4.  Escriba la función ```contiene(L1, L2)```, que entrega ```True``` si todo el contenido de `L2` se encuentra presente en `L1`, y ```False``` en caso contrario.
  
    Por ejemplo:

    ```python
    >>> L1 = ['a', 'b', 'r', 'a', 'c', 'a', 'd', 'a', 'b', 'r', 'a']
    >>> L2 = ['b','a','c','a']
    >>> contiene(L1, L2)
    True
    >>> L3 = ['a','b','c','d','e','f']
    >>> contiene(L3,L2)
    False
    ```

5. Escriba una función ```mezclarSopas(L1, L2)```, que toma dos listas de letras (que pueden ser de distintos tamaños), y retorna una lista con los `string` concatenados uno por uno.

    En caso que una lista sea más corta que la otra, debe concatenarse con un guión bajo.

    Ejemplo:

    ```python
    L1 = ['a', 'b', 'r', 'a']
    L2 = ['c', 'a']

    mezclarSopas(L1, L2)
    # ['ac', 'ba', 'r_', 'a_']
    ```

    Notar que `r` y `a` tienen un `_` al lado.

6. Escriba una función ```sinRepeticiones(L)``` que recibe una lista de letras, y retorna una nueva lista sin letras repetidas.

    ```python
    L = ['a', 'b', 'r', 'a', 'c', 'a', 'd', 'a', 'b', 'r', 'a']

    sinRepeticiones(L)
    # ['a', 'b', 'r', 'c', 'd']
    ```