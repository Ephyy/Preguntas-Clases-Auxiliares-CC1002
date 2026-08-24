---
tags: [Recursión, Programa Interactivo, Función Interactiva]
titulo: Palindrome (Variante 2)
---

# Palindrome (Variante 2)

1. Cree una función llamada ```invertir(n)```, que recibe un número entero no negativo, y entrega el mismo número con sus dígitos en el orden inverso.

    Por ejemplo: ```invertir(3684)``` entrega ```4863```.

2. Se dice que un número es palíndromo, si es igual a su inverso. Cree una función llamada ```palindromo(n)```, que recibe un número entero no negativo, y entrega como resultado un valor booleano, que indica si el número es palíndromo o no.

    Por ejemplo:
    - ```palindromo(7767)``` entrega ```False```
    - ```palindromo(121)``` entrega ```True```


3. Cree una función interactiva llamada ```inversor()```, que le pregunta eternamente a un usuario por un número, y este programa le muestra en pantalla el inverso del número ingresado, y un mensaje indicando si el número es palindromo o no. En el caso que el usuario ingrese un número negativo, el programa termina. Ejemplo:

    ```python
    inversor()
    >> ingrese Numero: 753
    El inverso es 357
    No es palíndromo
    >> ingrese Numero: 1001
    El inverso es 1001
    Si es palíndromo
    >> ingrese Numero: -8000
    Fin
    ```

