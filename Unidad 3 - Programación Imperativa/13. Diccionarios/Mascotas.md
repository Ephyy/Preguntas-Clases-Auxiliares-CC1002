---
tags: [Diccionarios]
---

# Mascotas 🐶🐱

Como una actividad diferente y creativa, en cierto curso de CC1002 se propone realizar un conteo de las mascotas que los/las estudiantes poseen, para luego ver cuál es la mascota más preferida por la mayoría.

Suponga que usted tiene un diccionario de la siguiente forma, en donde dado el nombre de una persona integrante del curso, se obtiene una lista con los tipos de mascota que posee:

```python
pets = {
    'Valentin': ['gato', 'gato', 'gato', 'gato', ...],
    'Catalina': ['perro', 'perro'],
    'Matias': [],
    'Pia': ['tortuga', 'perro', 'elefante', 'perro'],
    ...
}
```

Con esto, se pide crear una función llamada ```mascotas(D)``` que recibe un diccionario de mascotas como el del ejemplo, y retorna un nuevo diccionario, donde la llave serán los tipos de mascotas, y su valor asociado es la cantidad de veces que apareció dicha mascota como mascota de alguna persona.

Para el ejemplo, se espera que la función entregue un diccionario de la siguiente forma:

```python
{
    'gato': 4,
    'perro': 4,
    'tortuga': 1,
    'elefante': 1,
    ...
}
```