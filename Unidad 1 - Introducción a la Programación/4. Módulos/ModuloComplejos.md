---
tags: [Funciones, Módulos, Programa Interactivo]
---

# Números Complejos

Recordemos que la formula de euler para números complejos establece que:

$$ e^{i\theta} = cos(\theta) + i \cdot sen(\theta) $$

Donde $i$ es la unidad imaginaria y $\theta$ es un ángulo en radianes

Crearemos un **módulo** llamado `trigonometria.py` con las siguientes funciones:

1. La función `parteReal(angulo)` que recibe un ángulo en sistema sexagesimal
y retorne su coseno.

2. La función `parteImaginaria(angulo)` que recibe un ángulo en sistema sexagesimal y entregue su seno.

3. Ahora, en **otro archivo**, cree un script llamado `interactivo.py`, que importe el módulo `trigonometria.py` y genere el siguiente dialogo:

    ```python
    >> Angulo? 180   // recibe el ángulo como input
    e^(i*180) = -1.0 + i*1.22464679915e-16   // entrega la expresión en forma compleja
    ```

**Indicación:** 
Utilice el modulo `math` y que:

$$ Re(e^{i\theta}) = cos(\theta) $$
$$ Im(e^{i\theta}) = sin(\theta) $$







