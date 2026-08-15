---
tags: [Condicionales, Módulos, Funciones]
---

# Panamericanos [C1 2019-2]

1.  Escriba una función con el encabezamiento ```def ganador(x1,y1,z1,x2,y2,z2)``` que entregue un 1 si la primera terna (con los números enteros x1, y1 y z1) le gana a la segunda terna (con los números enteros x2, y2, z2), que entregue un 2 si la segunda terna le gana a la primera, o entregue un 0 si las dos ternas son iguales.

    Notas:
    - La terna (5,4,13) le gana a la las siguientes ternas: a la terna (2,6,25) puesto que 5 >2; a la terna (5,2,21) puesto que 4>2 y los primeros números son iguales; y a la terna (5,4,1) puesto que 13>1 y los dos primeros números son iguales.
    - Debe escribir la receta de diseño incluyendo al menos 3 pruebas (una por cada resultado posible)

2. El módulo grabado en el archivo `panamericanos.py` permite consultar los resultados de los últimos juegos panamericanos a través de las siguientes funciones:
   
    | Contrato             | Ejemplo de uso    | Resultado | Explicación                                           |
    | -------------------- | ----------------- | --------- | ----------------------------------------------------- |
    | `pais: int -> str`   | `pais(21)`        | `"Chile"` | Nombre del país cuyo n.º se indica en el argumento.   |
    | `oro: str -> int`    | `oro("Chile")`    | `13`      | Cantidad de medallas de oro obtenidas por el país.    |
    | `plata: str -> int`  | `plata("Chile")`  | `19`      | Cantidad de medallas de plata obtenidas por el país.  |
    | `bronce: str -> int` | `bronce("Chile")` | `18`      | Cantidad de medallas de bronce obtenidas por el país. |


    Escriba la función recursiva `posicionChile` (sin receta de diseño) que use el módulo anterior para calcular y entregar el lugar o posición que ocupó Chile en el medallero final de los juegos.