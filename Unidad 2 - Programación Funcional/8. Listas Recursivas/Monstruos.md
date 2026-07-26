---
tags: [Listas Recursivas]
---

# Monstruos 👾

La empresa Monsters Inc. es una empresa dedicada a asustar a los niñas(os) para obtener energía a partir de sus gritos (de manera similar a lo que hace cierta facultad de ingeniería y sus evaluaciones demoníacas). La gerencia de esta empresa le pide ayuda para modelar algunas estimaciones y situaciones de emergencia que pudiesen ocurrir mientras se "recolecta" energía, para lo cual usted decide usar estructuras para representar a los Monstruos, y listas para representar un conjunto de Monstruos.

A continuación se muestra la definición de la estructura `Monstruo`, junto a listas de Monstruos para usar en las pruebas.

```python
# Monstruo: color(String) cant. de ojos(int) cant. de brazos(int) índice de susto(float)
estructura.crear("Monstruo", "color ojos brazos susto")

# Monstruos de prueba:
verde1 = Monstruo("verde", 2, 3, 22.0)
naranja1 = Monstruo("naranja", 3, 3, 42.0)
morado1 = Monstruo("morado", 1, 2, 33.3)

azul1 = Monstruo("azul", 3, 5, 6.3)
azul2 = Monstruo("azul", 5, 8, 1.0)
rojo1 = Monstruo("rojo", 1, 1, 15.2)
rojo2 = Monstruo("rojo", 9, 4, 35.5)

listaM1 = lista(verde1, lista(naranja1, lista(morado1, listaVacia)))
listaM2 = lista(azul1, lista(rojo1, lista(azul2, lista(rojo2, listaVacia))))
```

Al respecto, se pide resolver las siguientes situaciones:

1. Se ha activado un código 3312. Debido al impacto de esta situación, los Monstruos experimentan un curioso cambio: pierden un ojo, pero ganan 3 brazos. Cree la función `codigo3312(LM)`, que recibe una lista de Monstruos, y entrega una lista de Monstruos, donde cada Monstruo fue modificado de acuerdo a lo mencionado anteriormente.

    Ejemplo:

    - `codigo3312(listaM1)` entrega:

      ```python
      lista(
          Monstruo("verde", 1, 6, 22.0),
          lista(
              Monstruo("naranja", 2, 6, 42.0),
              lista(
                  Monstruo("morado", 0, 5, 33.3),
                  listaVacia
              )
          )
      )
      ```

    Puede suponer que los Monstruos de la lista tendrán al menos un ojo y pueden quedar sin ojos.

2. La Gerencia necesita identificar a los Monstruos que generen más susto, y así tengan más probabilidades de generar energía. Cree la función `peligrosos(LM, i)` que recibe una lista de Monstruos, y entrega una lista con los Monstruos que tengan un índice de susto mayor al valor `i` dado.

    Ejemplo:

     - `peligrosos(listaM1, 30)` entrega:

       ```python
       lista(naranja1, lista(morado1, listaVacia))
       ```

3. La Gerencia ahora necesita calcular cuánta energía podría ser generada por un grupo de Monstruos (asumiendo que tienen éxito en su misión). La fórmula para calcular la energía es:

    $$
    \sum_{i=1}^{n} \text{Mind}_i \cdot \sqrt{\text{Mojos}_i + \text{Mbra}_i}
    \qquad [\text{GPPM}]
    $$

    Donde $\text{Mind}_i$ corresponde al índice de susto del Monstruo, $\text{Mojos}_i$ es la cantidad de ojos del Monstruo, $\text{Mbra}_i$ es la cantidad de brazos del Monstruo, y la unidad de medida de la energía es **Gritos Por Parte de Monstruo (GPPM)**.

    Cree la función `trabajar(LM)`, que recibe una lista de Monstruos, y entrega la energía total que pueden generar los Monstruos en la lista.

    Ejemplo:

    - `trabajar(listaM1)` entrega aproximadamente `209.7493566`.