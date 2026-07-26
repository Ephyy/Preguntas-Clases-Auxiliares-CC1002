---
tags: [Clases y Objetos]
---

# Se acerca la Navidad (Parte 2)🎅🏻☃️🎄
Santa ha quedado muy feliz con la implementación de la Clase Trineo realizada en la pregunta anterior. Ahora para salvar la navidad, le pide ayuda para implementar las siguientes funciones, que trabajan con objetos Trineo:

1. Implemente la función ```mostrarCapacidad(listaT)``` que recibe una lista con objetos Trineos, y muestra en pantalla la cantidad de espacio restante que le queda a cada Trineo, linea por linea. Cada trineo se enumera por la posición en la que se encuentra en la lista, contando desde 1. Ejemplo:

    ```python
    >>> mostrarCapacidad(listaT) # suponiendo que tenemos 3 trineos
        Trineo 1 le quedan 23 espacios
        Trineo 2 le quedan 2 espacios
        Trineo 3 le quedan 0 espacios
    ```

2. Implemente la función ```consultar(nombre, listaT)```, que recibe una lista de Trineos, y el nombre de un niño(a). La función entrega ```True``` si es que en algún Trineo de la lista, hay algún regalo asociado a ese nombre, y ```False``` si no. Para esto, suponga que los nombres son únicos a lo largo de todos los Trineos.

3. Supongamos que Santa nos entrega un documento (archivo) donde escribió los deseos de un grupo de niños(as). El archivo tiene la siguiente forma:

    ```text
    vanessa quiere codigosecreto
    vicente quiere celular
    monserrat quiere play5
    ...
    # <nombre_persona> quiere <regalo>
    ```
  
    Con esto, cree la función ```llenarTrineo(arch)```, que recibe un string con el nombre de un documento como el anterior, lo procesa, construye un Trineo de tamaño adecuado, donde se agregaron a todas las personas de la lista junto a su regalo deseado, y entrega tal Trineo como resultado. 
    
    Ejemplo:
    
    - `llenarTrineo("regalos.txt")` entrega un Trineo de capacidad 3, que internamente se representa como:
      ```python 
      DT = {'vanessa':'codigosecreto', 'vicente':'celular', 'monserrat':'play5', ...}
      ```