---
tags: [Módulos, Funciones, Programa Interactivo]
---

# Metal Latas 🥫

Nintendalas Corp. es una empresa de envases metálicos para bebidas, famosa por sus iconicos diseños apodados como "Metal Latas".

Cada día recibe decenas de propuestas de cilindros con distintas alturas y radios. Para evaluar la viabilidad de cada diseño, la empresa necesita calcular el costo de producción de cada lata tomando en cuenta:


- El volumen del líquido que contendrá.

- El área total de su superficie (para etiquetado y tapas).

Con lo que se tiene la  siguiente función de costo:
  
  $$ Costo(area, volumen) = 3.2*volumen + \sqrt{area^3} + 754 $$

La empresa busca automatizar el proceso de evaluación de las latas y necesita de su ayuda al enterarse de sus habilidades para resolver problemas en el curso de Introducción a la Programación. 


Para ello se tiene el módulo `cilindro`, el cual contiene las siguientes funciones:

| Función                  | Descripción                        | Ejemplo                           |
| ------------------------ | ---------------------------------- | --------------------------------- |
| `area(radio, altura)`    | Calcula el área de un cilindro.    | `area(5, 10)` entrega `471.24`    |
| `volumen(radio, altura)` | Calcula el volumen de un cilindro. | `volumen(5, 10)` entrega `785.40` |


1.  Utilizando el modulo `cilindro`, escriba en otro archivo una *función* ```costoLata(h, r)``` que calcule el costo de realizar una lata de altura $h$ y radio $r$. Esta función recibe como parámetros los valores de $h$ y $r$, ademas debe retornar el costo redondeado a 2 decimales.

    Ejemplo:
    - ```costoLata(10, 2)``` entrega ```3007.95```
      
    **Indicación:** Para redondear un valor puede utilizar la función ```round(n, c)```, la cual redondea un número *`n`* con una cantidad *`c`* de decimales.


2. Cree un *programa interactivo* que consulte al usuario el valor del radio y altura de un cilindro y muestre en pantalla el costo de crear una lata de esas características. Considere el siguiente dialogo como ejemplo:

    ```python
    Bienvenido al programa que calcula el costo de producir una lata
    Ingrese radio: ___
    Ingrese altura: ___
    El costo de producir una lata de estas características es de ___ pesos
    ```