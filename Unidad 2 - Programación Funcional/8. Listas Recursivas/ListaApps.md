---
tags: [Listas Recursivas, Estructuras]
---

# Apps Celular 📱

En este ejercicio, supondremos que las aplicaciones de un teléfono celular se pueden representar mediante la siguiente estructura:

```python
# app: nombre(str) espacio(num)(medido en MB)
estructura.crear("app","nombre espacio")
```

También, supondremos que las apps instaladas en un teléfono celular, se pueden representar como una lista de apps:

```python
ws = app("whatsapp", 346)
insta = app("instagram",266)
tik = app("tiktok", 430)
LA = lista(ws, lista(insta, lista(tik, listaVacia)))
```

Al respecto, cree las siguientes funciones que trabajan con una lista de apps.

1. Cree la función ```instalarApp(Lapps, nuevaApp)```, que recibe una lista de apps y una nueva app, y entrega como resultado una nueva lista de apps, con la nuevaApp agregada a la lista. En caso de que la aplicación ya estuviese instalada previamente, entonces debe actualizar los datos asociados a esa aplicación (el espacio que ocupa), y entregar la Lista de apps, con el dato modificado.

    Por Ejemplo:

    - ```instalarApp(LA, app("netflix", 149))``` entrega ```lista(ws, lista(insta, lista(tik, lista(app("netflix", 149), listaVacia))))```
    - ```instalarApp(LA, app("instagram", 280))``` entrega ```lista(ws, lista(app("instagram", 280), lista(tik, listaVacia)))```

2. Cree la función ```eliminarApp(Lapps, nombre)```, que recibe una Lista de apps y el nombre de una app, y entrega como resultado la Lista de apps, a la cual le borraron la app con el nombre entregado. En caso de que la aplicación a borrar no se encuentre en la lista, entonces devuelve la lista de apps intacta. 
  
    Ejemplo:

    - ```eliminarApp(LA, "instagram")``` entrega ```lista(ws, lista(tik, listaVacia))```
    - ```eliminarApp(LA, "youtube")``` entrega ```lista(ws, lista(insta, lista(tik, listaVacia)))```

3. Cree la función ```espacio(Lapps)```, que recibe una lista de apps, y entrega como resultado el espacio que ocupan todas las aplicaciones instaladas en el teléfono.

    Ejemplo:

    - ```espacio(LA)``` entrega ```1042```