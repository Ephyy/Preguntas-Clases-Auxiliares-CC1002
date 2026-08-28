---
tags: [Listas Recursivas, Estructuras, Abstracción Funcional]
titulo: Tienda de Disfraces (Variante 1)
---

# Tienda de Disfraces (Variante 1)

Una conocida tienda de disfraces se esta preparando para Halloween. Por experiencia de años anteriores, Claudia, la dueña del local, sabe que gran parte de las ventas se realiza a ultima hora, por lo que quiere estar preparada para controlar las ventas. Los inventarios de disfraces en la bodega se almacenan como una lista de estructuras Disfraz, en donde cada Disfraz es una estructura como la siguiente:


```python
# Disfraz: nombre(String) talla(String) precio(Int)
estructura.crear("Disfraz","nombre talla precio")

hada = Disfraz("hada", "M", 7500) furry = Disfraz("panda" "L", 8000)
sus = Disfraz("amongus", "M", 6500) poke = Disfraz("eevee", "S", 7000)
LD = lista(hada, lista(furry, lista(sus, lista(poke, listaVacia))))
```

Para esto, ayudaremos a Claudia, implementando las siguientes funciones en Python, usando exclusivamente **abstracción funcional**.

1. Cree la función ```disfracesTalla(L, T)```, que recibe una lista de disfraces y un string que indica una talla (```"S"```, ```"M"```, etc.). La función debe entregar una lista con todos los disfraces cuya talla sea igual a la entregada como parámetro. Ejemplo:
     - ```disfracesTalla(LD, "M")``` entrega ```lista(hada, lista(sus, listaVacia))```
  
2. Claudia sabe que la gente de cierta facultad se está preparando para cierto evento conocido como el día del disfraz, por lo que decide hacerles un descuento. Cree una función llamada ```descuento(L, d)```, que recibe una lista de disfraces y un % de descuento, y entrega una nueva lista de disfraces, a los cuales se les cambió el precio, aplicando el descuento indicado. Ejemplo: 

      - ```descuento(LD, 0.2)``` entrega:
         ```python
         lista(Disfraz("hada", "M", 6000), lista(Disfraz("panda" "L", 6400), lista(Disfraz("amongus", "M", 5200), lista(Disfraz("eevee", "S", 5600), listaVacia))))
         ```

3. Cree la función ```ganacias(L)```, que recibe una lista de Disfraces, y entrega las ganancias esperadas de la venta de disfraces, asumiendo que se venden todos los disfraces de la lista. Ejemplo:
     - ```ganancias(LD)``` entrega ```29000```
