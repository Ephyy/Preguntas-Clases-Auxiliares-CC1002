---
tags: [Listas Indexadas]
---

# Listas Climaticas⚡👴🏼⚡🔱

Los Dioses Intrinsicamente Malvados (DIM) han causado estragos con el clima en el último tiempo. Respecto a estos eventos, se cuenta con dos listas, que registran la temperatura y el estado del clima registrado en ese día:

```python
Ltemps = [11, -11, 17, -6, -2, 33, -10, 26, 3, -5]
Lclima = ["nublado", "nieve", "soleado", "tormenta", "lluvioso", "soleado", "nieve", "soleado", "nublado", "lluvioso"]
```

En donde la información entre ambas listas está asociada por su posición. Es decir, la información del dia 1, se puede acceder a través de `Ltemps[0]` y `Lclima[0]` (Dia nublado, 11°)

Con esta información, se pide que realice lo siguiente:

+ Cree la función ````promedioClimas(Ltemps,Lclima, clima)````, que recibe dos listas como las anteriores (ambas del mismo largo) y un str `clima`. Esta función entrega el promedio de temperaturas de todos los días que cumplan con ser del `clima` indicado.

  Ejemplo:

  - ```promedioClimas(Ltemps, Lclima, "nieve")``` entrega ```-10.5```

+ Cree la función `promedioDias(Ltemps, Lclima, inicio, fin)`, que recibe dos listas como las anteriores, y dos enteros (`inicio` < `fin`). La función entrega el promedio de temperatura, entre los días `inicio` y `fin` (inclusive). En el caso de que `inicio` o `fin` se encuentren fuera del rango de las listas, entonces debe calcular hasta donde se pueda. Aproxime el promedio para que tenga solo 1 decimal.

  Ejemplo:
  - ```promedioDias(Ltemps, Lclima, 1, 5)``` entrega ```5.2```
