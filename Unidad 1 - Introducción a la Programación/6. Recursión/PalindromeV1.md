---
tags: [Recursión]
---

# Palindrome (Variante 1)

Un dia mirando uno de los ventanales de la facultad, notó que ocurre un fenómeno curioso… todo lo que se ve en el espejo, está reflejado, sean números, diseños o pautas de controles. Preguntándose si es posible hacer algo parecido en Python, se propone a programar lo siguiente:


a) Cree la función recursiva ```invertir(N)```, que recibe un número entero positivo, y entrega el mismo
número, pero en orden inverso. Ejemplos:
- ```invertir(45397)``` entrega ```79354```
- ```invertir(777)``` entrega ```777```
  
Indicaciones:
- Por simplicidad, puede asumir que el número de más a la derecha no será un cero.
- Le puede ser de utilidad usar la función ```digitos(N)``` vista en clases.

b) Cree la función ```palindrome(N)`, que recibe un número entero positivo, y entrega True si el número se escribe igual al revés y al derecho, y False en caso contrario. Ejemplos:
- ```palindrome(1748)``` entrega ```False```
- ```palindrome(1223221)``` entrega ```True```

