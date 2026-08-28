---
tags: [Recursión]
dificultad: Media
---

# Quitar Digito 🔪

Escriba la función ```quitarDigito(n, d)```, que recibe un entero positivo `n` (distinto de cero) y un digito `d` (entre 0 y 9), y entregue el numero `n` sin las cifras iguales a `d`. En caso de quitar todos los dígitos se debe entregar 0.

Ejemplo: 
- ```quitarDigito(200301, 2)``` entrega ```301```
- ```quitarDigito(111111, 1)``` entrega ```0```
  
Nota:
- En caso de que el numero `n` quede con 0 al inicio, se deben ignorar (Ejemplo 1)
- **Restricción:** No se puede transformar el numero `n` a string.