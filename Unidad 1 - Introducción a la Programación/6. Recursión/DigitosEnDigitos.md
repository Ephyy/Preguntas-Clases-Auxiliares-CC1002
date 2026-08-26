---
tags: Recursión
dificultad: Media
---

# Dígitos en dígitos 🤯

Queremos revisar si todos los dígitos que componen un entero positivo `n` están contenidos en un numero (entero positivo) `m`, sin importar el orden ni cuantas veces aparecen. Para esto, siga los siguientes pasos:

1. Programe una función ```buscarDigito(n, d)``` que reciba un número entero positivo `n` (incluyendo el cero) y un dígito `d`. La función debe entregar ```True``` si el dígito `d` aparece dentro de los dígitos de `n`, y ```False``` en caso contrario.

    Ejemplo:
    - ```buscarDigito(0, 0)``` entrega ```True```
    - ```buscarDigito(5, 0)``` entrega ```False```
    - ```buscarDigito(314830, 1)``` entrega  ```True```
    - ```buscarDigito(123456, 7)``` entrega  ```False```

2. Programe una función ```estaContenido(n, m)``` que revise si todos los dígitos de un numero entero positivo `n` están contenidos en `m`. Use la función `buscarDigito` para programar su función.

    Ejemplo:
    - ```estaContenido(1, 5)``` entrega ```False```
    - ```estaContenido(13,98473341)``` retorna ```True```
    - ```estaContenido(983729,23)``` retorna ```False```
