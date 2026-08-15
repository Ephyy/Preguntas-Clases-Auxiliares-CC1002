---
tags: [Control, Recursión]
---

# Números de Munchausen

Un número de Munchausen es un entero positivo que es igual a la suma de todos sus dígitos elevados a los mismos dígitos. Por ejemplo, 3435 es un número de Munchausen, puesto que la suma $3^3 + 4^4 + 3^3 + 5^5$ es igual a 3435. Asimismo, 1 es también un número de Munchausen, puesto que $1^1 = 1$

1. Escriba la función de encabezamiento ```def esMunchausen(N)```, que reciba un número entero positivo $N$ y devuelva ```True``` si el número $N$ es de Munchausen y ```False``` en caso contrario.

    **Notas:**
    - En caso que algún dígito del número sea igual a 0, se debe considerar que $0^0 = 0$. Por ejemplo, 438579088 también es un número de Munchausen, puesto que $4^4 + 3^3 + 8^8 + 5^5 + 7^7 + 9^9 + 0^0 + 8^8 + 8^8 = 438579088$
    - Debe escribir la receta de diseño, incluyendo al menos 2 pruebas (una para ```True``` y otra para ```False```) \
    - Defina y use una función auxiliar recursiva de encabezamiento ```def suma(N)``` que calcule la suma de las potencias (no necesita escribir la receta de diseño de esta función auxiliar).

2. Escriba una función recursiva (sin receta de diseño) de encabezamiento ```def primero(x,y)```, que entregue el primer número de Munchausen que esté entre `x` e `y` (ambos inclusive). Si no existe ninguno, debe entregar `-1` como resultado.

    Por ejemplo, ```primero(3000,4000)``` entregará el primer número de Munchausen que se encuentra entre 3000 y 4000, y ```primero(2,10)``` entregará -1, puesto que entre 2 y 10 no hay ningún número de Munchausen
