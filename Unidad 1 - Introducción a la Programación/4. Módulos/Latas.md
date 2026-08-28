---
tags: [Módulos, Funciones, Programa Interactivo]
---
# Latas

Daniel trabaja para una reconocida embotelladora de jugos y bebidas (y otros líquidos refrescantes), y opera en la división que se encarga de los productos envasados en lata. Para la embotelladora, el costo de producir un producto enlatado, viene dado por el volumen de liquido a utilizar para llenar la lata, y la etiqueta o publicidad que se colocará en su contorno y tapas. Daniel recibe todos los días una planilla con nuevas propuestas de latas (cilindros de distinta altura y radio), y debe calcular el costo de cada una de estas propuestas.
Actualmente, este calculo lo realiza a mano, lo cual le quita mucho tiempo de trabajo, por
lo cual, acude a usted (quien tiene vastos conocimientos de programación) para que haga un
programa que le ayude a realizar estos cálculos con ayuda del computador. Para esto:
(Asuma que todas las medidas de distancia son dadas en centímetros)

**a)** Escriba un modulo llamado `cilindro.py`, que tenga funciones que calculen el área y volumen de un cilindro, dadas la altura y el radio del cilindro.

```python
def area(radio,altura):
...

def volumen(radio,altura):
...
```

**b)** Utilizando el modulo anterior, escriba una función `costoLata` que calcule el costo de realizar una lata de altura $h$ y radio $r$. Esta función recibe como parámetros los valores de h y r.

La función de costo es:

$$ CostoLata(area, volumen) = 3.2 \cdot volumen + \sqrt{area^{3}} + 754 $$

**Hint:** Recuerde que el área y el volumen del cilindro están en función de la altura y el radio de tal cilindro.

**c)** Cree una función interactiva que consulte al usuario el valor del radio y altura de un cilindro, y muestre en pantalla el costo de crear una lata de esas características. Considere el siguiente dialogo como ejemplo:

```python
>> programa()
Bienvenido al programa que calcula el costo de producir una lata
Ingrese radio: ...
Ingrese altura: ...
El costo de producir una lata de estas caracteristicas es de ___ pesos
```


