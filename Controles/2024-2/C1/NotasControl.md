---
tags: [Control, Condicionales, Programa Interactivo]
---

# Notas Control

Al inicio de un curso, el Equipo Docente informa cuántos controles se realizará: 1, 2 o 3 controles; además del examen.
Dependiendo del número de controles, la Nota Final se calcula según se indica en la tabla.


| Nº de Controles | Cálculo de Nota Final                                | Condición para reemplazar nota de examen por promedio de controles |
|-----------------|-------------------------------------------------------|----------------------------------------------------------------------|
| 1               | 50% promedio controles y 50% nota examen              | No aplica                                                           |
| 2               | 50% promedio controles y 50% nota examen              | Con promedio controles ≥ 5.5                                        |
| 3               | 60% promedio controles y 40% nota examen              | Con promedio controles ≥ 5.5                                        |


La condición establece que si un/a estudiante obtiene un promedio de controles $\geq$ 5.5 y la nota del examen es menor
que 5.5, entonces la nota del examen se reemplaza por el promedio de los controles.

La Nota Final debe ser mayor o igual a 4.0 para aprobar el curso. Si la nota final es menor que 4.0 pero mayor o igual a
3.7, se puede optar a una evaluación adicional. Si la Nota Final es menor a 3.7, se reprueba el curso.

Escriba un programa que pregunte por la cantidad de controles, las notas de controles y examen, y luego escriba la nota final y la situación final estableciendo un diálogo como el que se muestra en los siguientes dos ejemplos:

```python
Cantidad de controles (1 - 3)? 2        Cantidad de controles (1 - 3)? 3
Nota control 1? 3.7                     Nota control 1? 7
Nota control 2? 3.9                     Nota control 2? 6
Nota examen? 3.8                        Nota control 3? 6.5
Nota final: 3.8                         Nota examen? 4
Situacion: Evaluacion adicional         Nota final: 6.5
                                        Situacion: Aprueba
```

Indicaciones:
- Suponga que se ingresarán datos correctos (número de controles entre 1 y 3, notas entre 1.0 y 7.0), y que el/la
estudiante rindió todos los controles y el examen.
- La situación final debe ser ‘Aprueba’, ’Reprueba’, o ‘Evaluacion adicional’.
- Considere que la función predefinida `round(x,n)` redondea el valor x a n decimales. Por ejemplo,
`round(2/3,2)` devuelve 0.67, `round(3.956,2)` devuelve 3.96 y `round(3.954,2)` devuelve 3.95. Sólo debe redondear el cálculo final de la Nota Final.

