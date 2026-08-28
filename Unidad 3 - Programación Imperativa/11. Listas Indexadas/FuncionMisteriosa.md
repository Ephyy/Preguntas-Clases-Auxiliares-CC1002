---
tags: [Listas Indexadas]
---

# Función Misteriosa

Se tiene la siguiente función misteriosa:

```python
def misterio(L,e):
    return L.append(e)  
```

Discuta que es lo que ocurre con Ln en cada una de las siguientes secuencias de acciones:

```python
# Secuencia 1 
>> Ln = [2,5,8] 
>> misterio(Ln,4)
```

```python
# Secuencia 2 
>> Ln = [2,5,8] 
>> Ln = misterio(Ln,4)
```

```python
# Secuencia 3 
>> Ln = [2,5,8]
>> Lm = Ln
>> misterio(Lm,4)
```



