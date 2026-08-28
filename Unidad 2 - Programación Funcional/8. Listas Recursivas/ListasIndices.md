---
tags: [Listas Recursivas]
---

#  Lista de indices ℹ️

Las siguientes preguntas, trabajan bajo el concepto de índices. Los indices sirven para numerar los elementos de un conjunto.

En nuestro caso, los elementos se enumeran de 1 en adelante, desde el primer elemento de una lista, hacia la derecha.

Para los ejemplos, asumiremos que está definida la siguiente lista:

```L = lista(4, lista(3, lista("caramelo", lista(7, listaVacia))))```


En particular, si enumeramos los elementos de la lista anterior:
- ```4``` es el elemento en la posición 1
- ```3``` es el elemento en la posición 2
- ```"caramelo"``` es el elemento en la posición 3
- ```7``` es el elemento en la posición 4

1. Cree la función recursiva ```indice(L,e)```, que recibe una lista y un elemento, y entrega un número entero, que indica la posición de la primera aparición del elemento en la lista. En caso de que el elemento no este presente en la lista, la función retorna un cero. Ejemplo: 
   - ```indice(Le, 'caramelo')``` entrega: ```3```
  
2. Cree la función recursiva ```obtener(L,i)```, que recibe una lista y un entero que indica un índice de la lista. La función debe entregar el elemento almacenado en la posición i-esima de la lista. Ejemplo: 
   - ```obtener(Le,2)``` entrega: ```3```
  
3. Cree la función recursiva ```agregarEn(L,e,i)```, que recibe una lista, un elemento y un entero que indica una posición dentro de la lista. La función debe entregar una lista, donde se agrega el elemento en la posición i-esima, y el elemento que se encontraba en esa posición (y los que vienen) se desplazan un espacio hacia la derecha. En caso de que el índice no esté dentro del rango de la lista, entonces la función agrega tal elemento
    al final de la lista. Ejemplo:
    - ```agregarEn(Le,'manzana',2)``` entrega ```lista(4,lista('manzana', lista(3, lista('caramelo', lista(7, listaVacia)))))```
