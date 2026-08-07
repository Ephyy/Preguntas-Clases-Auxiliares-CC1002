---
tags: [Listas Recursivas, Estructuras]
---

# Catálogo de libros (Parte 2) 📚

El catálogo no está totalmente limpio, y puede pasar que un libro se haya ingresado mal y repita en una misma lista. Consideraremos que un libro está repetido si existe otro con el mismo nombre, autor y año de publicación. Por ejemplo:

```python
Libro4 = Libro("El Perfume", "Patrick Süskind", "Literatura Contemporánea", 1985, 304, 22)
Libro5 = Libro("El Perfume", "Patrick Süskind", "Literatura Contemporánea", 1985,
304, 2)

catalogo2 = lista(Libro1, lista(Libro4, lista(Libro2, lista(Libro3, lista(Libro5, listaVacia)))))
```

En este caso, el libro «El perfume» en verdad tiene 24 ejemplares, solo que está mal ingresado en el catálogo.

1. Cree la función ```librosIguales(libro1, libro2)``` que recibe 2 libros y determina si son iguales, siguiendo la explicación dada en el enunciado de este problema.
   - Por ejemplo: ```librosIguales(Libro4, Libro5)``` entrega ```True```
  
2. Cree la función ```contieneLibro(L, libro)``` que recibe una lista de libros y un libro. Esta función determina si el libro se encuentra en la lista `L`. Para determinar si un libro está o no en la lista, debe utilizar la definición de igualdad para la estructura Libro definida anteriormente.
   
    Por ejemplo:  
    ```python
    catalogo3 = lista(Libro1, lista(Libro4, lista(Libro2, lista(Libro3, listaVacia))))
    ```
    - ```contieneLibro(catalogo3, Libro5)``` entrega ```True```
  
3. Cree la función recursiva ```masRepetido(L)```, que recibe una lista de Libros, y entrega el nombre del libro que más se repita dentro de una lista. Puede asumir que solo habrá 1 Libro que se repita la mayor cantidad de veces dentro de una lista. En esta pregunta, para determinar la cantidad de repetidos **sólo nos fijaremos en apariciones en la lista**, no en el atributo cantidad.
      - Por ejemplo: ```masRepetido(L)``` entrega ```"El Perfume"``` 
     
     **Indicación:** Le puede convenir usar una variable por omisión, o crear una función auxiliar.

4. Cree la función recursiva ```sinRepetidos(L)```, que recibe una lista de Libros, y entrega la misma lista, pero sin elementos repetidos. Para ello, debe considerar que los libros repetidos se deben convertir en uno solo, actualizando la cantidad de ejemplares correspondiente.
   
    Ejemplo: En el caso de la lista `L`, tenemos 1 libro repetido, «El Perfume». Después de pasar por esta función, se debe obtener una nueva lista con 1 solo libro «El Perfume» y que tenga una cantidad de 24 ejemplares.

    Por ejemplo ```sinRepetidos(catalogo2)``` entrega:
    - ```lista(Libro1, lista(Libro("El Perfume", "Patrick Süskind", "Literatura Contemporánea", 1985, 304, 24), lista(Libro2, lista(Libro3, listaVacia))))```
    - O bien ```lista(Libro1, lista(Libro2, lista(Libro3, lista(Libro("El Perfume", "Patrick Süskind", "Literatura Contemporánea", 1985, 304, 24) listaVacia))))```