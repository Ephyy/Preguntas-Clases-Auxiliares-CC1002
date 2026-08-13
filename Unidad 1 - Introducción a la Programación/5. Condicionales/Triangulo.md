---
tags: [Condicionales, Módulos, Funciones, Programa Interactivo]
---

# Jugando con Triangulitos 📐

Suponga que existe un módulo llamado `triangulos.py` que ya contiene las siguientes funciones:

| Función | Ejemplo de uso | Descripción |
| --- | --- | --- |
| ```es_triangulo(a, b, c)``` | ```es_triangulo(3, 4, 5)``` entrega ```True``` | Verifica si los lados pueden formar un triángulo. Retorna ```True``` o ```False```. |
| ```clasificacion(a, b, c)``` | ```clasificacion(3, 3, 3)``` entrega ```'equilátero'``` | Retorna un string de acuerdo al tipo de triángulo que conforman los lados ```a```, ```b``` y ```c```: ```'equilátero'```, ```'isósceles'``` o ```'escaleno'```. Si los lados no conforman un triángulo, retorna ```'inválido'```. |
| ```es_rectangulo(a, b, c)``` | ```es_rectangulo(3, 4, 5)``` entrega ```True``` | Retorna ```True``` si el triángulo es rectángulo, es decir, cumple con el teorema de Pitágoras, o ```False``` si no. |

+ Implemente la función ```clasificacion(a, b, c)``` del módulo `triangulos.py` con su receta de diseño completa.

+ Use el módulo `triangulos.py` en el archivo `programa.py`, para implementar un programa interactivo que reproduzca el siguiente diálogo:

  `````````python
  >>> Ingrese lado a: 3
  >>> Ingrese lado b: 4
  >>> Ingrese lado c: 5

  forman triángulo?: si
  tipo de triángulo?: escaleno
  es rectángulo?: si
  `````````

  En caso que el usuario ingrese lados que no forman un triángulo, el programa debe mostrar el siguiente mensaje:

  `````````python
  >>> Ingrese lado a: 1
  >>> Ingrese lado b: 2
  >>> Ingrese lado c: 10

  forman triángulo?: no
  `````````