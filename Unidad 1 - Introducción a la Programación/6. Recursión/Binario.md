---
tags: [Recursión]
---

# Binario

1. Cree una función recursiva llamada `convertirABinario`, que recibe un entero positivo $n$, y entrega su codificación en binario como un string.

    Un numero entero se convierte a binario dividiéndolo sucesivamente por 2, y uniendo los restos de estas divisiones de derecha a izquierda en el orden que fueron realizadas. Las divisiones sucesivas terminan cuando el numero a dividir es 0 o 1.

    **Ejemplo:** ```convertirABinario(13)``` entrega ```"1101"```

2. Cree una función llamada ```mostrarBinarios```, que recibe un entero positivo, e imprime en pantalla la codificación binaria de todos los números desde 0 hasta `n` en orden descendiente (n, n − 1, ..., 2, 1, 0).

   Ejemplo:

   ```python
   >> mostrarBinarios(5)
   '101'
   '100'
   '11'
   '10'
   '1'
   '0'
   ```
