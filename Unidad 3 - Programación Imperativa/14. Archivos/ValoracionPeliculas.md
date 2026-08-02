---
tags: [Archivos, Listas Indexadas]
---

# Valoraciones de películas 🎥⭐

Las valoraciones sobre diversas películas realizadas por un grupo de personas, se encuentran guardadas en diversos archivos (1 archivo por persona, que contiene todas las valoraciones sobre películas vistas por tal persona), en donde cada linea contiene el nombre de la película vista, y separado por un espacio, un numero entero que indica la cantidad de estrellas con las que valoró la película (entre 1 y 5). Un ejemplo de 3 archivos, es el siguiente:

`amanda.txt` :
```text
Oppenheimer 4
Barbie 5
Five-Nights-at-Freddys 5
Trolls-3 1
```
`benito.txt` :
```text
Barbie 4
Trolls-3 2
Paw-Patrol 4
```

`camila.txt` :
```text
Five-Nights-at-Freddys 5
Barbie 5
Oppenheimer 5
```

Como se puede apreciar, no todas las personas necesariamente vieron la misma cantidad de películas y/o todas las películas. Con esto, se desea procesar estos archivos, para obtener un resumen sintetizado de la valoración que un grupo de personas tiene sobre un conjunto de películas. Para esto programe lo siguiente:

+ Cree la función ```listaPelis(listaArchivos)``` , que recibe una lista de nombres de archivos que poseen valoraciones como los anteriores. La función debe procesar estos archivos, para entregar en una lista los nombres de las películas presentes en los archivos sin repetición.

  Con el ejemplo anterior la función entregaría:

  ```python
  listaPelis(["amanda.txt", "benito.txt", "camila.txt"])
  ["Oppenheimer", "Barbie", "Five-Nights-at-Freddys", "Trolls-3", "Paw-Patrol"]
  ```

+ Cree la función ```matrizDeEstrellitas(listaArchivos)``` , que recibe una lista de nombres de archivos que poseen valoraciones como los anteriores. La función debe procesar estos archivos, para agrupar todas las valoraciones en una lista de lista (o matriz). La forma de organizar esta matriz sería la siguiente:

  - En la primera fila deben ir los nombres de todas las películas presentes entre todos los archivos, sin repeticiones.
  - En las filas siguientes, se deben poner la cantidad de estrellas con las que evaluó cada persona a cada película.

    - Una fila, corresponde a una persona. Por ejemplo, en la segunda fila van todas las calificaciones que dio la persona del archivo 1 a cada película (en el orden correspondiente al de la primera fila). Si la persona no tiene calificaciones para la película en cuestión, debe anotarse 0.

    Utilice la función de la parte A para ayudarse.

    Con el ejemplo anterior la función entregaría:

    ```python
    >>> matrizDeEstrellitas(["amanda.txt", "benito.txt", "camila.txt"])

        [["Oppenheimer", "Barbie", "Five-Nights-at-Freddys", "Trolls-3", "Paw-Patrol"], # nombres de películas
        [4, 5, 5, 1, 0], # calificaciones archivo 1 ordenadas
        [0, 4, 0, 2, 4], # calificaciones archivo 2 ordenadas
        [5, 5, 5, 0, 0]] # calificaciones archivo 3 ordenadas
    ```