---
tags: [Clases y Objetos]
---

# Polidemonios 😈😈

Un polinomio, también conocido como *Polidemonios*, es una expresión algebraica formada por la suma de varios monomios o términos, que probablemente ya le han atormentado en varios cursos matemáticos. En particular, un polinomio $P(x)$ de grado $n$ puede ser escrito de la forma

$$
P(x) = a_0 + a_1x + a_2x^2 + \dots + a_nx^n
$$

en donde los $a_i$ son coeficientes reales, con $i = 0, 1, 2, \dots, n$. (Note que son $n+1$ coeficientes).

En base a eso, con el objetivo de ganar un poco de dominio sobre estas malvadas expresiones, se le pide implementar la clase `Polinomio`, cuyo constructor recibe como parámetro una lista de $n+1$ coeficientes.

Por ejemplo, ```P = Polinomio([1,2,3])```, donde `P` representa el polinomio $1 + 2x + 3x^2$.

1. Cree el constructor de la clase `Polinomio`, en donde su representación interna es una lista de Python que guarda los coeficientes del polinomio. El i-ésimo índice de la lista almacena el coeficiente $a_i$ del polinomio.

   Por ejemplo, para representar al polinomio $P(x) = 1 + 2x + 3x^2$, la lista interna debe quedar como:

   ```python
   self.__coefs = [1,2,3]
   ```

2. Implemente el método ```mostrar(self)```, que muestra en pantalla el polinomio, siguiendo la siguiente notación: `"coef*x**potencia + ..."`.

   Por ejemplo:

   ```python
   >> P = Polinomio([1,2,3])
   >> P.mostrar()
   '1*x**0 + 2*x**1 + 3*x**2'
   ```

3. Implemente el método ```evaluar(self, x)``` que retorna el resultado de evaluar el polinomio en el número $x$.

   Por ejemplo, si evaluamos $P(x)=1+2x+3x^2$ en $x=2$, obtenemos $1+2∗2^1+3∗2^2=1+4+12=17$.

   ```python
   >> P = Polinomio([1,2,3])
   >> P.evaluar(2)
   17
   ```

4. Implemente el método ```__add__(self, P2)``` que retorne el polinomio resultante de la suma entre `P1` y `P2`.

   Por ejemplo:

   - Si $P_1(x)=1+2x+3x^2$
   - Si $P_2(x)=4$
   - Entonces $P_1(x)+P_2(x)=5+2x+3x^2$

   ```python
   >> P1 = Polinomio([1,2,3])
   >> P2 = Polinomio([4])
   >> P3 = P1.sumar(P2)
   >> P3.mostrar()
   '5*x**0 + 2*x**1 + 3*x**2'
   ```

**(Propuesto 1)** Implemente los métodos `__str__` y `__repr__`, que muestran un objeto `Polinomio` como lo realizado en la parte (B).

**(Propuesto 2)** Realice nuevamente este ejercicio, pero ahora suponiendo que internamente el polinomio se representa con un diccionario de Python, en donde las llaves representan la i-ésima potencia, y sus valores asociados representan el valor del coeficiente que acompaña a tal potencia.

Por ejemplo, para representar al polinomio $P(x)=1+2x+3x^2$, el diccionario interno debe quedar como: `self.__coefs = {0:1, 1:2, 2:3}`
