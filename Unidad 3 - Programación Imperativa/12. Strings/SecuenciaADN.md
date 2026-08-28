---
tags: [Strings, Ciclos Iterativos]
---

# Secuencia de ADN 🧬

Emilia está realizando unos experimentos en un laboratorio de biotecnología de la facultad. En tal experimento, se representan las secuencias de ADN como una sucesión de caracteres A, C, G y T, que representan las bases de nucleótidos (Adenina, Citosina, Guanina y Timina). Suponiendo que esta secuencia es representada como un string, y las reglas del laboratorio prohíben usar la función .count de strings y listas, ayude a Emilia a programar las siguientes funciones:

+ Cree una función llamada ```frecuencia(adn, nuc)```, que dada una secuencia de ADN y un nucleótido, entrega el porcentaje de presencia de ese nucleótido con respecto a toda la secuencia de ADN. Por ejemplo:

  - ```frecuencia('AGCTT', 'A')``` entrega ```20.0```
  - ```frecuencia('TACGCTTT', 'T')``` entrega ```50.0```

+ Cree una función llamada ```enlacesDebiles(adn)```, que dada una secuencia de ADN, cuenta y entrega la cantidad de enlaces débiles presentes en la secuencia. Un enlace débil se define como el par de nucleótidos 'AT' en una secuencia. Por ejemplo:

  - ```enlacesDebiles('AGCTT')``` entrega ```0```
  - ```enlacesDebiles('ACCTATGGTAAT')``` entrega ```2```


+ Cree una función llamada ```subSecuencia(adn,nuc)```, que dada una secuencia de ADN, entrega la subsecuencia de ADN mas grande, que se encuentre entre 2 nucleótidos idénticos dado. En caso de existir mas de una subsecuencia mayor, entregar la primera encontrada. Por ejemplo:

  - ```subSecuencia('ATACTCGTACTTCACTCC','C')``` entrega ```'CGTAC'```
  - ```subSecuencia('CATCAT','C')``` entrega ```'CATC'```
