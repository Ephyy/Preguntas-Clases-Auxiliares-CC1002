---
tags: [Clases y Objetos]
---

# El Trineo de Santa (Parte 1) 🦌🎁🎄

Se acerca Navidad! (Y nosotros aún aquí uwu) Y nuestro queride Santa, para traer la felicidad a todos los niños y niñas del mundo, le pide ayuda a usted en la preparación de los trineos para repartir los regalos. Para ello se le suministra a usted la siguiente definición y métodos de la clase Trineo:

| Método | Significado |
|---|---|
| `T = Trineo(N)` | Constructor de un objeto Trineo. Recibe la cantidad máxima de regalos que puede almacenar. |
| `T.agregarRegalo(nombre, regalo)` | Dado un nombre y un regalo (ambos strings), se le asigna al niño(a) de nombre entregado tal regalo. Si no queda espacio en el trineo, entonces no agrega el regalo. |
| `T.capacidadTotal()` | Entrega la capacidad total que tiene el trineo. |
| `T.obtenerRegalos()` | Entrega un listado con los niños(as) y sus regalos asociados. |

Con esto, Santa le pide ayuda con lo siguiente:

1. Implemente todos los métodos de la clase Trineo descritos en la tabla anterior. 
  
     - Considere que el campo (variable de estado) que describe a un trineo se modelará como un diccionario, donde cada llave es el nombre de un niño(a) y su valor es el regalo asociado a tal niño(a)
     - Considere un campo numérico para registrar la capacidad máxima del Trineo
     - Puede suponer que los nombres son únicos


2. Implemente un nuevo método, llamado ```capacidadRestante()```, que calcula y entrega la cantidad de espacio restante disponible en el Trineo.