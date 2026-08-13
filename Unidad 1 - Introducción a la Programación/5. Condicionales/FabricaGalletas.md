---
tags: [Condicionales, Módulos, Funciones, Programa Interactivo]
---

# Fabrica de Galletas

Una fabrica de galletas tiene a la venta las siguientes variedades de galletas:

| Producto          | Sabor Vainilla | Sabor Chocolate  | Sabor Frutilla |
|-------------------|----------------|------------------|----------------|
| Galleta Circular  | 50             | 60               | 55             |
| Galleta Cuadrada  | 70             | 90               | 65             |

Como acude frecuente a comprar a esta fabrica (ya que son las MEJORES galletas de la vida), le parece una buena idea crear un par de funciones para calcular cuanto le costará comprar una determinada cantidad de galletas de cierta forma y sabor. Para esto, cree un modulo llamado
`galletas`, con las siguientes funciones:

1. Cree la función ```galletaCuadrada(N, sabor)```, que recibe una numero `N` que indica la cantidad de galletas y un String que indica el sabor elegido para la galleta. La función debe entregar el precio total para esa cantidad y sabor de galletas, de acuerdo a la tabla.

2. Cree la función ```galletaCircular(N, sabor)```, que recibe una numero `N` que indica la cantidad de galletas y un String que indica el sabor elegido para la galleta. La función debe entregar el precio total para esa cantidad y sabor de galletas, de acuerdo a la tabla.

3. Para facilitar el uso de estas funciones, le parece buena idea crear un programa interactivo que le permita calcular amigablemente cuanto le costará comprar una bolsa con un surtido de galletas. Con ayuda del modulo anterior, cree un programa interactivo que pregunte por la cantidad de galletas de cada tipo y sabor que se desean comprar, y muestre en pantalla el precio total, siguiendo el dialogo del siguiente ejemplo:

    (Las lineas con un * al principio es donde se espera que el usuario ingrese algo)

    ```python
    Programa para calcular el precio de las MEJORES galletas :3
    * Cantidad de Galletas Cuadradas? 0
    * Cantidad de Galletas Circulares? 7
    * Sabor? Chocolate
    Necesitas 420 pesos para comprar todas esas galletas :)
    ```

    **Ind:** Por capricho de la fabrica, considere que no es posible comprar galletas con la misma forma, pero distinto sabor en un mismo día. Note que al ingresar una cantidad de 0 galletas, el programa interactivo no pregunta por el sabor. Asuma que todos los valores ingresados al programa serán validos.