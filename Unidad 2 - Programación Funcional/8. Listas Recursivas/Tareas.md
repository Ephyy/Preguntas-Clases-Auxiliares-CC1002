---
tags: [Listas Recursivas]
---

# Lista de Tareas 📝

Una persona muy organizada quiere estructurar las distintas tareas cotidianas (y no tanto) que tiene que hacer, con ayuda de una lista de tareas. Esto se puede representar con la siguiente estructura:

```python
# Tarea: descripcion(str) completada(bool) fechalimite(int)
estructura.crear("Tarea", "descripcion completada fechalimite")

# Tareas de ejemplo
T1 = Tarea("pasear al doggo", False, 20240926)
T2 = Tarea("estudiar para el control de álgebra", False, 20240925)
T3 = Tarea("comprar almuerzo", True, 20240923)
T4 = Tarea("Entregar la tarea de biología", False, 20240530)
T5 = Tarea("Hacer un meme", True, 20241001)

# Lista de tareas de ejemplo
Ltareas = lista(T1, lista(T2, lista(T3, lista(T4, lista(T5, listaVacia)))))
```

Con lo anterior:

- Una `Tarea` se representa como un texto con una descripción, una indicación de si se completó o no, y la fecha límite para completarla (en formato año-mes-día `AAAAMMDD`).
- Una lista de tareas representa todas las tareas que anoté, sin importar si ya fueron completadas o no.

Usando estas estructuras, programe las siguientes funciones:

+ Cree la función ```mostrarTareas(L)```, que recibe una lista de `Tarea`, y muestra en pantalla todas las tareas, línea por línea, de acuerdo al formato del siguiente ejemplo:

  ```python
  >>> mostrarTareas(Ltareas)
  pasear al doggo - no completada - 20240926
  estudiar para el control de álgebra - no completada - 20240925
  comprar almuerzo - completada - 20240923
  Entregar la tarea de biología - no completada - 20240530
  Hacer un meme - completada - 20241001
  ```

+ Cree la función ```pendientes(L)```, que recibe una lista de `Tarea` y entrega una lista de las `Tarea` que se encuentren pendientes (no completadas).

  Ejemplo:

  - ```pendientes(Ltareas)``` entrega:

    ```python
    lista(T1, lista(T2, lista(T4, listaVacia)))
    ```

+ Cree la función ```urgente(L, fechahoy)```, que recibe una lista de `Tarea` no completadas, y la fecha de hoy (en formato `AAAAMMDD`), y entrega la tarea que es más urgente de completar (la que hay que completar pronto, dado que se acerca su fecha límite para completarla). En caso de que exista más de una `Tarea` urgente en la lista, entonces solo entregue la primera que encontró.

  Ejemplo:

  - Suponiendo que tenemos en la variable `Lpend` la lista de tareas pendientes entregada por la función anterior:

    ```python
    urgente(Lpend, 20240924)
    # Tarea("estudiar para el control de álgebra", False, 20240925)
    ```