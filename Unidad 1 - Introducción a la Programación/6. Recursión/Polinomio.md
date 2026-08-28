---
tags: [Recursión]
---

# Polinomio

Se desea calcular el resultado de evaluar un polinomio de la forma $a_{n}x^{n} + a_{n−1}x^{n−1} + ... + a_{2}x^{2} + a_{1}x+a_{0}$, para un numero x dado, con $a_i$ entre [0, 9].

Para esto, cree una función llamada ```evaluar(x,n)``` , que recibe un numero x que será el usado para evaluar el polinomio, y un número entero n que simboliza los coeficientes del polinomio, en su determinada posición, y entrega como resultado de evaluar el polinomio en x.

Por ejemplo el polinomio $7x^{3} + 5x+ 1$ codificado en número sería 7051, ya que en la posición 0 $(x^{0})$ hay un 1, en la posición 1 $(x^{1})$ hay un 5, en la posición 2 $(x^{2})$ hay un 0 debido a que no hay término cuadrático, y finalmente en la posición 3 $(x^{3})$ hay un 7. 

Luego: `evaluar(3, 7051)` entrega $7 \cdot 3^{3} + 0 \cdot 3^{2} + 5 \cdot 3^{1} + 1 \cdot 3 ^{0} = 189 + 0 + 15 + 1 = 205$.

