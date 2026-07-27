---
tags: [Estructuras]
---

# Fracciones ➗

En clases se vio la estructura `Fraccion` y algunas funciones que operan con fracciones. Ahora realizaremos más funcionalidades que permiten extender la utilidad de esta estructura.

Para ello, considere la siguiente definición de la estructura:

```python
# Fraccion: numerador(int) denominador(int)
estructura.crear("Fraccion", "numerador denominador")
```

Y las siguientes fracciones de ejemplo:

```python
Frac1 = Fraccion(5, 8)
Frac2 = Fraccion(1, 3)
Frac3 = Fraccion(3, 12)
Frac4 = Fraccion(1, 4)
```

+ Cree la función `fracToStr(F)` que recibe una `Fraccion`, y entrega un string con la representación de la fracción `F` como un texto. Por ejemplo:

  - `fracToStr(Frac1)` entrega `"5/8"`.

+ Cree la función `simplificar(F)`, que recibe una `Fraccion`, y entrega una `Fraccion` que representa la forma simplificada de `F`. Ejemplo:

  - `simplificar(Frac3)` entrega `Fraccion(1, 4)`.

  Indicación: la función `math.gcd` del módulo `math` permite calcular el Máximo Común Divisor entre 2 cantidades.

+ Cree la función `restar(F1, F2)`, que recibe 2 fracciones y entrega la `Fraccion` que representa la resta entre `F1` y `F2` (`F1 - F2`). Ejemplo:

  - `restar(Frac1, Frac2)` entrega `Fraccion(7, 24)`.

+ Cree la función `multiplicar(F1, F2)`, que recibe dos fracciones, y entrega como resultado una `Fraccion`, que representa el resultado de la multiplicación de ambas fracciones. Ejemplo:

  - `multiplicar(Frac1, Frac2)` entrega `Fraccion(5, 24)`.

+ Cree la función `dividir(F1, F2)`, que recibe dos fracciones, y entrega como resultado una `Fraccion`, que representa el resultado de la división de ambas fracciones. Ejemplo:

  - `dividir(Frac1, Frac2)` entrega `Fraccion(15, 8)`.

+ Cree la función `iguales(F1, F2)` que recibe dos fracciones, y entrega `True` si es que ambas fracciones representan la misma cantidad (y `False` si no).

  Indicación: para evitar problemas de precisión con decimales, le puede servir que:

  $$
  \frac{a}{b} = \frac{c}{d}
  \iff
  a \cdot d = b \cdot c
  $$

  Ejemplo:

  - `iguales(Frac3, Frac4)` entrega `True`.