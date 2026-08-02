---
tags: [Listas Recursivas]
---

# Listas y Listas
Vamos a subir un nivel de dificultad, y vamos a trabajar con dos listas a la vez!

```python
Lej1 = lista(3, lista('manzana', lista(2, listaVacia)))
Lej2 = lista(7, lista(4, lista('piña', listaVacia)))
Lej3 = lista('piña', lista(7, listaVacia))
Lej4 = lista(2, lista(3, lista('manzana', listaVacia)))
```

+ Cree la función ```subconjunto(L1, L2)```, que recibe dos listas de elementos, y entrega True si todos los elementos de L2 están presentes en L1 (no necesariamente en el mismo orden). Ejemplo:
  - ```subconjunto(Lej2, Lej3)``` entrega ```True```
  - ```subconjunto(Lej1, Lej2)``` entrega ```False```
  
+ Cree la función ```mezclar(L1, L2)```, que recibe dos listas de elementos, y entrega y entrega una lista con todos los elementos de L1 y L2, sin repeticiones. Ejemplo:

  ```python
  LA = lista('A', lista(1, lista(7, listaVacia)))
  LB = lista(1, lista('B', lista('A',listaVacia)))
  mezclar(LA,LB) entrega lista('A', lista(1, lista(7, lista('B', listaVacia))))
  # (o alguna permutación distinta de los elementos anteriores)
  ```

+ Cree la función ```iguales(L1, L2)```, que recibe dos listas de elementos, y entrega ```True``` si ambas listas tienen los mismos elementos (no necesariamente en el mismo orden). Ejemplo:
  - ```iguales(Lej1, Lej2)``` entrega ```False```
  - ```iguales(Lej1, Lej4)``` entrega ```True```
  
  Puede asumir que no hay elementos repetidos

+ Cree la función ```concatenar(L1,L2)```, que recibe dos Listas, y entrega una nueva lista, donde los contenidos de la segunda lista fueron anexados al final de la primera lista. Ejemplo:
  -  ```concatenar(Lej1,Lej2)``` entrega ```lista(5,lista(8,lista('manzana', lista(6,lista('pera',lista(1,listaVacia))))))```

+ Cree la función ```intercalar(L1, L2)```, que recibe dos listas de elementos del mismo largo, y entrega una lista en que primero está el primer elemento de L1, luego el primero elemento de L2, luego el segundo elemento de L1, luego el segundo elemento de L2, y así sucesivamente. Ejemplo:
  - ```intercalar(Lej1, Lej2)``` entrega ```lista(3, lista(7, lista('manzana', lista(4, lista(2, lista('piña', listaVacia))))))```
 
+ Ahora modifique la función anterior para que pueda manejar el caso cuando las listas entregadas tienen distinto largo. Ejemplo:
  - ```intercalar2(Lej1, Lej3)``` entrega ```lista(3, lista('piña', lista('manzana', lista(7, lista(2, listaVacia)))))```
