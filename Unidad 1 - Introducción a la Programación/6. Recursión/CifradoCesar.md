---
tags: [Recursión]
---

# Cifrando Números 🔑

Uno de los métodos clásicos de cifrado se conoce como el **Cifrado de César**, en el cual todas las letras de un mensaje son reemplazadas por la letra que se encuentra cierta cantidad de posiciones más adelante, donde tal cantidad se conoce como la **Llave de Cifrado**. En caso de que no existan letras más adelante en el abecedario (por ejemplo, después de la Z), entonces se retoma desde el principio del abecedario. Esto se conoce como **Rotación**.

En esta pregunta, haremos una adaptación de este cifrado, que solo opera con números enteros positivos, donde las cifras de nuestro abecedario serán
`0 1 2 3 4 5 6 7 8 9`.

Por ejemplo, si tenemos el número `14575`, y queremos cifrarlo con la llave `4`, eso significa que tenemos que desplazar cada uno de sus dígitos 4 espacios hacia adelante:

- `5` queda en `9`.
- `7` queda en `1`.
- `5` queda en `9`.
- `4` queda en `8`.
- `1` queda en `5`.

Por lo que el número final quedaría: `58919`


Note que también se puede cifrar con una llave negativa. Por ejemplo, si tenemos el número `14575`, y lo ciframos con la llave `-4`, obtenemos: `70131`

Con esto, programe las siguientes funciones:

1. Cree la función ```desplazar(d, k)```, que recibe un número entero positivo `d` de 1 dígito, y un número entero `k`. La función entrega el dígito que corresponde, luego de desplazar `d` una cantidad de `k` espacios.

    Por ejemplo:

    - ```desplazar(5, 2)``` entrega ```7```.
    - ```desplazar(5, -2)``` entrega ```3```.
    - ```desplazar(8, 5)``` entrega ```3```.

2. Cree la función ```cesar(N, k)```, que recibe un número entero positivo de largo arbitrario, y un número entero. La función entrega el número que resulta luego de aplicar el cifrado de `k` sobre `N`.

    Por ejemplo:

    - ```cesar(14575, 4)``` entrega ```58919```.
    - ```cesar(14575, -4)``` entrega ```70131```.

    En caso de que el dígito de más a la izquierda, luego del desplazamiento, resulte en un cero, reemplazarlo por un `1`.

    - ```cesar(14575, -1)``` entrega ```13464```.

    **Nota:**
    - Le puede servir usar un parámetro por omisión.