---
tags: [Listas Recursivas, Estructuras]
---

# Prendas 👚

Su profe tiene un armario lleno de ropa, y tiene problemas para elegir ropa que combine día a día. Sus auxiliares, le dicen que en su curso hay mucha gente con buen gusto que pueden ayudarlo. 

Para afrontar el problema supondremos que la ropa se representa a través de la estructura `Prenda`, y un `Armario` como una Lista de Prendas.

```python
# Prenda: nombre(str) tipo(str) tag1(str) tag2(str)
estructura.crear('Prenda', 'nombre tipo tag1 tag2')
```
El atributo `tipo` puede tomar uno de los siguientes valores:

- ```"zapatos"```
- ```"pantalón"```
- ```"polera"```

Por otro lado, `tag1` y `tag2` corresponden a clasificadores que describen la prenda y cada Prenda debe tener dos tags distintos. Estos pueden ser:

- ```"simple"```
- ```"linda"```
- ```"elegante"```
- ```"animada"```

Por ejemplo, una polera con un gato podría ser considerada linda y animada:

```python
Prenda('polera de gato', 'polera', 'linda', 'animada')
```

Como sabemos que a su profe le gusta verse lo mas diva posible, programe las siguientes funciones:


1. La función ```agregar(L, P)```, que recibe un Armario `L` y una `Prenda`, y agrega la Prenda al Armario. Si ya existe una prenda exactamente igual, entonces deja el armario intacto.

2. La función ```quitar(L, nombre)```, que recibe un Armario `L` y el nombre de una prenda, entregando como resultado una Lista sin la prenda de ese nombre.

3. La función ```filtrarPorTipo(L, tipo)```, que recibe un Armario `L` y un tipo de Prenda, y entrega una Lista que contenga solo las Prendas de ese tipo que están en el Armario.

4. La función ```filtrarPorTag(L, tag)```, que recibe un Armario `L` y un tag, y entrega una Lista que contenga solo Prendas que tengan ese tag.

5. La función ```buscarPrendas(L, tipo, tag)```, que recibe un Armario `L`, un `tipo` y un `tag`, y entrega una Lista con todas las Prendas que cumplan con ser de ese tipo y que contengan ese tag.

6. La función ```existeCombinacion(L, tag)```, que entrega ```True``` si es que en el Armario `L` existe al menos una prenda de cada tipo que contenga el tag entregado.

7. **(Propuesto)** La función ```quitarPorTipo(L,tipo)```, que recibe un Armario `L` y un `tag`, y elimina del Armario todas las prendas que contengan ese tag.