---
tags: [Recursión]
---

# Números N-drónicos

Los números N-drónicos son números como cualquier otro, pero poderosos! ya que cuentan con la siguiente propiedad: son múltiplos de la suma de sus dígitos, pero solo si la suma de sus dígitos es mayor a 1. Se le pide crear un programa, que entregue un string con todos los números N-drónicos en un rango dado. Para esto:

1. Cree una función recursiva llamada ```sumarDigitos(n)```, que recibe un numero entero positivo, y entrega como resultado la suma de los dígitos de tal numero.
   
2. Cree una función llamada ```Ndronico(n)```, que recibe un numero entero, y entrega como resultado un valor booleano que indica si el numero es N-drónico o no.

3. Finalmente, usando la función `Ndronico`, cree una función recursiva de encabezado ```listaNdronicos(x, y)```, que recibe como parámetros dos enteros positivos `x` e `y`, y entrega un string con todos los números N-drónicos, presentes en el intervalo cerrado $[x, y]$. 
   
   Por ejemplo:
     - ```listaNdronicos(20, 30)``` entrega como resultado ```"20 21 24 27 30"```
     - ```listaNdronicos(13, 16)``` entrega ```""```, ya que no hay números N-drónicos en ese rango.