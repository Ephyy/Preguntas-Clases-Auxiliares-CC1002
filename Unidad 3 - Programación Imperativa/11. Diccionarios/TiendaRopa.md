# Tienda de Ropa 👗👢🎀🧣

Nicolás trabaja en una tienda súper conocida del retail, llamada *Falaferia*. En ella, mantienen el inventario de las poleras que tienen en bodega mediante un diccionario, donde la llave es el color de la polera, y el valor asociado a cada color es una lista con las tallas disponibles para las poleras de ese color.

Por ejemplo:

```python
Inventario = {
    'roja': ['XL', 'L', 'L', 'XS', 'XL', 'XS', 'S'],
    'azul': ['L', 'M', 'L', 'XS', 'XL', 'L', 'M', 'XS', 'XS'],
    'naranja': ['M', 'XS', 'S', 'S', 'M'],
    'morada': ['S', 'L', 'XL', 'XL', 'S', 'S', 'XS', 'M']
}
```

Con esto, Nicolás le pide ayuda a usted, una persona experta en diccionarios, para crear las siguientes funciones que le ayudarán mucho en su día a día en el trabajo:

- Cree la función `contarPoleras(Inv, talla, color)` que, dado un diccionario de poleras, una talla y un color, entrega cuántas poleras existen con el color y talla indicadas.

  Ejemplos:

  - `contarPoleras(Inventario, 'L', 'roja')` entrega `2`

  - `contarPoleras(Inventario, 'S', 'morada')` entrega `3`

- Cree la función `frecuencias(Inv)`, que dado un diccionario de poleras indexado por colores, entregue un diccionario de poleras indexado por tallas, asociado a la cantidad de poleras que tengan esa talla (sin importar el color).

  Ejemplo:

  ```python
  frecuencias(Inventario)
  ```

  entrega el diccionario:

  ```python
  {
      'XL': 5,
      'L': 6,
      'XS': 7,
      'S': 6,
      'M': 5
  }
  ```

- Cree la función `agregar(Inv, talla, color)`, que dado un diccionario de poleras, una talla y un color, agrega a tal diccionario una polera con el color y talla indicadas.

  Ejemplo:

  ```python
  agregar(Inventario, 'S', 'naranja')
  ```

  modifica el inventario original a:

  ```python
  Inventario = {
      'roja': [...],
      'azul': [...],
      'naranja': ['M', 'XS', 'S', 'S', 'M', 'S'],
      'morada': [...]
  }
  ```