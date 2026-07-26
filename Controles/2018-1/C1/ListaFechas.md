---
tags: [Control, Listas Indexadas]
---

# Listas de Fechas (P2-A C1 2018-01)

Una fecha puede ser representada como un número entero de la forma `AAAAMMDD`. Por ejemplo, `20180503` representa la fecha **3 de mayo de 2018**.

Escriba la función `fechasDelMes(L, m)`, que recibe una lista de fechas y un número que representa un mes. La función debe entregar una lista solo con las fechas que correspondan al mes indicado.

Ejemplo:

```python
LF = lista(18790521, lista(18100918,
     lista(18180212, lista(20180503, listaVacia))))

fechasDelMes(LF, 5)
# entrega:
lista(18790521, lista(20180503, listaVacia))
```