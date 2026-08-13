---
tags: [Condicionales, Módulos, Funciones, Programa Interactivo]
titulo: Sr Pera 🍐 (Variante 1)
---

# Sr Pera 🍐 (Variante 1)

El Sr. Pera, anticipándose al fin de semestre, desea hacer un programa en Python que le permita calcular la mínima nota que necesita en el examen para pasar directamente, o en su defecto, irse al examen de segunda. Para esto, consideraremos los siguientes criterios:
- Solo consideraremos el caso con 3 controles, y las notas se redondean al primer decimal.
- La eximición es con promedio de notas mayor o igual a 5.5 en los 3 controles.
- La nota final se calcula como 60% Promedio de controles + 40% Nota del examen.
- Se aprueba el curso, si la nota final, luego de rendido el examen, es mayor o igual a 4.0
- Se va a examen de segunda, si la nota final luego de rendido el examen, esta entre 3.7 y 3.9.

Con esto, para lograr ayudar al Sr. Pera, se le sugiere partir creando un modulo llamado calculoNotas, que contenga las siguientes funciones:

**a)** Una función llamada `eximido`, que recibe 3 notas de control, y entrega como resultado True, si con esas notas se exime, y False si no. 

**b)** Una función llamada `notaExamen`, que recibe el promedio de notas de control, y entrega como resultado, la nota mínima que se necesita en el examen, para pasar el curso.

**c)** Una función llamada `notaSegunda`, que recibe el promedio de notas de control, y entrega como resultado, la nota mínima necesaria en el examen, que permite rendir el examen de segunda.

Finalmente, con ayuda de este modulo, se quiere crear un programa interactivo en otro archivo, que pregunte al Sr.Pera por las 3 notas de control, e indique las notas que necesita para pasar el curso en el examen, o llegar al examen de segunda. En caso de que con las notas recibidas:
- Se encuentre eximido
- Necesite mas de un 7.0 para pasar en el examen
- Necesite mas de un 7.0 para llegar al examen de segunda
  
Debe mostrar en pantalla un mensaje acorde a cada caso. Puede tomar como ejemplo el siguiente dialogo interactivo:

```python
 Nota C1? 4.5 
 Nota C2? 5.5
 Nota C3? 2.6
 Necesitas un 3.7 para pasar el curso
 Necesitas un 3.0 para llegar al examen de segunda.
```