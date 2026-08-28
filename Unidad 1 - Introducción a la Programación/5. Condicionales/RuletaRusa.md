---
tags: [Condicionales, Funciones]
dificultad: Fácil
---

# Ruleta Rusa 🔫

Después de un agotador control de Introducción a la Programación, un grupo de estudiantes de la FCFM decide relajarse con una (afortunadamente inofensiva) partida de ruleta rusa... el revólver está cargado con una bala falsa, así que quien pierde solo se lleva un buen susto.

El revólver tiene 6 posiciones numeradas del 1 al 6, dispuestas en círculo, por lo que la posición siguiente a la 6 es nuevamente la 1. La bala está escondida en una de ellas, y al apretar el gatillo se acciona una posición determinada. 

Programe la función ```disparar(posicion_bala, posicion_actual)```, donde ```posicion_bala``` es el número de la posición en la que se encuentra la bala y ```posicion_actual``` es el número de la posición que se va a accionar. La función simula el disparo y entrega un veredicto según la posición de la bala respecto a la posición accionada:

- Si la bala se encuentra en la posición que se acciona, el veredicto es ```"BANG"```.
- Si la bala se encuentra en la posición inmediatamente siguiente a la accionada (es decir, el jugador se salvó por poco), el veredicto es ```"Por poco..."```.
- En cualquier otro caso, suena un ```"click"``` y el jugador sobrevive.

Tanto ```posicion_bala``` como ```posicion_actual``` son enteros entre 1 y 6 (inclusive). 

```python
>>> disparar(3, 3)
'BANG'
>>> disparar(4, 3)
'Por poco...'
>>> disparar(1, 5)
'click'
>>> disparar(1, 6)
'Por poco...'
```

- Recuerde realizar la receta de diseño.