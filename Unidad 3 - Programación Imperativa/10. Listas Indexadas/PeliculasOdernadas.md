# ¿Lista ordenada? 🔤✅

A Cindy le gustan mucho las películas, por lo que tiene un estante lleno de películas, las cuales se encuentran ordenadas por nombre, de menor a mayor. El problema es que su gato constantemente se sube al estante y le bota/desordena todas las películas, por lo que cada cierto tiempo tiene que estar mirando que su gato no ha causado caos y desordenado su colección.

Para ayudarle a revisar si su gato ha hecho maldades, cree la función `pelisOrdenadas(L)`, que recibe una lista de Python con nombres de películas. La función entrega:

- Un `0` si la lista está desordenada.
- Un `1` si la lista está ordenada de menor a mayor.
- Un `2` si la lista está ordenada **estrictamente** de menor a mayor (es decir, la lista está ordenada y no hay películas repetidas).

El caso de una lista ordenada de mayor a menor se considera como una lista desordenada. Por simplicidad, consideraremos que todos los nombres están en minúsculas.

Ejemplos:

```python
LP1 = ["mi vecino totoro", "el castillo ambulante", "el viaje de chihiro"]
LP2 = ["kiki: entregas a domicilio", "la tumba de las luciérnagas", "mi vecino totoro"]
LP3 = ["el viaje de chihiro", "el viaje de chihiro", "la tumba de las luciérnagas"]
```

- `pelisOrdenadas(LP1)` entrega `0`.
- `pelisOrdenadas(LP2)` entrega `2`.
- `pelisOrdenadas(LP3)` entrega `1`.