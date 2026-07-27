---
tags: [Estructuras]
---

# Alimentos 🍔🍎

Un alimento se puede representar mediante diversas características, como por ejemplo:

- Nombre (`str`)
- Calorías (`int`)
- N° de sellos (`int`)
- Vegan Friendly (`bool`)

Al respecto:

+ Cree la estructura `Alimento`, de acuerdo a las características anteriores.

+ Cree los siguientes alimentos, guardándolos en variables:

  - `AL1`: Big Mac, 563 calorías, 3 sellos, not vegan.
  - `AL2`: Manzana, 95 calorías, sin sellos, vegan.
  - `AL3`: Ensalada Lechuga-Tomate, 260 calorías, sin sellos, vegan.
  - `AL4`: Galletas Oreo, 170 calorías, 4 sellos, vegan.
  - `AL5`: Papas Fritas Kryzpo, 188 calorías, 2 sellos, not vegan.

+ Cree la función `esAlimento(x)`, que recibe cualquier cosa, y se encarga de indicar si cumple con ser una estructura alimento bien formada o no (de acuerdo a los criterios anteriores). Ejemplo:

  - `esAlimento(AL1)` entrega `True`.

+ Cree la función `esVegan(A)`, que recibe un `Alimento`, e indica si el alimento cumple con ser vegan o no. Ejemplo:

  - `esVegan(AL1)` entrega `False`.

+ Cree la función `mayorSellos(A1, A2)` que recibe 2 alimentos, y entrega el que tenga la mayor cantidad de sellos. En caso de empate, arbitrariamente se entrega el alimento `A1`. Ejemplo:

  - `mayorSellos(AL1, AL4)` entrega `Alimento("Galletas Oreo", 170, 4, True)`.

+ Cree la función `masSano(A1, A2)`, que recibe 2 alimentos, y entrega el alimento más sano, de acuerdo al siguiente criterio:

  - Se prefieren alimentos vegan.
  - Luego se prefieren los que tengan menos sellos.
  - Luego se prefiere el que tenga menos calorías.

  Ejemplo:

  - `masSano(AL2, AL4)` entrega `Alimento("Manzana", 95, 0, True)`.