---
tags: [Listas Recursivas, Estructuras]
---

# Supermercado Vegan 🛒🥗

Valentina va periódicamente al supermercado a comprar comida para sobrevivir en en dia a dia en la universidad. Como en un supermercado hay mucha variedad de alimentos, los datos que mas le interesan a ella de un alimento son su nombre, el precio (en pesos), las calorías (en kcal), y si es un alimento vegan-friendly o no. El problema es que a veces, debido a lo caótico que puede resultar comprar en un supermercado, compra alimentos que no le gustan, o llega a la caja y no tiene dinero suficiente para comprar todo lo que tiene en su carrito de compras. 

Para efectos de Ejemplos y Testing, puede usar la siguiente lista de alimentos:

```python
Pollo = Alimento("Pollo", 3990, 2500, True)
Fideos = Alimento("Fideos", 800, 274, False)
Skittles = Alimento( "Skittles", 950, 240, True)
Leche = Alimento( "Leche", 600, 84, False)
Arroz = Alimento("Arroz", 750, 130, True)
Pan = Alimento( "Pan", 1030, 265, False)
Lechuga = Alimento( "Lechuga", 850, 15, True)
Manzanas = Alimento( "Manzanas", 690, 52, True)
Chocolate = Alimento( "Chocolate Trencito", 1249, 835, False)

carrito = lista(Pollo, lista(Fideos, lista(Skittles, lista(Leche , lista(Arroz , lista( Pan , lista(Lechuga , lista(Manzana, lista( Chocolate , listaVacia )))))))))
```

Hoy ayudaremos a Valentina, creando funciones para facilitar sus compras.

1. Diseñe una Estructura de datos llamada ```Alimento```, con los atributos adecuados para almacenar los datos de un alimento que le interesan a Valentina.

    Ahora supondremos que un carrito de compras se representa como una lista de alimentos.


2. Cree una función llamada ```agregarAlCarrito(carrito, alimento)```, que recibe un carrito y un alimento, y agrega este alimento al carrito de compras.

3. Cree una función llamada ```subTotal(carrito)```, que recibe un carrito, y entrega el monto que cuesta comprar todos los alimentos en el carrito de compras.

4. Cree una función llamada ```eliminarKCal(carrito)```, que recibe un carrito, y elimina del carrito todos los alimentos que superen las 800kcal.
   
    **(Propuesto)** Modificar la función para eliminar todos los alimentos que superen una cierta cantidad de kcal, entregadas como parámetro.

5. Cree una función llamada ```eliminarNoVegan(carrito)```, que recibe un carrito, y elimina del carrito todos los alimentos que no sean vegan-friendly.

6. Cree una función llamada ```comprar(carrito, dinero)```, que recibe un carrito y una cantidad de dinero, y entrega una lista de alimentos que pueden ser comprados, sin superar el monto en dinero entregado. Para esto, siga el siguiente algoritmo:
   - Se recorren uno por uno los alimentos del carrito
   - Si hay dinero para comprar el alimento actual, entonces se compra, y se descuenta su precio del saldo disponible para comprar. En caso contrario, no se compra.
   - El proceso se repite hasta que se acaben los alimentos del carrito, o el dinero para comprar.