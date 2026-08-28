---
tags: [Listas Indexadas, Ciclos Iterativos]
---

# Lotería

Los números ganadores de un sorteo de un juego de azar, como el Loto, se pueden representar a través de una lista
de números enteros sin repetidos, por ejemplo: ```Lsorteo = [27, 40, 33, 18, 41, 38]```.

De igual manera, un boleto/ticket de números para un sorteo, también se pueden representar por una lista. Tome como ejemplo las listas:

Con esto, cree la función ```aciertos(LS, LB)```, que recibe una lista que contiene los números de un sorteo, y una lista con los números de un boleto asociado a tal sorteo. La función entrega la cantidad de aciertos que obtuvo el boleto con respecto al sorteo. Ejemplos:

- ```aciertos(Lsorteo, Lboleto1)``` entrega ```2```
- ```aciertos(Lsorteo, Lboleto2)``` entrega ```6```

**Indicaciones:**
- Su función no debe modificar/mutar las listas originales recibidas por parámetro.
- Verifique con precondiciones que ambas listas tengan el mismo largo.
