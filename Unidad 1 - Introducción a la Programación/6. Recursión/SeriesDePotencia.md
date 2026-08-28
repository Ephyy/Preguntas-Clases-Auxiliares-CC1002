---
tags: [Recursión]
---

# Series de Potencia

a) Cree una función llamada ```armonica(n)```, que permita calcular la serie:

$$ \sum_{k=1}^{n} \frac{1}{k} = 1 + \frac{1}{2} + \frac{1}{3} + \cdots + \frac{1}{n} $$


Con n términos. Por ejemplo:

- ```armonica(2)``` entrega ```1.5```


b) Cree una función llamada ```binpow(n)```, que permita calcular la serie:

$$ \sum_{k=0}^{n} \frac{1}{2^k} = 1 + \frac{1}{2} + \frac{1}{4} + \cdots + \frac{1}{2^n} $$

Con n terminos, Por ejemplo:

- ```binpow(3)``` entrega ```1.75```

c) Cree una función llamada ```taylor(x, n)```, que permita calcular la serie de taylor de la función $sin(x)$:

$$ \sum_{k=0}^{n} \frac{(-1)^k \cdot x^{2k+1}}{(2k+1)!} = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \cdots + \frac{(-1)^n x^{2n+1}}{(2n+1)!} $$

Con n términos. Por ejemplo:

- ```taylor(1.57 , 5)``` entrega aprox. ```1.0```


