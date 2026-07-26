---
tags: [Condicionales, Función Interactiva]
---

# Sr Pera (Variante 2)

Un muy amigo suyo de la “Universidad del Colo-Colo” esta aproblemado con el
curso “*Cálculos Modernos*”, ya que no le ha ido muy bien. Este curso consta de 3
controles y un examen, y su amigo ya ha dado los dos primeros controles.

Como usted es una persona humilde y de buen corazón, decide prestarle ayuda para
calmar su pera. Para esto utilizará sus magnificas habilidades en Python para realizar
tan magna tarea. Procederemos como sigue:

**a)** Cree la función `notaPara4(c1,c2)` , que reciba las   notas de los dos primeros
controles de su amigo y entregue cuanto necesita en su próximo control para
llegar con 4, 0 al examen.

**b)** Su amigo le agradece la ayuda pero lamentablemente no le fue como esperaba
y sus niveles de pera han aumentado significativamente, llegando a niveles por
sobre los 9000 [🍐 / 👨‍🎓]. Para disminuir los niveles de pera de su amigo se decide
hacer la función `notaParaExamen(c1,c2,c3)` que recibe las notas de control
de este triste y peron alumno y retorne la nota que necesita para pasar en el
examen.

**Indicación:** Su amigo le dice que la nota final del curso esta dada por:

$$NF = 0.6 \cdot NC + 0.4 \cdot EX $$
$$ NC >= 4.0$$

Donde $NC$ es el promedio entre los tres controles y $EX$ es la nota del examen.

**c)** Anticipándose a la pera que tendrá su amigo, decide crear una función llamada
`notaParaSegunda(c1,c2,c3)` , que recibe las notas de control, y entrega la
nota que necesita para llegar al examen de segunda. Para llegar al examen de
segunda, se tiene que cumplir que: $0.6 \cdot NC + 0.4 \cdot Ex \geq 3,7$

**d)** Finalmente, para facilitarle el uso de estas funciones, decide crear una función interactiva llamada `peramatico()` , que pregunta por las 3 notas de controles, y muestra en pantalla la nota que necesita para pasar en el examen, y la nota que necesita para llegar al examen de segunda, siguiendo el siguiente dialogo:

```python
>> peramatico()
Nota C1? 5.0
Nota C2? 3.0
Nota C3? 2.0
Necesitas un 5.0 para pasarlo de una
Necesitas un 4.3 para llegar al de segunda
```





