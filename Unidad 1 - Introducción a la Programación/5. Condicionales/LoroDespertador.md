---
tags: [Condicionales, Funciones]
---

# Loro Despertador

Considere que usted tiene un loro despertador al cual usted puede programar para que lo despierte con mensajes personalizados dependiendo de la ocasión. Estos mensajes son:

- Si es fin de semana, entonces depende si es sábado o domingo y si son vacaciones o no. \
Si es sábado sin vacaciones, debe decirle *“Se viene el control, wiii! :D”*, y en caso de ser un sábado con vacaciones o un domingo, debe despertarle diciendo *“Levántate humano flojo! Son las 11:00!”*
- Si es día de semana, entonces depende si son vacaciones o no. Si es en vacaciones, usa el mismo mensaje que para los fines de semana, en cambio si no son vacaciones, debe decir: *“Beauchef bonito te espera :) Son las 7:30 am!”.*
- Hay días donde la pera es fuerte, entonces, independiente del día, después del mensaje, el loro debe decir: *“La pera es fuerte en tí, humano...”*.


Para ello cree una función de encabezado ```loroDespertador(dia, vacaciones, pera)```, en donde dia corresponde a un número entero entre 1 y 7 inclusive, representando cada uno de los días de la semana, comenzando desde el Lunes. Vacaciones y pera son boolean, que indican su estado correspondiente. (Por ejemplo si vacaciones es False, entonces es un periodo de clases).


