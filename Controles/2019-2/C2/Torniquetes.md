---
titulo: Torniquetes 851
tags: [Control, Listas Recursivas, Estructura]
---

# Torniquetes 851 (P1 C2 2019-02)

Los torniquetes de entrada a la facultad manejan una lista que mantiene el RUT de las personas que ingresan y la cantidad de veces que han ingresado durante el día:

```python
# Persona: rut(str) ingresos(int)
estructura.crear("persona", "rut ingresos")

# Ejemplos de personas
p1 = persona("123-k", 1)
p2 = persona("234-0", 2)

# Lista de personas
LP = lista(p1, lista(p2, listaVacia))
```

Use las funciones del módulo `lista` (y eventualmente otras que haya visto en clases), para escribir las siguientes funciones:

- **(4.0p)** La función `ingresar(rut, Lpers)`, que recibe un RUT y una lista de personas, y registra el ingreso de una persona.

  - Si la persona ya existía en la lista, entonces se debe incrementar su cantidad de ingresos.
  - Si la persona no existe en la lista, entonces se debe agregar al final.

  Ejemplos:

  ```python
  ingresar("234-0", LP)
  # entrega:
  lista(persona("123-k", 1),
        lista(persona("234-0", 3),
              listaVacia))
  ```

  ```python
  ingresar("345-7", LP)
  # entrega:
  lista(persona("123-k", 1),
        lista(persona("234-0", 2),
              lista(persona("345-7", 1),
                    listaVacia)))
  ```

- **(2.0p)** La función `masIngresos(L)`, que recibe una lista de personas, y entrega la persona con más ingresos.

  Por ejemplo:

  - `masIngresos(LP)` entrega `persona("234-0", 2)`.

  **Nota:** Puede suponer que solo hay una persona que registra la mayor cantidad de ingresos.