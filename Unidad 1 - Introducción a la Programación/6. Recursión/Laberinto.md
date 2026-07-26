# Escapando del Laberinto 🧩

Buscando las pautas legendarias en el edificio escuela, ha caído en una trampa oculta, por lo que cayó en las catacumbas de 850, donde todo está muy oscuro, hay interminables pasillos y no se ve una salida.

En medio de su desesperación, encuentra un viejo documento, que al leerlo con la luz de su celular, se da cuenta que es un código en clave para poder encontrar la salida del laberinto, como si fuese un mapa del tesoro, donde el tesoro es escapar con vida de este lugar.

En el documento, se explica que la cantidad de pasos a moverse será representada por un dígito del `1` al `9`, mientras que la dirección se puede representar por un dígito del `1` al `4`, donde:

- `1` significa moverse hacia arriba.
- `2` significa moverse hacia la derecha.
- `3` significa moverse hacia abajo.
- `4` significa moverse hacia la izquierda.

Entonces, por ejemplo:

- `15` indica que se mueve 5 pasos hacia arriba.
- `42` indica que se mueve 2 pasos hacia la izquierda.

Y el código para llegar a la salida está representado por una cadena de números, siguiendo la nomenclatura anterior (por ejemplo: `32413512`).

Primero, para orientarse, necesita saber dónde se encuentra espacialmente la salida, para lo cual cree las siguientes funciones (asuma que se encuentra en el punto `(0, 0)`).

**a)** Cree la función `movHoriz(C)`, que recibe un número entero que representa una secuencia de movimientos, y entrega cuál es el desplazamiento neto en el eje horizontal.

Ejemplo:

- `movHoriz(32413512)` entrega `-1`.

**b)** Cree la función `movVert(C)`, que recibe un número entero que representa una secuencia de movimientos, y entrega cuál es el desplazamiento neto en el eje vertical.

Ejemplo:

- `movVert(32413512)` entrega `-5`.

**c)** Luego, cree la función `ruta(C)`, que va mostrando en pantalla los pasos que hay que dar en cada dirección, de acuerdo a la secuencia de movimientos recibida (leída de izquierda a derecha).

Por ejemplo:

```python
>>> ruta(32413512)

debes moverte 2 pasos hacia arriba
debes moverte 5 pasos hacia abajo
debes moverte 1 pasos hacia la izquierda
debes moverte 3 pasos hacia abajo
```

**d)** Finalmente, cree un programa interactivo, que nos muestra el camino a la salida, de acuerdo con el siguiente diálogo de ejemplo:

```python
Ingrese secuencia de movimientos: 32413512

La salida se encuentra en: (-1, -5)

Para llegar:
debes moverte 2 pasos hacia arriba
debes moverte 5 pasos hacia abajo
debes moverte 1 pasos hacia la izquierda
debes moverte 3 pasos hacia abajo

Ojalá hayas logrado escapar!
```