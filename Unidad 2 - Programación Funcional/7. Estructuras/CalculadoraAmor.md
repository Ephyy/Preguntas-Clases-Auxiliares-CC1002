---
tags: [Estructuras]
---

# Calculadora del amor

En este ejercicio, queremos ver qué tan compatibles son dos personas usando un poco de código.

1. Defina una estructura de datos inmutable llamada `Persona`. La estructura debe tener los siguientes campos:
   - `nombre`: una cadena de caracteres que representa el nombre de la persona.
   - `fecha`: un entero en formato `AAAAMMDD` que representa la fecha de nacimiento.
   - `color`: una cadena de caracteres que representa el color favorito de la persona.

2. Defina una función validadora ```esPersona(P)``` que valida si el parámetro `P` corresponde a una estructura `Persona` válida o no.

3. Defina una función llamada ```calcular_afinidad(persona1, persona2)``` que:
   - Reciba dos `Persona` como parámetros.
   - Calcule el índice de afinidad entre ellas usando las siguientes reglas:
     - Si el `color` es el mismo, sume 20 puntos.
     - Si el día de la fecha de cumpleaños es igual al mes de la otra persona, sume 30 y, en caso contrario, reste 10.
     - Si la diferencia de años en `fecha` es de 5 años o menos, sume 30 puntos. Si es entre 6 y 10 años, sume 10 puntos. Si es mayor a 10 años, no sume puntos.