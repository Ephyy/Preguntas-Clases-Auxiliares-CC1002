---
tags: [Control]
---

# **[C1 2017-1]** Datos del Censo 

Para el censo, los datos de una persona se codificarán en un entero de 9 dígitos, en la siguiente forma:

| Dígitos        | Dato             | Valor permitido            | Ejemplo |
|----------------|------------------|----------------------------|---------|
| 1°             | Sexo             | 1 (hombre) o 2 (mujer)     | 2       |
| 2°, 3° y 4°    | Edad (en años)   | Entero ≥ 0                 | 035     |
| 5° y 6°        | Nº de hijos      | Entero ≥ 0                 | 03      |
| 7°             | Estado civil     | 1 (soltero) o 2 (casado)   | 2       |
| 8° y 9°        | Nacionalidad     | Entero ≥ 0 (ej. 00=chilena)| 00      |

Al respecto, cree la función `obtenerDato(valor, dato)`, que reciba un número entero (que contiene los datos de una persona) y un string (que puede ser: "sexo", "edad", "hijos", "estado civil" o "pais"), y entregue un número entero con el valor indicado.

Por ejemplo:
- `obtenerDato(203503200,"edad")` entrega 35
- `obtenerDato(203503200,"estado civil")` entrega 2

**Notas:**
- Haga un test para cada caso posible de dato.
- En caso de que el string entregado en dato sea distinto a los indicados, entonces la función devuelve un -1
