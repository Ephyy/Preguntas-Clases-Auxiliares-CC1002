---
tags: [Condicionales]
---

# Cálculo de Salario 🤑

Una empresa de venta de figuritas necesita hacer un programa que automatice el cálculo de los sueldos de sus trabajadores del área de ventas.

En esta pregunta calcularemos el salario líquido de un trabajador aplicando los descuentos legales y bonificaciones de la empresa sobre el sueldo bruto.

Considere que esta empresa calcula los sueldos de sus trabajadores siguiendo las reglas a continuación:

+ Primero se aplican los descuentos legales. Para ello debe hacer un descuento equivalente al 10% para destinarlo a AFP, y también un descuento del 7% para destinarlo a su plan de salud. Ambos descuentos se calculan sobre el sueldo bruto.

+ Al sueldo con los descuentos aplicados se le añade una bonificación por la cantidad de horas extras trabajadas. En caso de trabajar entre 0 y 5 horas extras, la bonificación es de 20.000 por hora. En caso de haber trabajado 10 horas extras o más, la bonificación es de 40.000 por hora extra.

+ En caso de que la persona haga teletrabajo, se suma 20.000 al sueldo para costear la electricidad utilizada.

+ En caso de que la persona **no** haga teletrabajo, se le suman 30.000 para movilización y transporte.

+ Si el trabajador hace 10 ventas o menos, no obtiene ninguna bonificación. Si el trabajador hace entre 10 y 29 ventas, entonces se le da una bonificación de 20.000. Si realiza entre 30 y 39 ventas, se da una bonificación de 40.000. Y si realiza 40 ventas o más, se da una bonificación de 70.000.

+ El trabajador obtiene un descuento de 15.000 por hora de atraso durante el mes.

Cree una función llamada ```cálculoSueldoLiquido(sueldo_bruto, horas_extras, teletrabajo, cantidad_de_ventas, atrasos)```.

Esta función recibe:

- el sueldo bruto en CLP.
- la cantidad de horas extras realizadas por el trabajador durante el mes (considere que solo pueden ser enteros).
- la variable `teletrabajo`, que corresponde a un booleano indicando si es que la persona teletrabaja o no.
- la cantidad de ventas que hace el trabajador.
- la cantidad de horas de atraso del trabajo acumuladas durante el mes (considere que solo pueden ser enteros).

La función debe utilizar los argumentos de entrada para calcular y entregar correctamente el sueldo final para cualquiera de sus trabajadores.

Recuerde seguir los pasos de la receta de diseño.