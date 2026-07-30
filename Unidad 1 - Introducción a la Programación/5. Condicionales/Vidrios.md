---
tags: [Condicionales]
---

# Vidrios

Los vidrios de 851 se caen! Por esto la facultad contrató a un equipo de investigación que pueda identificar la causa del desprendimiento de los vidrios. Tu eres parte de ese equipo, y tu jefe te pide que programes la siguiente función que nos ayudará a modelar la caída de los vidrios:

La función ```destino_estudiante(posicion_estudiante, posicion_vidrio)``` simula la caída de un vidrio y entrega un veredicto que depende de la posición del estudiante en relación al vidrio:
Tanto la posición del vidrio como la del estudiante son enteros entre el 1 y el 10 (inclusive).

- Si el estudiante se encontraba a 3 metros o mas del vidrio el veredicto es «Salvado»
- Si el estudiante se encontraba a 1 o 2 metros de distancia del vidrio el veredicto es «Herido»
- Finalmente si el estudiante se encontraba en la misma posición que el vidrio el veredicto es «GG»
  
**Recuerde usar la receta de diseño.**

```python
>>> destino_estudiante(10, 8)
Herido
>>> destino_estudiante(5, 1)
Salvado
>>> destino_estudiante(6, 6)
GG
```