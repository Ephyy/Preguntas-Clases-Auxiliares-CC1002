# Tamagotchi

En este ejercicio, tenemos la misión de revivir a los conocidos *Tamagotchi*, ya que su Profesor de Cátedra nunca tuvo la oportunidad de jugar con uno durante su infancia.

Para empezar, modelaremos a los Tamagotchi mediante la siguiente estructura:

```python
# Tama: nombre(str) felicidad(int) hambre(int) tipo(str)
estructura.crear("Tama", "nombre felicidad hambre tipo")
```

En particular, los índices de **felicidad** y **hambre** no pueden ser negativos.

Con esto, cree las siguientes funciones para interactuar con estructuras `Tama`:

1. La función `esTamagotchi(T)`, que valida si el parámetro `T` corresponde a una estructura `Tama` válida.

    **Ejemplos:**

    ```python
    esTamagotchi(Tama("nekoo", 50, 20, "gato"))
    # True
    ```

    ```python
    esTamagotchi(Tama(23, 99.99, "tengo anvre", 11))
    # False
    ```

2. Si el Tamagotchi tiene mucha pena o mucha hambre, abandona al humano irresponsable y se va a buscar otro. Lo anterior ocurre cuando el índice de felicidad llega a 0 y/o el de hambre llega a 100.

    Cree la función `tamagotchiSeVa(T)`, que retorna `True` si el Tamagotchi cumple alguno de estos criterios y `False` en caso contrario.

    **Ejemplo:**

    ```python
    tamagotchiSeVa(Tama("nekoo", 0, 20, "gato"))
    # True
    ```

3. Función `alimentar(T)`, que dada una estructura Tama `T`, entrega un nuevo `Tama`, donde el índice de felicidad aumenta en 10 unidades, y el índice de hambre disminuye en 30 unidades. Ejemplo:

    Recuerde que los índices no pueden ser negativos.

    **Ejemplo:**

    ```python
    alimentar(Tama("nekoo", 50, 20, "gato"))
    # Tama("nekoo", 60, 0, "gato")
    ```

4. La función `jugar(T)`, que recibe una estructura `Tama` y retorna un nuevo `Tama` de acuerdo con las siguientes reglas:

     - Si el ind. de hambre está bajo 50, entonces el índice de felicidad aumenta en 30 unidades, y el
   índice de hambre aumenta en 30 unidades.

     - Si el ind. de hambre está sobre 50, entonces el Tamagotchi se niega a jugar, y el ind. de felicidad
   disminuye en 20 unidades.

    **Ejemplo:**

    ```python
    jugar(Tama("nekoo", 50, 20, "gato"))
    # Tama("nekoo", 80, 50, "gato")
    ```