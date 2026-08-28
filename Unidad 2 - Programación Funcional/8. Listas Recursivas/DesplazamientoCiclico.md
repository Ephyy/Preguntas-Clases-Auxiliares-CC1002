---
tags: [Listas Recursivas]
---

# Desplazamiento cíclico 🔄

1. Cree la función ```desplazamiento(L, n)``` que reciba una lista `L` y un entero `n`, y desplace cada elemento de L hacia la derecha en n posiciones. Los elementos de la cola, van pasando hacia el inicio si la cantidad de posiciones a desplazar supera el largo de la lista.

    Por ejemplo, considere la lista:

    ```L = lista(1, lista(2, lista(3, lista(4, lista(5, listaVacia)))))```

    Entonces desplazamiento(L, 2) entregaría:

    ```L = lista(4, lista(5, lista(1, lista(2, lista(3, listaVacia)))))```

2. Cree la función ```desplazamientoInv(L, n)``` que reciba una lista `L` y un entero `n`, y desplace cada elemento de `L` hacia la izquierda en `n` posiciones. El algoritmo es el mismo del caso anterior, pero desplazando la lista hacia el lado contrario.

    Por ejemplo ```desplazamiento(L, 2)``` entregaría:

    ```L= lista(3, lista(4, lista(5, lista(1, lista(2, listaVacia)))))```