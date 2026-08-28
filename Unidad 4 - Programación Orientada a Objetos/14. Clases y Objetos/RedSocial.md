---
tags: [Clases y Objetos, Interacción entre Objetos]
dificultad: Difícil
---

# Red Social

Debido al eventual cierre de su red social favorita, se ha propuesto crear su propia red social, para mantenerse en contacto con su grupo de amiwis. Para esto, ha trabajado muchos días diseñando el esquema de la red social en base a objetos, y ha concluido que una red social se puede representar como un objeto central (la red en sí), que se encarga de administrar la interacción entre los objetos que viven dentro de la red (las cuentas de las personas).

Con esto, ha implementado la Clase `Cuenta` , con las siguientes operaciones (puede asumir que está implementada y funcional)

| Método | Significado |
|---|---|
| `C = Cuenta(user)` | Constructor de un objeto `Cuenta`. Recibe el nombre/username que tendrá la cuenta. También crea una lista de publicaciones, seguidos e intereses (inicialmente vacías). |
| `C.getPublicaciones()` | Entrega la lista de publicaciones de la cuenta. |
| `C.getIntereses()` | Entrega la lista de intereses de la cuenta. |
| `C.getSeguidos()` | Entrega la lista de seguidos de la cuenta. |
| `C.follow(user2)` | Agrega a la lista de seguidos un nuevo username, si es que no se encontraba previamente. |
| `C.postear(msg)` | Agrega un nuevo mensaje a la lista de publicaciones de la cuenta. |
| `C.agregarInteres(gusto)` | Agrega a la lista de intereses un nuevo interés, si es que no se encontraba previamente. |

Con esto, ahora se propone a crear la clase `RedSocial` , que agrupa un conjunto de objetos Cuenta . Para esto, realiza lo siguiente

+ Implemente la clase `RedSocial` y su constructor. La única variable de estado sería un diccionario, que asocia `usernames` (str) a Objetos `Cuenta` (inicialmente el diccionario parte vacío)
  
+ Implemente el método ```crearCuenta(self,username)```, que crea una nueva Cuenta con el username indicado, si es que el username no existía previamente en la Redsocial. La cuenta creada se agrega al diccionario de Cuentas de la Redsocial.
  
+ Implemente el método ```publicar(self,username,msg)```, que postea el mensaje indicado, asociado a la cuenta indicada (agrega el msg a la lista de publicaciones de la cuenta)
  
+ Implemente el método ```seguir(self,user1,user2)```, que agrega a la lista de seguidos de la cuenta asociada a `user1`, el nombre de la cuenta `user2` . Debe verificar que ambas cuentas existan en la Redsocial antes de agregarlo.
 
+ Implemente el método ```sumarInteres(self,user,interes)```, que agrega a la lista de intereses de la cuenta asociada a `user`, el interés indicado.

+ Implemente el método ```verPerfil(self,user)```, que muestra en pantalla todas las publicaciones de la cuenta asociada a `user`.
  
+ Implemente el método ```verMuro(self, user)```, que muestra en pantalla todas las publicaciones de la cuenta asociada a `user`, y también muestra las publicaciones de todas las cuentas seguidas por `user`.
  
+ Implemente el método ```gustosSimilares(self, gusto)```, que entrega una lista con todos los username que tengan dentro de su lista de intereses, el gusto indicado.