---
tags: [Recursión]
dificultad: Media
---

# El número C.D. Anakena 🏆🏆🏆🏆👕🦊

El número de Anakena, se define como: 


  _"La suma de la multiplicación de pares de dígitos de un numero"_


Por ejemplo:

Si tenemos el número 482130, los pares de dígitos son 30, 21 y 48. Para cada par, sus dígitos se multiplican, y luego todos los resultados se suman, entregando el número de Anakena.

$$ 
Anakena(482130)
    = 4*8 + 2*1 + 3*0 
    = 32 + 2 + 0 
    = 34
$$

En el caso de un número de largo impar, entonces el dígito de más a la izquierda, se multiplica por un cero:

$$ 
Anakena(85437)
    = 0*8 + 5*4 + 3*7 \
    = 0 + 20 + 21\
    = 41
$$

$$
    Anakena(123456789)
    = 0*1 + 2*3 + 4*5 + 6*7 + 8*9
$$
$$
    = 0 + 6 + 20 + 42 + 72\
    = 140
$$

Por simplicidad, asumiremos que:

- Un número nunca empezará por un cero
- El número no será negativo

Para calcular el número de Anakena, programe la función recursiva ```anakena(N)```, que recibe un número entero positivo, y entrega el número de Anakena de tal número `N`, de acuerdo a la descripción anterior.

Ejemplos:
- ```anakena(482130)``` entrega ```34```
- ```anakena(85437)``` entrega ```41```
- ```anakena(1)``` entrega ```0```
- ```anakena(12345678)``` entrega ```100```

Indicaciones:
- Plantee adecuadamente el Caso base y Caso recursivo
- Primero programe su solución, asumiendo que el número ingresado es de largo par. Luego revise si es necesario hacer adaptaciones para el caso de largo impar.
- Recuerde disminuir el tamaño del problema en cada paso recursivo