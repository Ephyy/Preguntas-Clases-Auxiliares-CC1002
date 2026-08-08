---
tags: [ABB, Árboles Binarios]
---

# Funciones ABB 

En clases se vieron los Arboles de Búsqueda Binaria (ABB). Ahora realizaremos algunas funcionalidades simples para entender el funcionamiento de estos árboles. Se pide implementar lo siguiente:

1. Función ```contarHojas(A)```, que dado un ABB, entrega la cantidad de hojas que posee.\
**Nota:** Las hojas de un árbol son aquellos nodos que no tienen “hijos”

2. Función ```altura(A)```, que dado un árbol ABB, nos entregue su altura. \
**Nota:** Altura es la distancia máxima que existe entre el nodo raíz y sus hojas

3. Función ```buscar(A,x)```, que dado un árbol ABB de números, entrega ```True``` si `x` esta en el ABB `A`.

4. Función ```agregar(A,N)```, que dado un árbol ABB y un numero `N`, inserta el numero en el árbol, manteniendo sus propiedades y siempre que el numero no exista en el árbol.