---
tags: [Recursión, Módulos, Programa Interactivo]
---

# Tiendita

En la tienda modular, tienen el módulo tiendita, que provee las siguientes funciones para trabajar con los productos de una tienda:

| **Función**               | **Descripción**                                                                 | **Ejemplo**                                   |
|------------------------|------------------------------------------------------------------------------|-------------------------------------------|
| ```precio(nombre)```         | Entrega el precio de un producto, dado su nombre                             | ```precio('kuky')``` entrega ```1380```               |
| ```oferta(nombre) ```        | Indica si el producto tiene un % de oferta                                   | ```oferta('kuky')``` entrega ```0.1``` (10% de oferta)|
| ```calcularImpuesto(nombre)```| Indica si el producto paga algún % de impuesto sobre el precio final (ej. IVA) | ```calcularImpuesto('kuky')``` entrega ```0.19``` (19% de impuesto) |
| ```escanear(codigo)```       | Recibe un número entero que representa un código de barras y entrega el nombre del producto | ```escanear(1002421445)``` entrega ```'kuky'``` |


Al respecto, cree un programa que permita realizar la siguiente interacción:
- Preguntar por el nombre de un producto.
- Muestra en pantalla su precio, si es que está en oferta, y el precio final luego de aplicar descuentos e
impuestos.
- Pregunta por otro producto.
- Eventualmente cuando se ingrese "fin", el programa muestra el precio final de la compra.

Ejemplo de dialogo esperado:

```python
nombre producto? kuky 
precio: 1380
oferta: 10% de descuento
impuesto: 19%
precio final: 1478

nombre producto? ...
...
nombre producto? fin
El total de la compra es: 16452
```

Use las funciones del módulo, y cree todas las funciones auxiliares que considere necesarias.