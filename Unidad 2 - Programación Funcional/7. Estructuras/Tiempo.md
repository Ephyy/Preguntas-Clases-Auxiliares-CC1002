---
tags: [Estructuras]
---

# Tiempo

Se desea contar con un Modulo llamado Tiempo, que permita manejar tiempos expresados en Horas y Minutos, y realizar algunas operaciones entre estos tiempos. Para esto, implemente las siguientes estructuras y funcionalidades de este modulo:

a) La estructura `Tiempo`, la cual posee dos atributos: Horas y Minutos.

b) Una función llamada ```esTiempo(X)```, que recibe «cualquier cosa» y entregue ```True``` si corresponde a una representación de tiempo válida, y ```False``` si no.

c) Una función llamada ```tiempoAStr(T)```, que recibe un `Tiempo`, y entrega dicho tiempo en formato `'HH:MM'` (como un string). Por ejemplo:
- ```aMinutos(Tiempo(3,5))``` entrega ```185```

d) Una función llamada ```crearTiempo(minutos)```, que recibe una cantidad de minutos no negativa, y retorna un Tiempo que representa esa cantidad de minutos. Por ejemplo:
- ```crearTiempo(185)``` entrega ```Tiempo(3,5)```

f) Una función llamada ```sumar(T1,T2)```, que recibe dos Tiempos, y entrega como resultado un dato de tipo Tiempo que representa la suma de los dos tiempos. Por ejemplo:
- ```sumar(Tiempo(3,5), Tiempo(4,58))``` entrega ```Tiempo(8,3)```

g) Una función llamada ```restar(T1,T2)``` , que recibe dos Tiempos y entrega como resultado un dato de tipo Tiempo que representa la resta de los dos tiempos. (En caso de que el resultado calculado sea negativo, entonces el tiempo resultante es 0). Por ejemplo:
- ```restar(Tiempo(4,58), Tiempo(3,5))``` entrega ```Tiempo(1,53)```

h) Una función llamada ```mayor(T1,T2)```, que compara dos `Tiempo` y entrega el `Tiempo` que sea mayor. Por ejemplo:
- ```mayor(Tiempo(4,58), Tiempo(3,5))``` entrega ```Tiempo(4,58)```
