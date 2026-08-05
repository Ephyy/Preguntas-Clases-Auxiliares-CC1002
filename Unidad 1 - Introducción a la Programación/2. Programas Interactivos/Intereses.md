---
tags: [Funciones, Programa Interactivo, Función Interactiva]
---

# Intereses

Sofía se encuentra en un problema existencial al frente de un banco, debido a que no sabe
cómo invertir su dinero. Un ejecutivo al verla tan angustiada, le ofrece dos formas de invertir su dinero: Usando *Interés simple* o *Interés compuesto*.

- **Interés Simple:** Se calcula de la siguiente forma: $C_{f} = C_{i}(1 + t \cdot i)$ en donde Ci es
el capital o monto inicial, i es el interés en forma decimal, y t los periodos de tiempo.
En este interés se calcula sólo en base al capital inicial, sin considerar las ganancias
intermedias.
- **Interés Compuesto:** Se calcula de la siguiente forma: $C_{f} = C_{i}(1 + i)^{t}$
en donde los parámetros son los mismos a la fórmula anterior. Este interés si considera las ganancias intermedias generadas por la tasa

Cuando Sofía supo que debía calcular, se angustió aún más, por lo que desesperadamente le pide ayuda a usted, para saber cuál de las dos opciones es mejor.

Para ayudar a Sofía se le pide:

**a)** Escriba una función `interesSimple` que calcule el interés simple, acorde a los parámetros mencionados anteriormente.

**b)** Escriba una función `interesCompuesto` que calcule el interés compuesto, acorde a los parámetros mencionados anteriormente.

**c)** Usando las funciones anteriores, cree una función interactiva `inversion()` que pida al usuario el monto inicial, la tasa de interés anual, y el tiempo en años, e imprima en pantalla el monto ganado tanto por interés simple, como por interés compuesto. Con ello Sofía podrá ver qué le conviene más y será feliz.

```python
>> inversion()
Ingrese monto inicial: ...
Ingrese interes: ...
Ingrese periodo: ...
El monto ganado usando interes simple es de: ___ pesos
El monto ganado usando interes compuesto es de: ___ pesos
```





