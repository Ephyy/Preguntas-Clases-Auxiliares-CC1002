---
tags: [Listas Indexadas, Ciclos Iterativos]
---

# Bilz y Pap 🔴🟡

Debido a la falta de sueño, usted se ha quedado dormide en clases, y sueña que ha viajado al mundo de Bilz y Pap. Allí, le reciben Billy y Maik, quienes le proponen los siguientes desafíos para ayudarle a despertar y así poner toda la atención posible en clases. Como este es un mundo de fantasía, las únicas operaciones permitidas sobre Listas son `L.pop()` y la concatenación de listas `( L = L + [x] )`.

1. Escriba la función ```pap(L)```, que toma una Lista de elementos, y entrega la lista con los elementos en orden inverso. Ejemplo:
   
    ```python
    >>> L = ['a', 'b', 1, 3, True, 4.2,'R']
    >>> pap(L)
    ['R', 4.2, True, 3, 1, 'b', 'a']
    ```

2. Escriba la función ```bilz(L)```, que toma una Lista de elementos, y los filtra, dejando solo los que sean de tipo numérico. Ejemplo:

    ```python
    >>> L = ['a', 'b', 1, 3, True, 4.2,'R']
    >>> bilz(L)
    >>> print(L)
    [1, 3, 4.2]
    ```