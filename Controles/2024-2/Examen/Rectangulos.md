---
tags: [Control, Estructuras, Árboles Binarios]
dificultad: Media
---

# Rectángulos ⬜

Un rectángulo se puede representar mediante estructuras, almacenando las coordenadas del vértice superior izquierdo y del vértice inferior derecho:

```python
# Rectangulo: int int int int
estructura.crear('Rectangulo', 'X1 Y1 X2 Y2')
R1 = Rectangulo(1, 6, 6, 2)
R2 = Rectangulo(4, 5, 5, 3)
R3 = Rectangulo(4, 1, 6, 0)
R4 = Rectangulo(2, 3, 3, 1)
```

![Rectangulo](./img/rectangulo.png)


Al respecto, programe las siguientes funciones:

+ **(2.0p)** Escriba la función ```estaContenido(RA, RB)```, que recibe dos Rectángulos, y entrega ```True``` si el Rectángulo `RB` está contenido o encerrado dentro del Rectángulo `RA`, y ```False``` en cualquier otro caso. Asuma que las coordenadas de cada rectángulo son coherentes (X1 < X2 y Y1 > Y2).

  Ejemplos:

  - ```estaContenido(R1, R2)``` entrega ```True```
  - ```estaContenido(R1, R3)``` entrega ```False```
  - ```estaContenido(R1, R1)``` entrega ```True```
  - ```estaContenido(R1, R4)``` entrega ```False```

+ **(4.0p)** Un Árbol Binario de Rectángulos (ABR) permite agrupar un conjunto de rectángulos, de tal manera que en cada valor del AB se almacena un rectángulo, y los rectángulos almacenados en los árboles izquierdo y derecho deben estar contenidos en el rectángulo almacenado en la raíz del árbol. Por ejemplo, para el siguiente árbol:

  ```python
  ABR1 = AB(T1,
            AB(T2, arbolVacio, arbolVacio),
            AB(T3,
                AB(T4, arbolVacio, arbolVacio),
                AB(T5, arbolVacio, arbolVacio)))
  ```

  ![Árbol Binario de Rectángulos](./img/rectangulo(parte2).png)

  Los Rectángulos `T2` y `T3` están contenidos en `T1` y a su vez, `T4` y `T5` están contenidos en `T3`.

  Escriba la función ```validarArbol(A)```, que recibe un árbol de rectángulos como el de la figura, y valida que esté bien construido (usando la función `estaContenido`, aunque no la haya implementado), es decir, que los rectángulos de los subárboles izquierdo y derecho estén contenidos en el rectángulo de la raíz del árbol, entregando ```True``` en ese caso y ```False``` en cualquier otro escenario. Por ejemplo:

  - ```validarArbol(ABR1)``` entrega ```True```