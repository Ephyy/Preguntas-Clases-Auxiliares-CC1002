---
tags: [Recursión]
dificultad: Difícil
---

# Numeros de D’furrí

Un número se dice que es D’furrí (pronunciado «de-fuugi») si cumple la siguiente propiedad: \
*«El resultado de la suma consecutiva de los dígitos de N, se encuentra presente como uno de los dígitos de N»*

Por ejemplo: 
- 456 es D’furrí porque 4 + 5 + 6 → 15, luego 1 + 5 → 6, y 6 está en los dígitos de 456.
- Pero 2456 no lo es, pues 2 + 4 + 5 + 6 → 17 → 1 + 7 → 8, y 8 no está en los dígitos de 2456.

Para ello se le pide crear las siguientes funciones para poder determinar si un numero es D’furrí o no.

a) Cree la función recursiva ```sumarDigitos(n)```, que suma los dígitos de un numero. Por ejemplo:
- ```sumarDigitos(456)``` entrega ```15```.

b) Cree la función recursiva ```reducir(n)```, que suma consecutivamente los dígitos de un numero, hasta obtener un número entre 0 y 9. Por ejemplo:
- ```reducir(456)``` entrega ```6```.

c) Cree la función recursiva ```buscarDigito(n, d)```, que verifica si el dígito d está en las cifras del número n. Por ejemplo:
- ```buscarDigito(456, 6)``` entrega ```True```.

d) Cree la función ```esDfurri(n)```, que verifica si un número n cumple con ser D’furrí. Por ejemplo:
- ```esDfurri(456)``` entrega ```True```
