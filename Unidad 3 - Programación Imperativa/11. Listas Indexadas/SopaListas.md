---
tags: [Listas Indexadas]
---

# Sopa de Listas 📋

A continuación, tenemos varios ejercicios misceláneos, donde hay que utilizar conocimientos de listas y ciclos para resolverlos.

- Cree una función llamada `comunes(L1, L2)`, que recibe dos listas que contienen números y `string` en ningún orden en particular, y entrega una lista con los elementos en común entre ambas listas.

  Ejemplo:

  ```python
  LA = [23, 42, "hola", "manzana", 8]
  LB = ["hola", 22, 24, 48, 23]

  comunes(LA, LB)
  # [23, "hola"]
  ```

  No es necesario que los elementos en la lista final queden en un orden en particular.

- Cree una función llamada `palindroma(L)`, que recibe una lista de elementos cualquiera, e indica si la lista cumple con ser palíndroma o no.

  Se dice que una lista es palíndroma si se ve igual al revés y al derecho.

  Ejemplo:

  ```python
  LA = [23, 42, "hola", 42, 23]
  LB = ["hola", 22, 24, 48, 23]

  palindroma(LA)
  # True

  palindroma(LB)
  # False
  ```

- Cree una función interactiva llamada `notas()`, que le pregunta a una persona por una cantidad indeterminada de notas entre `1.0` y `7.0`, hasta que se ingrese la palabra `fin`.

  Cuando ocurra eso, la función muestra en pantalla el promedio, mayor y menor nota ingresadas.

  Ejemplo:

  ```text
  >>> notas()

  ingrese nota: 4.0
  ingrese nota: 5.0
  ingrese nota: 6.0
  ingrese nota: fin

  minimo = 4.0
  maximo = 6.0
  promedio = 5.0
  ```

  En principio puede asumir que las notas se ingresarán en el rango `1.0`–`7.0`, pero luego piense cómo modificar su solución para que el programa siga funcionando si es que le ingresan una nota fuera de rango, o un `string` distinto de `fin`.