# El dado 🎲 (C3-2015-02 P2)

La Clase `Dado` posee los métodos indicados en la siguiente Tabla:

| Método | Significado | Ejemplo |
|---|---|---|
| `D = Dado(L)` | Crea un dado de `L` lados, con un valor inicial `0` (para indicar que aún no ha sido lanzado). | `D = Dado(6)` |
| `D.lanzar()` | Lanza el dado, de manera que tome un valor aleatorio entre `1` y `L`. | `D.lanzar()` no entrega nada, pero modifica su valor, por ejemplo, a `3`. |
| `D.valor()` | Entrega el valor del Dado. | `D.valor()` entrega `3`. |
Al respecto:

+ Cree la Clase `Dado` con todos sus métodos. Suponga que internamente el dado se representa con dos atributos.

  - Un número entero que representa su valor actual
  - Un número entero que indica el valor máximo que puede tomar el dado

+ Cree la función ```lanzarDados(N, L)```, que recibe dos números enteros `N` y `L`. La función entrega como resultado una lista de `N` dados de `L` lados, donde cada dado se crea y lanza una vez. 
  
  Por ejemplo:

  - ```lanzarDados(2,6)``` entrega una lista con 2 objetos Dados de 6 caras (y cada uno tiene un valor al azar entre 1 y 6)