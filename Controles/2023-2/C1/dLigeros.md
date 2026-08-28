---
tags: [Control, Recursión, Funciones]
dificultad: Media
---

# Números d-ligeros ⚖️

Un número entero positivo es "d-ligero" si ninguno de los dígitos del número es mayor que d. Por ejemplo, 3124 es "4-ligero", pues ninguno de los dígitos es mayor que 4, pero 3124 no es "2-ligero", pues tiene al menos 1 dígito que es mayor que 2. Al respecto:

+ Escriba la función recursiva ```mayorQue(n, d)```, que recibe un número `n` y un dígito `d` (entre 1 y 9). La función entrega cuántos dígitos de n son mayores que d. 
 
  Por ejemplo:

  - ```mayorQue(3124, 2)``` entrega ```2```
  - ```mayorQue(3124, 4)``` entrega ```0```
  
+ Usando la función anterior, escriba la función ```esLigero(n, d)```, que indica si un número cumple con ser dligero o no. 
  
  Ejemplo:
  - ```esLigero(3124, 4)``` entrega ```True```
  - ```esLigero(3124,2)``` entrega ```False```

**Indicación:** Puede crear funciones auxiliares o usar variables por omisión si lo considera necesario