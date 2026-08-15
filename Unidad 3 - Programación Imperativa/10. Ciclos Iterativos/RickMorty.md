---
tags: [Ciclos Iterativos, Programa Interactivo]
---

# Morty y las tablas de multiplicar

Rick & Morty se preparan para dar inicio a su nueva temporada, pero se han topado con un problema inesperado. Jerry, el padre de Morty, esta muy preocupado por el rendimiento de su hijo en matemáticas, por lo que le dice que si no mejora sus notas, no podrá participar de la nueva temporada. 

Cree un programa interactivo que ayude a Morty a estudiar las tablas de multiplicar, siguiendo un dialogo similar al que aparece mas abajo:

- Se generan dos números enteros al azar entre 1 y 9, y muestra en pantalla la
operación de multiplicación entre ambos, y pide ingresar una respuesta.
- Si acierta, el programa muestra el mensaje `"Correcto!"`. Si falla, el programa muestra el mensaje `"Incorrecto!"`. En ambos casos, el programa repite el flujo de acciones anterior, generando una nueva multiplicación y preguntando por su resultado.
- Si en vez de un resultado, se ingresa la palabra `"fin"`, el programa termina, mostrando un recuento de respuestas correctas vs el total.


```python
   Ayudemos a Morty a estudiar matemáticas!
-> 5 * 8 ? 40
   Correcto!
-> 7 * 4 ? 24
   Incorrecto :(
   ...
-> 9 * 9 ? fin
   Tuviste 4 aciertos de 5 preguntas
```