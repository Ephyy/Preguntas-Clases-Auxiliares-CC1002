---
tag: [Control, Listas Recursivas]
---

# Lista de Personas [C2 2024-2]

Las siguientes instrucciones permiten definir variables y listas con datos de personas:

```python
# Persona: identificador(int) nombre(str)
estructura.crear('Persona', 'identificador nombre')
P1 = Persona(101, 'Ana Rios')   #ejemplo de variable de tipo persona
P2 = Persona(213, 'Juan Baeza') #ejemplo 2
P3 = Persona(21, 'María Caro')  #ejemplo 3
LP = lista(P1, lista(P2, lista(P3, listaVacia))) #lista de personas
```

Con esto, realice lo siguiente:
+ (2.0 ptos.) Escriba la función ```buscarPersona(Lpersonas, id)```, que recibe una lista de Personas y un identificador, y entrega la Persona que tiene ese identificador. Suponga que no hay personas repetidas en la lista, y que todas las personas tienen un identificador distinto. Si no existe una persona con el identificador indicado dentro de la lista, entonces la función entrega None. Ejemplos:
  - ```buscarPersona(LP, 213)``` entrega: ```Persona(213, 'Juan Baeza')```
  - ```buscarPersona(LP, 33)``` entrega: ```None```
  
+ (4.0 ptos.) Escriba la función ```listaPersonas(Lpersonas, Lids)```, que recibe una lista de personas y una lista de identificadores, y entrega una lista con las personas que tengan tales identificadores (sin incluir las que no existan en la lista de personas). Ejemplo:
  - Si tenemos la lista de identificadores 
  
    ```Li = lista(21, lista(33, lista(101, listaVacia)))```

    entonces ```listaPersonas(LP, Li)``` entrega: ```lista(P3, lista(P1, listaVacia))```
