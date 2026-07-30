---
tags: [Listas Recursivas]
---

# Notas de Cursos 🧮

En cierta universidad, la información de las notas de un(a) estudiante se guarda en una lista de estructuras:

```python
# Curso: nombre(str) notas(lista(float))
estructura.crear("Curso", "nombre Lnotas")

# Cursos de ejemplo
Calc = Curso("cálculo", lista(1.5, lista(3.8, lista(6.3, listaVacia))))
Alg = Curso("álgebra", lista(6.4, lista(1.7, lista(4.6, lista(5.5, listaVacia)))))
Fis = Curso("física", lista(5.2, lista(4.4, listaVacia)))
Comp = Curso("computación", lista(6.5, listaVacia))

# Lista de cursos de ejemplo
Lcursos = lista(Calc, lista(Alg, lista(Fis, lista(Comp, listaVacia))))
```

Es decir:

- Un estudiante tiene asociada una lista de cursos.
- Un curso se compone de un nombre y una lista de notas.
- La lista de notas es un listado de las notas (floats entre `1.0` y `7.0`) obtenidas en tal curso.

Al respecto, se pide lo siguiente:

- Cree la función ```promedioNotas(LN)```, que recibe una lista de números, y calcula el promedio de los números almacenados en la lista.

  Ejemplo:

  - ```promedioNotas(lista(5.2, lista(4.4, listaVacia)))``` entrega ```4.8```.
  - ```promedioNotas(lista(6.5, listaVacia))``` entrega ```6.5```.

- Cree la función ```promedioPersona(LC)```, que recibe una lista de cursos, y calcula el promedio general, es decir el promedio de los promedios de cada curso.

  Ejemplo:

  - ```promedioPersona(Lcursos)``` entrega aproximadamente ```5.0```.

- Para evitar reprobar un ramo que no tiene salvación, cree la función ```eliminaEspecial(LC)```, que recibe una lista de cursos, y entrega una lista de cursos, en la cual se eliminó el curso con el promedio más bajo.

  Ejemplo:

  - ```eliminaEspecial(Lcursos)``` entrega:

    ```python
    lista(Alg, lista(Fis, lista(Comp, listaVacia)))
    ```