---
tags: [Control, Listas Recursivas, Estructuras]
---

# Baraja de Naipes francés

Una baraja de naipe francés se compone de cartas, donde cada una tiene una **pinta** (Corazón, Diamante, Trébol o Pica) y un **valor** (A, 2, 3, ..., 9, 10, J, Q, K). Al respecto, una Carta puede ser representada por la siguiente estructura:

```python
# Carta: pinta(str) valor(int)
estructura.crear("Carta","pinta valor")
```

Por simplicidad se representa el valor como un número entero entre 1 y 13 (A=1, J=11, Q=12, K=13), y la pinta por la letra inicial de cada una ('C', 'D', 'T', 'P'). No se consideran naipes conocidos como ''Comodín'' o ''Joker''.

Una mano de cartas puede ser representada como una lista de estructuras `Carta`. No existe un largo mínimo ni máximo para la lista. Por ejemplo, las cartas: 8 de Corazones, Rey de Diamante y As de Pica, se pueden representar con la siguiente lista:

```python
L1 = lista(Carta('C', 8), lista(Carta('D', 13), lista(Carta('P', 1), listaVacia))) 
```

En una mano de cartas pueden existir las siguientes combinaciones de cartas:

- **Par:** Dos cartas con el mismo valor, sin importar la pinta. En el caso que una misma carta sirva para formar más de un par con otra carta, solo se considera una combinación, es decir, si tengo 3 cartas de igual valor solo hay un “par”, si tengo 4 cartas de igual valor son dos “pares”.
- **Escalera:** La mano completa debe ser una secuencia de 3 o más valores consecutivos en orden creciente de la misma pinta. En el caso del Rey (K=13) se considera que su continuación es el As (A=1), y se le denomina Escalera cíclica.

Al respecto, se quieren definir funciones que permitan ayudar a construir un juego de cartas. 

**Indicaciones:**
- Suponga que existe la función ```largo(L)```, que devuelve la cantidad de cartas en la lista `L`.
- Para los ejemplos de las funciones, supondremos la existencia de las siguientes listas de cartas:

```python
LC1 = lista(Carta('P', 2), lista(Carta('D', 2), lista(Carta('T', 2), lista(Carta('T', 5), lista(Carta('D', 5), listaVacia)))))
LC2 = lista(Carta('P', 2), lista(Carta('T', 5), lista(Carta('D', 2), lista(Carta('D', 5), lista(Carta('T', 2), listaVacia)))))
LC3 = lista(Carta('T',12), lista(Carta('T',13), lista(Carta('T', 1), lista(Carta('T', 2), listaVacia))))
LC4 = lista(Carta('T',13), lista(Carta('T', 1), lista(Carta('T', 2), lista(Carta('T',12), listaVacia))))
LC5 = lista(Carta('D',11), lista(Carta('P',12), lista(Carta('C',13), listaVacia))) 
```

+ **(2.2p)** Escriba la función recursiva ```pares(L)```, que recibe una lista de Cartas. La función entrega una lista con las cartas de la lista que forman pares, siguiendo el mismo orden de la lista original. Los pares solo se pueden formar entre dos cartas consecutivas en la lista.
   
  Ejemplos:
  - ```pares(LC1)``` entrega:
  ```lista(Carta('P', 2), lista(Carta('D', 2), lista(Carta('T', 5), lista(Carta('D', 5), listaVacia))))```
  - ```pares(LC2)``` entrega: ```listaVacia```

+ **(2.2p)** Escriba la función recursiva ```consecutivos(L)```, que recibe una **lista de Cartas**. La función indica si **todas** las cartas en la lista son valores consecutivos y además comparten la misma pinta, siguiendo el mismo orden de la lista original.
  
  Ejemplos:
  - ```consecutivos(LC3)``` entrega: ```True```
  - ```consecutivos(LC4)``` entrega: ```False```
  - ```consecutivos(LC5)``` entrega: ```False```

+  **(1.6p)** Escriba la función ```puntaje(L)```, que recibe una **lista de Cartas**, y asigna una puntuación a las Cartas en la lista (en el orden que vienen), de acuerdo con el siguiente criterio:
   - Cada par de cartas aporta 3 puntos.
   - Una escalera (ver definición arriba) aporta 2 puntos multiplicado por el largo de la escalera.
  
    Ejemplos:
    - ```puntaje(LC1)``` entrega: ```6```
    - ```puntaje(LC3)``` entrega: ```8```