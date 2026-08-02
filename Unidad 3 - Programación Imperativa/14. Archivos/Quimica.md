---
tags: [Archivos, Listas Indexadas]
---

# Química 🧪

Los elementos de la tabla periódica se encuentran almacenados en un archivo `(tabla_periodica.csv')` bajo el siguiente formato:

```
simbolo,nombre,masa_atomica,grupo,tipo,estado_fisico
H,hidrogeno,1.008,1,no metal,gas
He,helio,4.0026,18,gas noble,gas
Li,litio,6.94,1,metal alcalino,solido
...
C,carbono,12.011,14,no metal,solido
N,nitrogeno,14.007,15,no metal,gas
O,oxigeno,15.999,16,no metal,gas
F,fluor,18.998,17,halogeno,gas
...
```

Es decir, la primera linea contiene los encabezados de una tabla, y las siguientes lineas contienen la
información asociada a un elemento químico. Puede asumir que todos los elementos de la tabla
aparecen en el archivo. Con esto se pide lo siguiente:

+ Cree la función `estado(E)`, que recibe un estado (```'solido'```, ```'liquido'```, ```'gas'```). La función, con ayuda del archivo tabla_periodica.csv', entrega una lista con el nombre de todos los elementos químicos que tengan tal estado físico. Ejemplo:
  - ```estado('solido')``` entrega: ```['litio', 'carbono', ...]```

+ Suponiendo que una molécula puede expresarse como una lista, por ejemplo: $H_{2}O$ se expresa como: ```['H', 'H', 'O']```, cree la función ```pesoMol(LM)```, que recibe una lista que representa una molécula, y entrega la masa de tal molécula (es decir, la suma de todos sus pesos atómicos). Ejemplo:
  - ```pesoMol( ['H', 'H', 'O'] )``` entrega: ```18.015```
