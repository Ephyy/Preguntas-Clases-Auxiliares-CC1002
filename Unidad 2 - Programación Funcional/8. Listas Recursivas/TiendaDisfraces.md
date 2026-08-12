---
tags: [Listas Recursivas, Estructuras, Abstracción Funcional]
---

# Tienda de Disfraces

Una tienda de disfraces se encontró el dia de hoy con una sorpresa, ¡Los disfraces se encontraban desordenados y desparramados en el suelo!. La gente encargada de la tienda logró organizar todos los disfraces en una lista. Además, cada disfraz posee los siguientes atributos:

```python
# Disfraz: nombre(str) cantidad(int) talla(str)
estructura.crear('Disfraz','nombre talla cantidad')

LD = lista(Disfraz('fantasmita','XS',5),lista(Disfraz('fantasmita','S',0), lista(Disfraz('pirata','S',3),lista(Disfraz('esqueleto','M',5), lista(Disfraz('momia','M',0),lista(Disfraz('fantasmita','L',4), lista(Disfraz('momia','L',1),lista(Disfraz('esqueleto','XL',1), listaVacia))))))))
```

Como necesitan vender muchos disfraces el día de hoy, necesitan resolver rápidamente diversos problemas (y con rápidamente, nos referimos a que usen astutamente abstracción funcional en la solución si es posible), con ayuda de las siguientes funciones:

1. La función ```sinStock(Ld)``` que recibe una lista de disfraces y entrega una lista de disfraces cuya cantidad asociada sea 0.

2. La función ```filtrarTalla(Ld, t)``` que recibe una lista de disfraces y una talla, y entrega una lista de disfraces que solo tengan la talla entregada.

3. La función ```incrementar(Ld, nombre)```, que recibe una lista de disfraces, y un nombre. La función incrementa en 1 la cantidad asociada a los disfraces con ese nombre en la lista, sin importar su talla.

4. La función ```contar(Ld, t)```, que recibe una lista de disfraces y una talla, y entrega la cantidad total de disfraces de esa talla presentes en la lista.

5. La función ```agregar(Ld, nombre, t, n)```, que recibe una lista de disfraces, un nombre, una talla y una cantidad n. La función agrega el nuevo disfraz a la lista, con los datos entregados. Si el disfraz con las mismas características (nombre, talla) ya existía en la lista, entonces incrementa su cantidad en n.
