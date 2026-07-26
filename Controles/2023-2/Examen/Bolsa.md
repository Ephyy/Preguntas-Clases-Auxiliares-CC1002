---
tags: [Control, Clases y Objetos]
---

# La Bolsa (Variante EX 2023-02) 📦🍬

En el contexto de un concurso sorpresa, un grupo de Auxiliares necesita crear una Clase que permita modelar una Bolsa, de la cual se puedan ingresar dulces, y extraerlos al azar. La siguiente tabla describe los métodos disponibles de la clase:

| Método | Significado |
|---|---|
| `B = Bolsa(N)` | Crea la Bolsa `B` inicialmente vacía, y con capacidad máxima para `N` elementos. |
| `B.ingresar(elemento)` | Ingresa el elemento dentro de la Bolsa `B`. Entrega `True` si se pudo ingresar correctamente, o `False` si no se pudo agregar por falta de espacio. |
| `B.extraer()` | Extrae y entrega un elemento cualquiera de la Bolsa `B` (elegido al azar). Entrega `None` si la bolsa está vacía. |

Por ejemplo, un uso de la Bolsa sería el siguiente:

```python
# Se crea una bolsa de capacidad 4
>>> Dulces = Bolsa(4)
# Se ingresan 4 dulces
>>> Dulces.ingresar("suny")
    True
>>> Dulces.ingresar("loops")
    True
>>> Dulces.ingresar("trencito")
    True
>>> Dulces.ingresar("cereal bar")
    True
# Al intentar ingresar un 5°, no será posible
>>> Dulces.ingresar("frugele")
    False 
# Al extraer un dulce, me entrega aleatoriamente algún dulce de la bolsa
>>> Dulces.extraer()
    "loops"
```



Con esto, el grupo de auxiliares les pide ayuda con lo siguiente:

+ Escribir la Clase ```Bolsa``` con todos los métodos de la Tabla. Considere que internamente, una Bolsa contiene dos atributos:

  - ```self.elementos```: Una lista que guarda los distintos elementos que hay en la Bolsa.
  - ```self.capacidad```: Un entero que indica la capacidad máxima de elementos que pueden haber en la Bolsa

+ Escribir un test para la Clase ```Bolsa```, que permita probar el comportamiento de los 3 métodos.
