# Disfraces

Un grupo de amiwis ha decidido anotar los disfraces que previamente han usado en fiestas, cumpleaños y eventos, en un diccionario, donde a cada persona, se le asocia una lista con los disfraces que tiene:

```python
disfracesEj ={ 'javiera' : ['pony','hada'],
               'ephy': ['gato','pony','diablo'],
               'dani' : [],
               'arianne' : ['araña','doggo','zelda', 'kirby'],
               'monse' : ['zombie','wooper'],
               'julieta': ['doggo','zelda','virus'],
               'vane' : ['doggo','hada','gato'] }       
```

Esto, con el objetivo de poder prestarlos, si es que alguien los necesita. Al respecto:


+ Escriba la función ```quienPuedePrestar(Ddisfraz, nombre_disfraz)```, que recibe un diccionario de disfraces y el nombre de un disfraz, y entrega una lista con los nombres de las personas que tienen tal disfraz. Ejemplos:

  - ```quienPuedePrestar(disfracesEJ, 'pony')``` entrega: ```['javiera', 'ephy']```
  - ```quienPuedePrestar(disfracesEJ, 'shrek')``` entrega: ```[]```


+ Escriba la función ```quienTieneMas(Ddisfraz)```, que recibe un diccionario de disfraces, y entrega el nombre de la persona que tiene más disfraces. Puede suponer que hay solo una persona que posee la mayor cantidad de disfraces. Ejemplo:

  - ```quienTieneMas(disfracesEj)``` entrega: ```'arianne'```

  **Propuesto:** Modifique su solución, para considerar el caso cuando puede haber más de una persona con la misma cantidad máxima de disfraces. 

+ Escriba la función ```cuantosHay(Ddisfraz)```, que recibe un diccionario de disfraces, y entrega un nuevo diccionario, en el cual la llaves son los nombres de los disfraces, y los valores son la cantidad de disfraces de ese tipo/nombre en el diccionario original. Por ejemplo:

  - ```cuantosHay(disfracesEj)``` entrega:

  ```python
  { 'pony': 2 , 'hada': 2, 'gato': 2,
    'zombie': 1, 'doggo': 3, 'diablo':1,
    'wooper': 1, 'zelda': 2, 'virus': 1,
    'araña': 1, 'kirby': 1
  }
  ```