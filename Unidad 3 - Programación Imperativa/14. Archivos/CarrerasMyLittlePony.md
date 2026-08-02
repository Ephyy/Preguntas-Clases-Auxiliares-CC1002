---
tags: [Archivos, Listas Indexadas, Ciclos Iterativos]
---

#  Carreras My Little Pony

Los personajes de My Little Pony compitieron en una carrera contrareloj y necesitan su ayuda para determinar los lugares que obtuvieron. Para ello le entregan un archivo con el tiempo que demoró cada una de ellas. Para todos los casos el tiempo tiene el formato mm:ss (minutos:segundos). El archivo recibido sigue la siguiente estructura:

```text
AppleJack 17:02
Fluttershy 08:45
Rainbow-Dash 12:35
Pinkie-Pie 14:28
Rarity 21:34
Sweetie-Belle 06:12
```

Su trabajo es entregar un nuevo archivo con los nombres de los personajes ordenados por lugar obtenido en la carrera. Dado que es una carrera contrarreloj, mientras menor sea el tiempo del personaje, mejor es su lugar obtenido. Además, se debe incluir el lugar obtenido.

Para ello cree la funcion ```lugares_carreras(nombre_archivo)``` que recibe el nombre del archivo con los tiempos de la carrera y crea un nuevo archivo con las posiciones o lugares obtenidos en la carrera por cada personaje. Por ejemplo, para el archivo del ejemplo anterior se obtiene el siguiente archivo:

```
1. Sweetie-Belle
2. Fluttershy
3. Rainbow-Dash
4. Pinkie-Pie
5. AppleJack
6. Rarity
```