# Canciones de Spotify 2.0 🟢🎧

En este problema, nuevamente trabajaremos con una ya conocida playlist de canciones. Tal playlist se encuentra en un archivo de texto como el siguiente:


*playlist.txt*
```
birds of a feather~~~251alternative~~~billie eilish
who~~~~~~~~~~~~~~~~~~170k-pop~~~~~~~~~jimin
taste~~~~~~~~~~~~~~~~157pop~~~~~~~~~~~sabrina carpenter
sailor song~~~~~~~~~~211pop~~~~~~~~~~~gigi perez
espresso~~~~~~~~~~~~~157funk~~~~~~~~~~sabrina carpenter
that's so true~~~~~~~166pop~~~~~~~~~~~gracie abrams
good luck, babe!~~~~~218pop~~~~~~~~~~~chappell roan
night changes~~~~~~~~226alternative~~~one direction
i wanna be yours~~~~~183indie rock~~~~arctic monkeys
we are the champions~182rock~~~~~~~~~~queen
```

- Cada linea guarda la información de una canción (nombre, duración en segundos, genero y artista)
- En cada linea:
  - Los primeros 21 caracteres contienen la información del nombre
  - Los siguientes 3 caracteres contienen la duración
  - Los siguientes 14 caracteres contienen el género
  - Los siguientes caracteres hasta el final de la linea contienen el/la artista
  - El espacio sobrante entre un dato y otro, se rellena con el carácter "colita de chancho" ```~```

Al respecto, se pide que realice lo siguiente:


+ Cree un programa que lea el archivo *playlist.txt*, y construya el archivo *playlist2.txt*, donde ahora los datos de nombre, duración, etc. se encuentren separados por el simbolo ```;``` (punto y coma). Por ejemplo, para el archivo que se muestra arriba, se espera producir el siguiente archivo:

  *playlist2.txt*
  ```
  birds of a feather;251;alternative;billie eilish
  who;170;k-pop;jimin
  taste;157;pop;sabrina carpenter
  sailor song;211pop;gigi perez
  espresso;157;funk;sabrina carpenter
  that's so true;166;pop;gracie abrams
  good luck, babe!;218;pop;chappell roan
  night changes;226;alternative;one direction
  i wanna be yours;183;indie rock;arctic monkeys
  we are the champions;182;rock;queen
  ```


+ Cree una función llamada ```cancionesOrdenadas(nombre_archivo)```, que recibe el nombre de un archivo que contiene una playlist como la generada en la parte (A) (datos de canciones separadas por ```;```), y entrega una lista de listas, en donde se entrega la información de cada canción, pero ordenada de mayor a menor duración. Por ejemplo:

  - ```cancionesOrdenadas("playlist2.txt")``` entrega:

    ```python
    [["birds of a feather", 251, "alternative", "billie eilish"],
     ["night changes", 226 , "alternative", "one direction"],
     ["good luck, babe!", 218, "pop", "chappell roan"],
     ...
     ["espresso", 157, "funk", "sabrina carpenter"]]
    ```

+ Propuestos:

  - Cree una función que recibe el nombre de un archivo que contiene una playlist, y entrega el nombre de la canción de mayor duración

  - Cree una función que recibe el nombre de un archivo que contiene una playlist, y entrega el promedio de duración entre todas las canciones de la playlist