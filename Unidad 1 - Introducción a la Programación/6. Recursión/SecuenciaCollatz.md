---
tags: [Recursión]
dificultad: Media
---

# Secuencia de Collatz

En matemática existe un problema conocido como "Conjetura de Collatz", que plantea un proceso muy sencillo para generar una secuencia de números a partir de cualquier entero positivo.

El proceso comienza con un número N y, en cada paso, se reemplaza N según las siguientes reglas:

- Si `N` es par, el siguiente valor se obtiene dividiendo `N` por `2`.
- Si `N` es impar, el siguiente valor se obtiene multiplicando `N` por `3` y sumando `1`.
- El proceso termina cuando `N` alcanza el valor `1`.

Por ejemplo, comenzando con `N = 6`:

```
6 → 3 → 10 → 5 → 16 → 8 → 4 → 2 → 1
```

Cree una función de encabezado ```collatz(N)``` que reciba un número entero positivo `N` y muestre en pantalla todos los valores por los que pasa `N` hasta llegar a `1`.

Por ejemplo:

```python
>> collatz(6)
6
3
10
5
16
8
4
2
1
```