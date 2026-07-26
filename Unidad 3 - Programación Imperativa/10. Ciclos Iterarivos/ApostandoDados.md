---
tags: [Ciclos Iterativos, Programa Interactivo]
---
# Apostando a los dados 🎲🎲

En el casino secreto de las catacumbas de 850, estudiantes se juntan a jugar juegos de azar y realizar apuestas. Dentro de todos los juegos, hay uno que usted juega frecuentemente, que consiste en que secretamente se lanzan 2 dados, y tiene que adivinar cual es la suma de los números que salió en los dados. Si adivina, entonces gana la ronda (y gana dos fichas), y si no, pierde una ficha. 

Para poder practicar, decide crear un programa interactivo que le ayude a simular este juego (y así tener más posibilidades de adivinar en el juego real).

Escriba un programa interactivo, que:
- Pregunte a una persona que ingrese un número entero entre 1 y 12  (no es necesario verificar).
- El programa secretamente, lanza 2 dados, y muestra la suma en pantalla
  - Si el valor de la suma de los dados coincide con el número ingresado, entonces ganas 2 fichas.
  - Si no coincide, entonces pierdes 1 ficha
- Se vuelve a repetir la secuencia de acciones, hasta que la persona tenga 0 fichas, o decida retirarse.

Consideraciones:

- Al empezar el programa, la persona inicia con 5 fichas
- Para retirarse, hay que escribir la palabra ``fin``

Ejemplo de dialogo:

```python 
>> ingrese número: 8
   Los dados dicen... 6
   Piedes 1 ficha
   Te quedan 4 fichas

>> ingrese número: 10
   Los dados dicen... 10
   Ganas 2 fichas
   Te quedan 6 fichas

...

>> ingrese número: fin
   te has retirado con 8 fichas
```
