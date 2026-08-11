---
tags: [Control, Recursión, Programa Interactivo]
---

# RUN [C1 2016-02]


1. Escriba una función recursiva llamada ```sumaProductos(a, b)```, que reciba dos enteros positivos y entregue la suma de los productos entre sus dígitos.
   
    Por ejemplo
    
    - ```sumaProductos(12345, 6789)``` debe entregar ```110```, que es el resultado de 5*9 + 4*8 + 3*7 + 2*6 + 1*0 = 45 + 32 + 21 + 12 + 0.

2. Escriba una función llamada ```verificador(run)```, que reciba un entero de hasta 8 dígitos (que representa la parte del RUN que está antes del guión) y entregue un string con el dígito verificador (el valor que debe estar después del guión en el RUN). 
 
    **Indicación:**  Para calcular el dígito verificador se debe:

    - Usar la función `sumaProductos` con el entero de hasta 8 dígitos y el número `32765432`.
    - Calcular `D` como: 11 menos el resto de la suma anterior dividida por 11
    - Entregar ```"0"``` en caso el caso de que el valor `D` sea 10, ```"K"``` en caso el caso de que el valor `D` sea 11 o ```D``` (como string) en cualquier otro caso.
  
3. Use las funciones en un programa interactivo que lea un número entero con dígitos del RUN sin el guión, y escriba el RUN completo de acuerdo al diálogo indicado en el siguiente ejemplo:

    ```python
    >>> Ingrese los primeros 8 dígitos del RUN: 12345678
    RUN completo es 12345678-5
    ```