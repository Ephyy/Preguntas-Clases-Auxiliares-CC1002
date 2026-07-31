---
tags: [Control, Diccionarios, Listas Indexadas]
dificultad: Muy díficil
---

# Paraderos de Buses 🚌🚏

El recorrido de un bus interurbano se guarda en un diccionario, donde la llave indica el código del recorrido (un número entero) y el valor es una lista de Python de Strings con el lugar de inicio del recorrido y todos los paraderos del bus, desde el primer paradero al último paradero:

```python
D = {101:['Santiago','Curico','Talca','Chillan'],
     102:['Chillan','Talca','Curico','Santiago'],
     150:['Santiago','Rancagua','Curico','San Rafael','Talca','Parral', 'Chillan'],
     212:['Valparaiso', 'Los Vilos', 'Coquimbo'],
     315:['Puerto Montt', 'Ancud', 'Castro', 'Quellon']}
```

Por ejemplo, el recorrido 101 parte en Santiago y termina en Chillán, con paradas en Curicó, Talca y Chillán.

+ **(3.0 p)** Escriba la función ```siguienteParadero(D, codigo, paradero)```, que reciba el diccionario `D` de recorridos, un código de un recorrido y el nombre de un paradero, y devuelva el nombre del siguiente paradero. En caso de que se ingrese el nombre del último paradero, o de un paradero que no existe en el recorrido, o de un recorrido que no exista, la función debe devolver el String vacío (''). Por ejemplo:

  - ```siguienteParadero(D, 101, 'Curico')``` devuelve ```'Talca'```.
  - ```siguienteParadero(D, 150, 'Curico')``` devuelve ```'San Rafael'```.
  - ```siguienteParadero(D, 315, 'Quellon')``` devuelve el String vacío (```'Quellon'``` es el último paradero del recorrido 315).
  - ```siguienteParadero(D, 212, 'Calera')``` devuelve el String vacío (no existe el paradero ```'Calera'``` en el recorrido 212).
  - ```siguienteParadero(D, 500, 'Santiago')``` devuelve el String vacío (no existe el recorrido 500).

+ **(3.0 p)** Escriba la función ```menosParadas(D, origen, destino)```, que reciba el diccionario `D` de recorridos, un paradero de origen y un paradero de destino distintos, y devuelva la menor cantidad de paradas entre origen y destino entre los recorridos almacenados en `D`. Si no hay ningún recorrido que lleve de origen a destino, la función debe devolver -1. Por ejemplo:

  - ```menosParadas(D, 'Curico', 'Talca')``` devuelve ```1```, porque en el recorrido 101 para ir de Curicó a Talca hay una sola parada (Talca), en cambio en el recorrido 150 hay dos paradas (San Rafael y Talca).
  - ```menosParadas(D, 'Quellon', 'Ancud')``` devuelve ```-1```, porque no hay ningún recorrido en D que inicie en Quellón y llegue a Ancud.