---
tags: [Control, Listas Recursivas]
---

# Listas Complementarias (P2-A C1 2022-01)

Para esta pregunta consideraremos que estamos trabajando en el conjunto con los números enteros del 1 al 100 (inclusive). 

Escriba la función ```complemento(L)```, que recibe una lista de números enteros entre 1 y 100, y entrega una lista con el complemento de ese grupo de números. Por ejemplo:

  - Si ```LC = lista(2, lista(3, lista(98, listaVacia)))```, entonces:

  ```python
  complemento(LC) entrega:

  lista(1, lista(4, lista(5, lista(6, ...,
    lista(97, lista(99, lista(100, listaVacia))) ... ))))
  ```

  Es decir, la función entrega una lista con todos los números entre 1 y 100 que no se encuentran en la lista recibida como parámetro.
