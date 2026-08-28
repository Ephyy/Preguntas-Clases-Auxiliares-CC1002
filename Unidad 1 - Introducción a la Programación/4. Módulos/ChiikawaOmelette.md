---
tags: [Módulos, Funciones, Programa Interactivo]
---

# Chiikawa y el Omelette Prohibido 🥘
Chiikawa es una famosa serie de TikTok de personajes principales Chiikawa, Usagi y Hachiware, todos muy glotones y amigables. 

Un día, los tres deciden preparar un omelette, pero antes necesitan calcular cuánto puede comer cada uno en un tiempo determinado. Para resolverlo, piden ayuda a les estudiantes del curso Introducción a la Programación, invitándoles a programar una función que realice el cálculo.

Considere que cada personaje come con respecto al tiempo una cantidad de:

- $C(t) = ln( t + cos(t))$
- $U(t) = exp(t) -1$
- $H(t) = 2(t - sin(t))$


1. Escriba un módulo llamado `chiikawa.py`, en el defina las funciones ```comida_Chiikawa(t)```, ```comida_Usagi(t)``` y  ```comida_Hachiware(t)```, que reciban un tiempo `t` `(int)` y entrega cuanto come cada personaje respectivo en ese tiempo redondeado a 1 decimal.

    Ejemplo:
    - ```comida_Chiikawa(3)``` entrega ```0.7```
    - ```comida_Usagi(3)``` entrega ```19.1```
    - ```comida_Hachiware(3)``` entrega ```5.7```

2. En otro archivo, utilizando el modulo anterior, haga un programa interactivo que pregunte por un tiempo y muestre en pantalla lo que come cada personaje y el total entre los tres.

    Por ejemplo, para un tiempo ingresado $t=3$ se tiene:
    ```python
    >> Ingrese un determinado tiempo: 3
    Chikawa come: 0.7   
    Usagi come: 19.1
    Hachiware come: 5.7
    Entre los tres comen un total de: 25.5
    ```

    ![Omelette](./img/omelette.jpg)


3. Chiikawa y amigos quedaron muy contentos con el trabajo, ¡pero resulta que no debían comerse el omelette! 

    Por este error, los llevan a la cárcel. Sin embargo, los policías están dispuestos a dejarlos en libertad si cada uno paga una multa proporcional a la cantidad de omelette que comió en comparación con lo que comieron entre los tres.
    
    Ayúdelos a calcular cuánto debe pagar cada uno creando una función (en el mismo archivo del programa de la parte B) ```porcentaje_omelette(u, h, c)```. Esta recibe la cantidad de omelette que comió cada uno de los tres amigos y muestra el porcentaje que representa lo que comió cada uno respecto del total comido entre los tres.

    Por ejemplo:
    ```python
    > porcentaje_omelette(0.7, 19.1, 5.7)
    Chiikawa comió un: 2.7% y debe pagar $2700  
    Usagi comió un: 74.9% y debe pagar $74900    
    Hachiware comió un: 22.4% y debe pagar $22400
    ```

    En este caso, el total de omelette comido por los tres es: $0.7 + 19.1 + 5.7 = 25.5$

    Por lo tanto, Chiikawa comió aproximadamente un 2.7% de lo que comieron entre los tres, Usagi un 74.9% y Hachiware un 22.4%. Como la multa total es de \$100.000, cada uno debe pagar el mismo porcentaje de la multa.
    

    *Indicaciones:* 
    - Notar que la función **muestra** valores en lugar de retornar. 
    - El porcentaje se calcula respecto del total de omelette que comieron los tres personajes, no respecto de la cantidad total de omelette que había originalmente.

      ![carcel](./img/carcel.jpg)