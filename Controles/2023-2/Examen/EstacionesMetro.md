# Estaciones de Metro (EX-2023-02 P2)

Los nombres de las estaciones de una línea del Metro se pueden representar en una lista recursiva. Por ejemplo:

```python
L1 = lista("San Pablo", lista(..., lista("Los Dominicos", listaVacia)...)).
```

Al respecto, escriba la función ```comunes(X,Y)```, que recibe dos lineas de metro, y entrega una lista con los nombres de las estaciones que son comunes a las líneas del metro ``X`` e ``Y``.

Por ejemplo, si `L5` es una lista con las estaciones de la línea 5 del metro de Santiago y `L3` una lista con las estaciones de la línea 3, entonces:

 - ```comunes(L5,L3)``` entrega: ```lista("Plaza de Armas", lista("Irarrazaval", listaVacia))```, ya que los trenes de esas dos líneas se detienen en esas dos estaciones.
 
Notas:
- Pueden usar las funciones del módulo lista (cabeza, cola, esLista, esVacia y largo)
- Para realizar sus tests, defina al menos dos listas (a modo de ejemplo). No es necesario que replique exactamente la red de Metro de Santiago, puede inventar nombres de estaciones.

**Propuesto:** Realizar la función utilizando ciclos en lugar de recursión.