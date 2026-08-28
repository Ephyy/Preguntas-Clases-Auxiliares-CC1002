---
tags: [Control, Árboles Binarios]
---

# Árboles Celulares (P2 C2 2019-02)

Considerando que un árbol binario se define como:

```python
# AB: valor(any) izq(AB) der(AB)
estructura.crear("AB", "valor izq der")
```

Un árbol binario se considera un **árbol celular** si:

- El valor de un nodo es mayor que los valores de sus hijos izquierdo y derecho.
- El valor de un nodo es mayor o igual a la suma de los valores de sus hijos izquierdo y derecho.
- Los subárboles izquierdo y derecho de un nodo también cumplen con ser **celulares**.
- Un árbol vacío y un nodo hoja cumplen con ser **celulares**.

Por ejemplo, el siguiente árbol binario es **celular**:

![Árbol celular ACel1](img/arbol_celular.png)

Al respecto, escriba las siguientes funciones:

+ Escriba la función ```esCelular(A)```, que recibe un árbol binario, y entrega ```True``` si es que corresponde a un árbol celular (y ```False``` en cualquier otro caso).

  Ejemplo:

  - ```esCelular(ACel1)``` entrega ```True```.

+ Se define el **decaimiento celular** para cada valor de un árbol celular, como la diferencia entre el valor de un nodo y la suma de los valores de sus hijos izquierdo y derecho. Por ejemplo:

  - El decaimiento del nodo de valor `100` es `1`, pues `(100 - (47 + 52))` es `1`.
  - El decaimiento del nodo de valor `47` es `11`, pues `(47 - (18 + 18))` es `11`.
  - El decaimiento del nodo de valor `52` es `13`, pues `(52 - 39)` es `13`.
  - El decaimiento de los nodos hoja (`18`, `18` y `39`) es `0`.

  Escriba la función ```decaimiento(A)```, que recibe un árbol binario celular, y calcula el decaimiento total del árbol (es decir, la suma del decaimiento de todos sus nodos).

  Por ejemplo:

  - ```decaimiento(A)``` entrega ```25```.