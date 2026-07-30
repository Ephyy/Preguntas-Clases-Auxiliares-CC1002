---
tags: [Control, Funciones, Módulos, Programa Interactivo]
---
# Números Romanos [C1 2017-2]

El modulo de nombre romano contiene las funciones que se indican
en la siguiente tabla:

| Ejemplo 1            | Resultado  | Ejemplo 2           | Resultado | Significado                                                  |
|----------------------|------------|----------------------|-----------|---------------------------------------------------------------|
| decimal('V')         | 5          | decimal('I')         | 1         | Valor decimal de un dígito romano                            |
| decimal2('I','V')    | 4          | decimal2('V','I')    | 6         | Valor decimal de un número romano de 2 dígitos              |
| esValido('IV')       | True       | esValido('I5')       | False     | True si el número romano ingresado es correcto (False si no)|
| digito(1,'IV')       | 'I'        | digito(2,'IV')       | 'V'       | Primer o segundo dígito de un número romano  de 2 dígitos                |

a) Escriba la función ```decimal(n)``` , que toma un dígito romano y entrega su valor decimal. considere que los dígitos romanos I, V, X, L, C, D y M tienen los valores 1, 5, 10, 50, 100, 500 y 1000 respectivamente. La función debe entregar 0 en caso de recibir algo distinto a lo indicado anteriormente.

b) Escriba la función ```decimal2(n1,n2)``` , considerando que el primer dígito se resta del segundo dígito si su valor es menor y se suma al segundo si su valor no es menor. Si alguno de los parámetros no es un numero romano, entregar 0.

c) Escriba un programa que use las funciones del modulo romano para leer un numero romano de 2 dígitos, y muestra en pantalla el valor decimal correspondiente, de acuerdo al siguiente dialogo de ejemplo. En caso que el número romano no sea válido debe escribir el mensaje “numero romano incorrecto”

```python
Ingrese un numero romano: VI
El valor decimal es 6
```



