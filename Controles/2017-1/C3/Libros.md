---
tags: [Control]
---
# Libros 📚 (C3-2017-01 P2)

Un objeto de la Clase Libro posee los métodos indicados en la siguiente Tabla:

| Método | Significado | Ejemplo |
|---|---|---|
| `L = Libro(codigo, titulo)` | Crea libro `L` con el código y título indicados. | `L = Libro("DOI-123", "Harry Potter")` |
| `L.prestar(persona)` | Presta libro `L` a la persona indicada. Entrega `True` si se pudo prestar correctamente, o `False` si ya estaba prestado. | `L.prestar("dani")` entrega `True`. |
| `L.devolver()` | Devuelve el libro `L`, por lo que ya no queda asociado a una persona. | `L.devolver()` |
| `L.lector()` | Entrega el nombre de la persona que tiene el libro (o `None` si no está prestado). | `L.lector()` entrega `None`. |
Al respecto:

+ Use los métodos anteriores para crear una función llamada ```prestados(LL)```, que recibe una lista de objetos `Libro`, y entrega el porcentaje de libros que están prestados. Por ejemplo, si se tiene:

  ```python
  L1 = Libro("DOI-123", "Harry Potter")
  L2 = Libro("DOI-456", "Como entrenar a tu dragon")
  L3 = Libro("DOI-789", "Alicia en el Pais de las Maravillas")
  ```

  Donde supondremos que solo `L2` se encuentra prestado, entonces:

  - ```prestados([L1, L2, L3])``` entrega: ```33.3```

+ Escriba los métodos Constructor y ```prestar``` de la clase Libro. Suponga que un objeto de la clase Libro se representa con los siguientes atributos:

  - ```__codigo```: string

  - ```__titulo```: string

  - ```__lector```: string (o ```None``` si no está prestado)
  