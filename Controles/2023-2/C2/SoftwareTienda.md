---
tags: [Control, Listas Recursivas, Estructuras]
dificultad: Difícil
---

# Software de una Tienda

Una tienda mandó a construir un sotiware para manejar sus productos. Al ser una tienda pequeña, la persona a cargo de programar el sotiware hizo el siguiente diseño:

- La información asociada a un producto de la tienda se guarda en la estructura producto
- La cantidad disponible de un producto se guarda en la estructura item
- El stock de toda la tienda se guarda en una lista de ítems

```python
# producto: código(int) precio(int) tipo(str) nombre(str)
estructura.crear("producto", "codigo precio tipo nombre")

# item: producto(producto) cantidad(int)
estructura.crear("item", "producto cantidad")

P1 = producto(234564, 3500, "leche", "Soprole")
P2 = producto(323456, 1250, "legumbre", "Lenteja Superior")
P3 = producto(290083, 100, "confite", "Chicle 2en1")

stock = lista(item(P1, 10), lista(item(P2, 45), lista(item(P3, 234), None)))
```

Al respecto, escriba las siguientes funciones:

+ **(1.5 p)** La función ```cantidadDisponible(cod, L)```, que recibe un código de producto y una lista de stock, y retorna la cantidad disponible de ese producto. Si el producto no exista en el stock, entonces entregar 0. \
Por ejemplo, ```cantidadDisponible(323456, stock)``` entrega: ```45```

+ **(1.5 p)** La función ```reducirCantidad(cod, L)```, que recibe un código de producto y una lista de stock, y retorna una lista de stock, donde se rebajó en una unidad la cantidad del producto asociado al código indicado. \
Por ejemplo: ```reducirCantidad(234564, stock)``` entrega: \
```lista(item(P1, 9), lista(item(P2, 45), lista(item(P3, 234), None)))```

+ **(1.5 p)** La función ```precioProducto(cod, L)```, que recibe un código de producto y una lista de stock, y retorna el precio de venta asociado al producto. \
Por ejemplo: ```precioProducto(323456, stock)``` entrega: ```1250```

+ **(1.5 p)** Use las funciones anteriores para crear un programa interactivo, que solicite a un vendedor(a) el código de un producto, y realice una venta, de acuerdo con el diálogo indicado en el siguiente ejemplo:

  ```
  Ingrese código del producto? 234564
  El precio de venta es: 3500 pesos
  Luego de la venta quedarán 9 unidades del producto
  ```

  Nota: Si el producto no está en el stock, entonces debe mostrar el mensaje "Producto sin Stock"