---
tags: [Funciones]
---
# Herón

Una forma conocida para calcular el área de un triángulo es la formula de Herón:

$$ A = \sqrt{S(S − a)(S − b)(S − c)} $$

donde a, b, c son los lados del triángulo, y S es el semi-perímetro del mismo.

1. Cree una función llamada ```semiPerimetro(a, b, c)``` que reciba tres números correspondientes a los lados del triángulo, y entregue el semi-perímetro de este.
2. Usando la función anterior, escriba la función ```Heron(a, b, c)``` , que recibe también tres números correspondientes a los lados, y entrega como resultado, el cálculo del área de este triángulo.

    **Nota:** No hace falta verificar que los lados cumplen la desigualdad triangular, asuma que los lados entregados la cumplen.