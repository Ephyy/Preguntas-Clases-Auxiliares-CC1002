---
tags: [Recursión]
titulo: Números Primos (Variante 1)
---

# Números Primos (Variante 1)

a) Cree una función llamada ```esPrimo(n)``` , que entrega True si n es primo y False si no. Recuerde que un numero primo es aquel que solo puede ser dividido por 1 y por si mismo.

**Ind:** Cree una función recursiva auxiliar.

b) Usando la función anterior, cree una función recursiva llamada ```primosEnRango(x,y)```, que retorna un string con todos los números primos presentes en el intervalo $[x, y]$, separados por espacio.

```python
>> primosEnRango(10, 20)
"11 13 17 19 "
>> primosEnRango(70, 80)
"71 73 79 "
```

c) Finalmente usando la parte anterior, cree una función llamada ```tablaPrimos(ini,fin)``` que imprime en pantalla los números primos desde ini hasta fin, en intervalos de largo 10. Si el intervalo es más grande que fin, debe cortarse, como se ve en el siguiente ejemplo:

```python
>> tablaPrimos(10, 35)
Primos en el rango 10-20
11 13 17 19
Primos en el rango 20-30
23 29
Primos en el rango 30-35 # el intervalo no es 30-40 pues 40 es mayor a fin (35)
31
```
