---
tags: [Recursión]
dificultad: Media
---

# Números CVV ☮️

Diremos que un número entero positivo es "CVV" si cada uno de sus dígitos es divisor del número formado por los dígitos que se encuentran a su izquierda.

Por ejemplo, el número ```4266``` es CVV, ya que, viendo de derecha a izquierda:
- ```6``` es divisor de ```426```
- ```6``` es divisor de ```42```
- ```2``` es divisor de ```4```
- ```4``` es divisor de ```4```

En cambio, ```5913``` no es CVV:

- ```3``` es divisor de ```591```
- ```1``` es divisor de ```59```
- ```9``` NO es divisor de ```5```


Cree una función de encabezado ```esCVV(n)``` que reciba un número entero positivo y retorne ```True``` si el número es progresivo y ```False``` en caso contrario.

**Nota:** Puede asumir que todas cifras de `n` son distintas de 0.