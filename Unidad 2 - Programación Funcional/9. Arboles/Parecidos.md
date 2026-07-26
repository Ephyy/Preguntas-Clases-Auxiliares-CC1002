---
tags: [Árboles Binarios]
---

#  Arboles parecidos

Dos árboles binarios se dice que son _parecidos_, si es que tienen el mismo contenido, aunque no necesariamente en el mismo orden. Por simplicidad asumiremos que en un mismo árbol no puede haber elementos repetidos.

![arboles magnéticos](./img/arbol_simil.png)

Por ejemplo, el árbol `AP1` es similar con ` AP2`, pues tienen el mismo contenido, pero no es similar con ` AP3`, pues, a pesar de que tienen la misma forma, su contenido es distinto. Al respecto, programe lo siguiente:

**a)** Cree la función `contieneTodos(A1, A2)`, que recibe dos árboles binarios, y entrega `True` si es que todos los elementos del árbol `A1` se encuentran presentes en `A2`. Por ejemplo:

  - `contieneTodos(A1, A2)` entrega `True`
  - `contieneTodos(A1, A3)` entrega `False`

  Hint: Recuerde que existe la función `buscar(A,e)` de árboles binarios.

**b)** Cree la función `parecidos(A1, A2)`, que recibe dos árboles binarios, y entrega `True` si es que tales arboles cumplen con ser parecidos. Por ejemplo:

  - ` parecidos(A1, A2)` entrega `True`
  - ` parecidos(A1, A3)` entrega `False`