---
tags: [Control, Módulos, Programa Interactivo]
dificultad: Media
---

# Fintech 🏦💰

El módulo `fintech` contiene las siguientes funciones:

```python
# valorCAE: int -> float
# retorna el valor CAE (en porcentaje y con 2 decimales) para un número de días futuros a contar de hoy
# Ejemplo: valorCAE(0) retorna 33.54 #CAE de hoy
# Ejemplo: valorCAE(3) retorna 32.74 #CAE de 3 días más

# valorCuota: num, int, int -> num
# devuelve el valor de la cuota mensual de un crédito para un monto (en pesos plazo (en meses) y día en que se contrata el crédito (0 en adelante).
# Ejemplo: valorCuota(5000000, 36,0) retorna 222064 que corresponde al valor a pagar por un crédito de 5 millones en 36 cuotas cursado el día de hoy (0).

# interes: num, float -> num
# calcula el interés (en pesos) sobre un monto (en pesos) depositado a una cierta tasa de interés
# Ejemplo: interes(1000, 0.02) retorna 20 porque si se depositasen $1000 con una tasa de interés anual del 2%, se ganaría $20 ($1,000 x 0.02) de interés el primer año

# totalCredito: int, num -> num
# retorna el costo total de un crédito en un plazo (en meses) con un determinado valor de cuota (en pesos)
# Ejemplo: totalCredito(36, 222064) retorna 7994304 correspondientes a un crédito pactado a 36 meses con una cuota de 222064
```

Usando las funciones que necesite del módulo `fintech` , escriba un programa en Python que establezca un diálogo de consultas y sugerencias similar al mostrado en el ejemplo. Notar que el programa debe indicar cuando conviene cursar el crédito (entre hoy o mañana) dependiendo cuando sea más barato el crédito:

```text
Monto que solicita?: _5000000_
Plazo del crédito en meses?: _36_

Si el crédito lo cursa hoy:
El CAE de su crédito : 33.54
Pagará 36 cuotas de: $ 222064
Costo total del crédito: $ 7994304

Si el crédito lo toma mañana:
El CAE de su crédito: 32.74
Pagará 36 cuotas de: $ 202064
Costo total del crédito: $ 7274304

Le conviene tomar el crédito mañana, ya que ahorrará $ 720.000.
```

**Indicación:** están subrayados ( _ ) los datos que ingresa el usuario y puede suponer que los datos ingresados son siempre
correctos por lo que no debe validarlos.