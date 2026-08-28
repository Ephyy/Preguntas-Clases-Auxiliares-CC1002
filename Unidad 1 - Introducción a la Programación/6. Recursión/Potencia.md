---
tags: [Recursión]
---

# Potencia 🅿️

Programe la función recursiva ```potencia(x, y)```, que calcula $x^{y}$ , con la restricción $y \in \mathbb{N}$. Para ello, considere la siguiente definición:

$$
x^y =
\begin{cases}
x^{\frac{y}{2}} \cdot x^{\frac{y}{2}} & \text{si } y  \text{ es par}\\
x \cdot x^{y-1} & \text{si } y  \text{ es impar} \\
1 & \text{si } y = 0 \\
\frac{1}{x^{y}} & \text{si } y < 0 \\
\end{cases}
$$

Ejemplos:

- ```potencia(3,2)``` entrega ```9```
- ```potencia(2,-3)``` entrega ```0.125```

