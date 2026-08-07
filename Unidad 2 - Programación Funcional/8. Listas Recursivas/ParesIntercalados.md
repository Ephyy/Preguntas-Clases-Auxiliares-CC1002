---
tags: [Listas Recursivas]
---

# Pares intercalados

Una lista de números es "SuperPar" si cumple con la condición de tener pares e impares de forma intercalada. No hay restricción para el número de inicio, es decir, se puede comenzar con un par o un impar, lo importante es que se cumpla con el criterio de tener pares/impares de forma intercalada.

Cree una función ```superPar(L)``` que recibe una lista de números, y entrega ```True``` si L cumple con las condiciones para ser superPar, o ```False``` en caso contrario. Por ejemplo:

```python
L1 = lista(2, lista(3, lista(4, lista(5, listaVacia))))
L2 = (3, lista(10, lista(11, lista(32, lista(17, lista(16, lista(9, listaVacia)))))))
L3 = lista(2, lista(4, lista(5, listaVacia)))
```

Dadas las listas de arriba:

- ```superPar(L1)``` entrega ```True```
- ```superPar(L2)``` entrega ```True```
- ```superPar(L3)``` entrega ```False```
