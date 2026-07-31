---
tags: [Control, Archivos, Diccionarios, Listas Indexadas]
dificultad: Muy difícil
---

# Resultados Votación [C3 2024-2]

En la reciente votación para gobernadores regionales, en cada región resultó elegida la persona candidata que obtuvo la mayor cantidad de votos. Esa mayoría debe ser al menos de un 40% de los sufragios válidamente emitidos en la región. Si en una región ninguna persona candidata alcanzó el 40% de los votos, entonces habrá una segunda elección entre las dos personas que obtuvieron más votos. Suponiendo que no hay empates en la votación y que todas las personas candidatas tienen nombres distintos:

+ (3.5 ptos.) Escriba una función de nombre ```ganador(D)```, que recibe un diccionario que asocia los nombres de las personas candidatas de una misma región con los votos que obtuvieron en la elección. El diccionario contiene la información de al menos dos personas candidatas. La función debe retornar una lista de largo uno o dos, que contenga el nombre de la persona ganadora (si es que obtuvo más del 40% de los votos), o bien, los nombres de las dos personas que obtuvieron más votos y que se enfrentarán en la segunda elección.

  Por ejemplo:
    - Si ```Dvotos = {"A":5, "B":15, "C":10}```, entonces ```ganador(Dvotos)``` devuelve ```["B"]```
  
      pues B obtuvo el 50% de los votos.
    - Si ```Dvotos = {"A":12, "B":10, "C":13}```, entonces ```ganador(Dvotos)``` devuelve ```["C","A"]```
      
      pues tales candidatos/as obtuvieron los porcentajes más altos de votos, con 37.1% y 34.3%
      respectivamente.

+ (2.5 ptos.) El archivo `"votos.txt"` contiene la información de las votaciones de todas las personas candidatas de
todas las regiones, ordenado por número de región. Cada línea del archivo contiene tres valores separados por "_":
el número de la región, el nombre de una persona y la cantidad de votos que obtuvo tal persona

  ```text
  1_Ana Gonzalez_400
  1_Ana Soto_3500
  ...
  13_Juan Perez_12345
  13_Juan Gonzalez_11245
  13_Juan Soto_12289
  ...
  ```

  Por ejemplo, la línea con el contenido ```"13_Juan Perez_12345"``` significa que en la región 13 el candidato de nombre "Juan Perez" obtuvo 12345 votos.

  Al respecto, escriba un programa que pida el número de una región y, usando la información del archivo y la función de la parte anterior (puede usar la función aún si no la implementó), muestre en pantalla el nombre de la persona ganadora en la región, o los nombres de las dos personas que competirán en la segunda elección. Dos ejemplos de ejecución del programa son los siguientes:

  ```python
  >>> Región? 13
  Juan Perez y Juan Soto
  ```

  ```python
  >>> Región? 1
  Ana Soto
  ```