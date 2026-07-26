# Canciones de Spotify 🟢🎧

Una persona muy computina guarda la información de sus canciones favoritas en un archivo de texto como el siguiente:

**playlist.txt**

```text
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

- Cada línea guarda la información de una canción (nombre, duración en segundos, género y artista).
- En cada línea:
  - Los primeros 21 caracteres contienen la información del nombre.
  - Los siguientes 3 caracteres contienen la duración.
  - Los siguientes 14 caracteres contienen el género.
  - Los siguientes caracteres hasta el final de la línea contienen el/la artista.
  - El espacio sobrante entre un dato y otro se rellena con el carácter "colita de chancho" `~`.

Al respecto, se pide que realice lo siguiente:

- Cree la función `cancionesPorGenero(nombre_playlist, genero)`, que recibe un `string` con el nombre de un archivo como el anterior, y un `string` con algún género musical. La función imprime en pantalla todos los nombres de canciones cuyo género coincida con el indicado.

  Ejemplo:

  ```python
  >>> cancionesPorGenero("playlist.txt", "pop")

  taste
  sailor song
  that's so true
  good luck, babe!
  ```

- Cree la función `duracionMenorA(nombre_playlist, tiempo)`, que recibe un `string` con el nombre de un archivo estilo playlist, y un número entero positivo que representa segundos. La función entrega una lista con todos los nombres de las canciones que duren menos que `tiempo` segundos.

  Ejemplo:

  `duracionMenorA("playlist.txt", 180)` entrega: `["who", "taste", "espresso", "that's so true"]`

- Cree la función `artistasDistintos(nombre_playlist)`, que recibe un `string` con el nombre de un archivo estilo playlist. La función entrega la cantidad de artistas distintos en la playlist.

  Ejemplo:

  
  - `artistasDistintos("playlist.txt")` entrega `9`