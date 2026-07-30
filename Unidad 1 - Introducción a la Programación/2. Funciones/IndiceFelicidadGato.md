---
tags: [Funciones]
---
# Calculando el IFG 

El Índice de Felicidad de un Gato (IFG) al recibir un churu, puede calcularse con la siguiente formula:

$$ I = (\frac{3 \cdot G}{e^{H}}) \cdot (\frac{1 + ln(C)}{2}) $$

- $C$ = Ganas de comer del gato. Es un factor aleatorio entre 1 y 10, donde 1 es pocas ganas y 10 muchas ganas.
- $G$ = Gramos de churu consumidos.
- $H$ = Insipidez del churu. 0 significa que es muy sabroso, y 5 muy insípido.

(Obviamente esta formula incluye un factor aleatorio, pues los gatos son impredecibles.)

Cree la función ```ifg_churu(gramos, insipidez)```, que recibe los gramos de churus consumidos y sabor del churu, y calcula el índice antes descrito. Por simplicidad, redondee el resultado obtenido a 2 decimales.

```python
>> ifg_churu(200,0)
961.7
>> ifg_churu(200,0)
801.88
>> ifg_churu(250,4)
20.88
```

**Nota:** Dado que la formula usa un factor aleatorio, una misma invocación de la función puede entregar resultados distintos. Por lo tanto, no es testeable.