---
tags: [Control, Archivos, Diccionarios, Listas Indexadas]
---

# Archivos CSV 📝[C3 2025-2]

Una tabla de datos se representa por un diccionario `(dict)`. Cada llave corresponde al nombre de una columna de la tabla, y cada valor es una lista con los datos de la columna respectiva. A continuación, se muestra de forma visual un ejemplo de una tabla con datos de personas, y el diccionario `df` que se usa para representarla. 

| Nombre | Edad | Peso | Altura |
|---|---:|---:|---:|
| Pedro | 34 | 78.4 | 1.76 |
| Andrea | 25 | 54.3 | 1.63 |
| Kevin | 56 | 82.9 | 1.80 |

```python
df = {'nombre': ['Pedro', 'Andrea', 'Kevin'],
      'edad':   ['34', '25', '56'],
      'peso':   ['78.4', '54.3', '82.9'],
      'altura': ['1.76', '1.63', '1.80']} 
```

Para las siguientes preguntas puede asumir que el diccionario de la variable `df` existe, por lo que puede ser utilizado en la receta de diseño.

+ **(3.0p)** Los archivos de texto que siguen el formato CSV **(comma-separated values)** buscan representar en su contenido conjuntos de datos organizados como una tabla. Cada línea de texto representa una fila de la tabla, y los valores de cada columna se separan por una coma (`,`). La primera línea del archivo representa la fila con los títulos de las columnas (que son distintos entre sí). Por ejemplo, el siguiente archivo, de nombre `datos.csv`, sigue el formato CSV:

  ```text
  nombre,edad,peso,altura
  Pedro,34,78.4,1.76
  Andrea,25,54.3,1.63
  Kevin,56,82.9,1.80
  ```

  Escriba la función ```leerDatos(nombre)``` (sin receta de diseño, sólo el cuerpo de la función), que recibe el nombre de un archivo (un **String**), y entrega un diccionario con la información que contiene. Puede asumir que el contenido del archivo sigue el formato CSV correctamente. 

+ **(1.0p)** Escriba la función ```obtenerColumna(D, c)``` (con receta de diseño completa), que recibe un diccionario que representa una tabla, y el nombre de una columna. La función entrega **una nueva lista** con los datos copiados de la columna correspondiente. Ejemplos:
  - ```obtenerColumna(df, 'nombre')``` entrega: ```['Pedro', 'Andrea', 'Kevin']```
  - ```obtenerColumna(df, 'edad')``` entrega: ```['34', '25', '56']```
  - ```obtenerColumna(df, 'peso')``` entrega: ```['78.4', '54.3', '82.9']```

+ **(2.0p)** Escriba la función ```obtenerFila(D, f)``` (sin receta de diseño, sólo el cuerpo de la función), que recibe un diccionario que representa una tabla, y el índice de una fila con datos. La función entrega **un nuevo diccionario** con los datos de la fila correspondiente. Ejemplos:

  - ```obtenerFila(df, 0)``` entrega ```{'nombre': 'Pedro', 'edad': '34', 'peso': '78.4', 'altura': '1.76'}```
  - ```obtenerFila(df, 1)``` entrega ```{'nombre': 'Andrea', 'edad': '25', 'peso': '54.3', 'altura': '1.63'}```
  - ```obtenerFila(df, 2)``` entrega ```{'nombre': 'Kevin', 'edad': '56', 'peso': '82.9', 'altura': '1.80'}```

