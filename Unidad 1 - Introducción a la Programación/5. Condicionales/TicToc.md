---
tags: [Condicionales]
---

# TicToc

El juego del TicToc se usa a menudo para que los niños aprendan a dividir. Este consiste en que los jugadores se van turnando diciendo consecutivamente los números desde el 1 en adelante. Cuando el número que toca en la ronda es divisible por 3, deben decir `"Tic"`, cuando es divisible por 5, `"Toc"`, y cuando es divisible simultáneamente por 3 y 5 deben decir `"TicToc"`. 

Escriba una función de encabezado ```tictoc(n)``` , la cual recibe un número positivo cualquiera y, de acuerdo a las reglas del juego, devuelva ’Tic’, ’Toc’ o ’TicToc’, o bien, un string vacío ('') si no cumple la regla. 

Por ejemplo:

```python
>> tictoc(1)
''
>> tictoc(3)
'Tic'
>> tictoc(5)
'Toc'
>> tictoc(15)
'TicToc'
```