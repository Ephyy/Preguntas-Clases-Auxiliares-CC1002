---
tags: [Archivos, Listas Indexadas]
---

# Uma Musume 🐴

Se cuenta con un archivo CSV llamado `carreras.csv` que contiene información de distintas carreras de Uma Musume, el cual sigue el siguiente formato:

```
fecha,pista,uma,posicion,tiempo_s
2025-06-01,Nakayama,Tokai Teio,2,96.3
2025-06-02,Tokyo,Mejiro McQueen,1,120.1
2025-06-03,Kyoto,Special Week,1,93.8
2025-06-04,Tokyo,Tokai Teio,3,98.4
2025-06-05,Nakayama,Mejiro McQueen,2,119.5
2025-06-06,Kyoto,Special Week,1,94.2
2025-06-07,Tokyo,Gold Ship,1,130.0
2025-06-08,Tokyo,Special Week,4,95.1
2025-06-09,Kyoto,Tokai Teio,1,97.0
2025-06-10,Nakayama,Gold Ship,2,128.5
```

La primera línea corresponde a los encabezados de una tabla y las siguientes líneas corresponden a la información de una determinada carrera. Teniendo en cuenta lo anterior, se le pide lo siguiente:

+ Implemente la función ```filtrarPorPista(nombreArchivo, pista)``` que reciba el nombre de un archivo CSV de carreras y una pista (por ejemplo ```"Tokyo"```), y escriba un nuevo archivo con el nombre de la pista (por ejemplo Tokyo.csv) con solo aquellas carreras que ocurrieron en esa pista. Este nuevo archivo debe incluir la línea de encabezado original.
  
  Por ejemplo, ```filtrarPorPista("carreras.csv", "Tokyo")``` genera el siguiente archivo `Tokyo.csv`:

  ```
  fecha,pista,uma,posicion,tiempo_s
  2025-06-02,Tokyo,Mejiro McQueen,1,120.1
  2025-06-04,Tokyo,Tokai Teio,3,98.4
  2025-06-07,Tokyo,Gold Ship,1,130.0
  2025-06-08,Tokyo,Special Week,4,95.1
  ...
  ```

+  Cree la función ```promedioUma(nombreArchivo, nombreUma)``` que reciba el nombre del archivo CSV de carreras y el nombre de una Uma Musume (por ejemplo ```"Mejiro McQueen"```), y retorne una lista de dos elementos: `[nombreUma, prom]`, donde prom es el promedio de sus tiempos de carrera, redondeado a dos decimales.
  
    Si la Uma Musume no tiene registros, debe retornar ```[nombreUma, 0.0]```.

    Por ejemplo:
    - ```promedioUma("carreras.csv", "Tokai Teio")``` entrega ```['Tokai Teio', 97.23]```
    - ```promedioUma("carreras.csv", "Mejiro McQueen")``` entrega ```['Mejiro McQueen', 119.8]```
    - ```promedioUma("carreras.csv", "Rice Shower")``` entrega ```['Rice Shower', 0.0]```