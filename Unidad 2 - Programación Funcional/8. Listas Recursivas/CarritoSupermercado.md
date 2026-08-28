---
tags: [Listas Recursivas, Estructuras]
---


# Carrito Supermercado 🛒

Un carrito de supermercado puede ser representado como una Lista de Artículos para el hogar,
en donde cada Artículo es una estructura como la siguiente:

```python
# articulo: nombre(str) cantidad(int) precio(int)
estructura.crear("articulo","nombre cantidad precio")
```

Suponiendo que usted tiene creada una Lista de Artículos (por simplicidad, usaremos la palabra **carrito** como sinónimo), se le pide que realice las siguientes funciones:

1. Una función llamada ```precioTotal(Larts)```, que recibe un carrito y entrega como resultado, la suma de los precios de cada uno de los Artículos que se encuentran dentro del carrito.

2. Una función llamada ```agregar(Larts, nuevoArt)```, que recibe un carrito y un nuevo artículo `nuevoArt`, y entrega como resultado una nueva Lista de Artículos, con el nuevo Artículo agregado al final de la Lista. En caso que el Artículo ya se encontrara dentro del carrito, debe actualizarse la cantidad de éste como la suma de lo que había y lo que está agregando, y su nuevo precio será el mínimo entre ambos Artículos. Finalmente se debe entregar la Lista de Artículos con el dato modificado.
   
    **Indicación:** Puede suponer que no hay nombres distintos para un mismo artículo.

3. Una triste función llamada ```recortar(Larts, maxTotal)``` que recibe un carrito y un precio máximo total admitido, y devuelve una nueva Lista de Artículos cuyo precio total sea menor o igual a `maxTotal`. En caso que el carrito no cumpla, deben ir quitándose los Artículos desde el inicio (ver Indicación), hasta que se cumpla la condición, o bien, hasta que el carrito quede vacío.

    **Indicación:** Al quitar Artículos, se retiran todas las unidades de éstos, y no una a una.

4. (Propuesto) Modifique la función del item anterior para que en vez de quitar la cantidad completa del primer Artículo del carrito, vaya quitando de uno en uno.

5. Una función llamada ```contiene(Larts, name)```, que recibe un carrito y un string name que corresponde al nombre de un Articulo y entrega como resultado ```True``` si es que existe un Artículo en el carrito con dicho nombre, o ```False``` en caso contrario.

6. Una función llamada ```partyHard(Larts, partyL)``` que recibe un carrito y una Lista de strings con nombres de Artículos que comúnmente se usan en las fiestas, y retorna ```True``` si es un carrito partyHard, es decir, si para cada uno de los nombres dentro de `partyL` existe un Artículo con dicho nombre en `Larts` , o ```False``` en caso contrario.
