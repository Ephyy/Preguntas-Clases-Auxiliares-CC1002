---
tags: [Control, Condicionales, Funciones, Programa Interactivo]
dificultad: Media
---

# Suma últimos pares dígitos

+  Escriba una función ```suma(numero)```, que reciba un entero positivo que contiene varios pares de dígitos. Por ejemplo, el número 12345678 contiene los pares 12, 34, 56 y 78. La función debe entregar la suma de los 3 últimos pares, por ejemplo, ```suma(12345678)``` devuelve ```168``` (34 + 56 + 78). Suponga que siempre se le entrega un número de al menos 6 dígitos. 

+ Escriba un programa que use la función suma en un programa que establezca el diálogo de consultas y resultados similar al indicado en el siguiente ejemplo:  

  ```
  País y medallas? 10091220
  Total: 41
  País y medallas? 21234110
  Total: 74
  País y medallas? 55102030
  Total: 60
  País Ganador: 21
  ```

Notas
- Cada número que se lee con�ene 4 pares (8 dígitos). Cada número iden�fica al país y las medallas de oro, plata y bronce obtenidas por ese país. Por ejemplo, el número 12345678 significa que el país 12 obtuvo 34 medallas de oro, 56 de plata y 78 de bronce.
- Se leen exactamente 3 números (como aparece en el ejemplo)
- El país ganador es el que ob�ene más medallas en total (suponga que no hay empates)
