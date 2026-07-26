---
tags: [Archivos]
---

# La Pauta 📝✔️❌

En una prueba de alternativas (con 4 alternativas por pregunta), se cuenta con el archivo ```pauta.txt```, que como su nombre lo dice, contiene la respuesta correcta a cada pregunta, linea por linea:

*pauta.txt*
```text
C
A
D
C
C
B
```

También, se tienen archivos, que contienen las respuestas a tal prueba, entregadas por algún estudiante, cuyos nombres son de la forma ```resp_nombre.txt```. Por ejemplo:

*resp_amelia.txt*
```text
C
B
D
C
C
A
```

Al respecto, se quiere crear un programa que ayude a contrastar las respuestas con la pauta, y asignar puntaje, para lo cual le piden programar la función de nombre ```revisar(nombre_pauta, nombre_resp)```, que recibe el nombre de dos archivos (la pauta y la respuesta de un estudiante respectivamente). 

La función construye un nuevo archivo, llamado ```puntaje_[nombre].txt```, donde ```[nombre]``` es el nombre de la persona que está en el nombre del archivo respuesta. En este archivo, por cada linea, se coloca la respuesta de la persona, y separado por un espacio, se coloca ```1pt``` si es que la respuesta en esa posición coincide con la pauta en la misma posición, y ```0pt``` si es que no coincide. Por ejemplo:

- ```revisar("pauta.txt", "resp_amelia.txt")``` construye el archivo ```puntaje_amelia.txt``` con el siguiente contenido:

  *puntaje_amelia.txt*
  ```text
  C 1pt
  B 0pt
  D 1pt
  C 1pt
  C 1pt
  A 0pt
  ```

- Puede asumir que todas las personas respondieron todas las preguntas