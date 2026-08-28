---
tags: [Listas Recursivas, Estructuras]
---

# Catálogo de libros (Parte 1) 📚

A usted le piden ayuda para manejar un catálogo de libros de una biblioteca. El catálogo, corresponde a una lista recursiva de estructuras «libro», tal como se muestra a continuación.

```python
#Libro: nombre(str) autor(str) categoria(str) hojas(int) cantidad(int)
estructura.crear("Libro", "nombre autor categoria hojas cantidad")

Libro1 = Libro("El león, la bruja y el armario", "C. S. Lewis", "fantasía", 240, 87)
Libro2 = Libro("Juego de Tronos", "George R.R. Martin", "fantasía", 800, 24)
Libro3 = Libro("Cuatro Estaciones en Japón", "Nick Bradley", "ficcion literaria", 384, 20)

catalogo = lista(Libro1, lista(Libro2, lista(Libro3, listaVacia)))
```

1. Escriba una función llamada ```contarCategoria(L, c)```, que recibe una lista de libros y entrega un número indicando la cantidad de libros correspondientes a la categoría `c`. No basta solo con contar la cantidad de apariciones de un libro con la categoría, sino que se debe considerar el atributo «cantidad» de la estructura libro.
   
    Por ejemplo:
    - ```contarCategoria(catalogo, "ficcion literaria")``` entrega ```20```
    - ```contarCategoria(catalogo, "fantasía")``` entrega ```111```

2. En la biblioteca se dieron cuenta de que había un problema de conteo en la cantidad de ejemplares de los libros. Escriba una función llamada ```sumarEjemplares(L, n)```, que recibe una lista de libros y un número entero `n`. Entrega una nueva lista donde a cada uno de los libros se le suma la cantidad `n` a su cantidad.
