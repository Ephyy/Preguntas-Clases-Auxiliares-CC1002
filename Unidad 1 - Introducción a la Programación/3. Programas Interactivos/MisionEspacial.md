---
tags: [Funciones, Programa Interactivo]
---

# Misión Espacial 🚀

Eres el capitán de la nave Endurance, encargada de un viaje interestelar hacia un planeta recién descubierto. Antes de despegar, necesitas calcular 2 datos clave para planificar la misión:

- Combustible necesario: depende de la distancia al planeta y del peso de la nave.
- Costo de la misión: depende del combustible necesario y del precio por litro.

El sistema de la nave trabaja con unidades espaciales en lugar de kilómetros. Por eso, en todos los cálculos es necesario convertir la distancia en km a unidades espaciales mediante la fórmula secreta de la Federación Espacial.

Tu misión como programador es:

+ Escribir una función que convierta kilómetros a unidades espaciales. Esta función se llamará `convertir_a_unidades_espaciales`, y debe recibir la distancia en km y entregar la distancia en unidades espaciales. Para hacer la conversión tenga en cuenta las siguientes consideraciones:

  - 500 km corresponden a 1 unidad espacial.
  - La ruta nunca es perfectamente recta; las naves deben hacer maniobras para evitar asteroides, seguir órbitas o aprovechar impulsos gravitatorios, y eso aumenta la distancia real recorrida en un 10%.

  Entonces, al valor resultante de hacer la conversión del punto anterior súmele el 10%.

+ Escribir una función que calcule el combustible utilizado llamada `calcular_combustible`. Esta recibirá los argumentos `distancia_km` y `peso_nave`. Para hacer el cálculo considere que se gastan 50 litros por unidad espacial y por tonelada de nave.

+ Escribir una función llamada `calcular_costo_mision` que calcule el costo total de la misión. Considere que el costo total corresponde a lo que se gasta en combustible. La función debe recibir como argumentos la distancia en km, el peso en toneladas y el precio del combustible por litro.

**Hint:** Utilice funciones dentro de funciones.