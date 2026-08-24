---
tags: [Control, Listas Recursivas, Estructuras]
---

# Estructura Triángulo [C2 2015-2]

Un triángulo de lados enteros se puede representar a través de una estructura que contenga sus 3 lados:

```python
# triangulo: a(int) b(int) c(int)
estructura.crear('triangulo','a b c')
```

Con todo lo anterior, es hora de ejercitar con triángulos, realizando las siguientes funciones:

1. ```perimetro(T)```: Dado un triangulo, entrega su perímetro.
2. ```tipoTriangulo(T)```: Dependiendo de las características del triangulo, entrega:
  
     - 3 si es equilátero (3 lados iguales).
     - 2 si es isósceles (2 lados iguales).
     - 1 si es escaleno (3 lados distintos).
     - cero si no es un triángulo.
     
     Nota: 3 números enteros positivos forman un triángulo si todas las sumas de dos de ellos es mayor que el tercero.

3. ```triangulosIso(listaT)```: Recibe una lista de triángulos y entrega una lista con los triángulos de la lista que sean isósceles.
  
4. ```trianguloMayor(listaT)```: Recibe una lista de triángulos y entrega el triángulo de mayor perímetro. (Asuma que hay 1 solo triangulo de mayor perímetro).
