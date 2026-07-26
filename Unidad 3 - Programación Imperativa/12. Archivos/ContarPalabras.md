# Contar Palabras 🔤

A Vicente le gustan mucho las historias y fábulas infantiles, las cuales guarda en archivos de texto como el siguiente:

**zorro_cigueña.txt**

```text
Al zorro le encantaban las bromas pesadas y quiso gastarle una a su amiga la cigüeña. Un día la invitó a cenar a su casa y la cigüeña aceptó con mucho agrado. La cigueña se presentó a la hora acordada y tras conversar un buen rato, se dirigieron al comedor. El zorro había preparado una deliciosa sopa, pero la sirvió en dos platos muy llanos. La cigüeña apenas pudo probar la sopa con la punta de su largo pico. El zorro, entre risas burlonas, se tomó toda la sopa y al final se lamió y relamió el plato. La cigüeña pronto se dio cuenta de la broma de mal gusto que le estaba jugando el zorro. Sin embargo, disimuló su enojo. Al despedirse, dio las gracias al zorro dejándole saber que estaba invitado a almorzar a su casa al día siguiente. El zorro se presentó en la casa de la cigüeña. Al entrar, sintió un olor exquisito que le hizo agua la boca y lo llenó de emoción. Pero la emoción le duró poco, porque el guiso que había preparado la cigüeña le fue servido en un jarro muy largo y de cuello estrecho. La cigüeña alcanzaba fácilmente el guiso con su pico, pero no el zorro con su hocico ancho y corto. El zorro, muy avergonzado, se marchó con el rabo entre las patas.
```

Al respecto, a Vicente le interesa saber cuál es la palabra que más se repite en los cuentos, por lo que le pide ayuda para programar las siguientes funciones:

+ Cree la función `separar(nombre_archivo)`, que recibe el nombre de un archivo de texto. La función debe procesar las líneas del archivo, y entregar una lista con todas las palabras del documento (sin importar si están repetidas), que tengan largo mayor a 3. Ejemplo:

  - `separar("zorro_cigueña.txt")` entrega:

    ```python
    ["zorro", "encantaban", "bromas", ...]
    ```

+ Cree la función `masRepetida(Lpalabras)`, que recibe una lista de strings (como la que se obtiene con la función anterior). La función debe entregar la palabra de largo mayor a 2 que más se repite dentro de la lista. Puede asumir que solo hay una palabra que se repite más veces dentro de la lista. Ejemplo:

  - `masRepetida(["zorro", "encantaban", "bromas", ...])` entrega:

    ```python
    "zorro"
    ```