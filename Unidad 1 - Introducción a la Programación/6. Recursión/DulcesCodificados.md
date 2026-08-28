---
tags: [Recursión]
---

# Dulces Codificados 

En cierta tienda, un pedido de dulces se codifica como un número entero, donde cada cifra indica un tipo de dulce predeterminado (de 9 tipos que ofrece la tienda). Por ejemplo: `422454` codifica que se quieren 3 dulces de tipo 4, 2 dulces de tipo 2 y 1 dulce de tipo 5.

La tienda le pide ayuda para crear una forma de entender y procesar estos pedidos más fácil y rápidamente. Por lo mismo, se le pide que:

1. Cree una función recursiva ```contarDulces(n,p)``` , que dado un entero `n` y un entero `p` (con 0 <= p <= 9), entrega como resultado cuantas veces se repite el tipo de dulce `p` en el pedido codificado como el número `n`. Ejemplo: 
     - ```contarDulces(143412549,4)``` entrega ```3```

2. Cree una función ```mostrarPedido(n)``` , que recibe un número entero `n`, el cual representa un pedido, y muestra en pantalla la cantidad que se ordenó de cada tipo de dulce. Ejemplo:

    ```python
    >>> mostrarPedido(93789436)
    el dulce 0 se repite 0 veces
    el dulce 1 se repite 0 veces
    ...
    el dulce 8 se repite 1 veces
    el dulce 9 se repite 2 veces
    ```