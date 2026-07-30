---
tags: [Condicionales]
---

# El O exclusivo

En lógica, así como existe la conjunción (`and`) y la disyunción (`or`), también existe el operador de disyunción exclusiva, que se comporta de acuerdo a la siguiente tabla de verdad:

| A     | B     | A ⊕ B |
|-------|-------|-------|
| False | False | False |
| False | True  | True  |
| True  | False | True  |
| True  | True  | False |

Como en python no existe esta operación, se le pide programar la función ```xor(b1, b2)```, la cual recibe dos expresiones booleanas, y entrega ```True``` si solo una de las expresiones recibidas es ```True``` (y la otra es ```False```), y ```False``` en cualquier otro caso (de acuerdo a la tabla de verdad). Ejemplos:

- ```xor(True, False)``` entrega ```True```
- ```xor(True, True)``` entrega ```False```
