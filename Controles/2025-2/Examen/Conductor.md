---
tags: [Control, Clases y Objetos, Interacción entre Objetos]
---

# Auto / Conductor [Ex 2025-2]

Para modelar la interacción entre un Conductor y sus Automóviles, se han diseñado dos clases:

Aquí tienes la información organizada en dos tablas, una por clase:

- Clase `Auto`

  | Elemento | Detalle |
  |---|---|
  | **Atributos internos** | patente, marca, combustible (litros), rendimiento (km/litro), capacidad del estanque (litros) |
  | **Getters/Setters** | setPatente – getPatente, setMarca – getMarca, setCombustible – getCombustible, setRendimiento – getRendimiento, setCapacidad – getCapacidad |
  | `conducir(distancia)` | Resta del combustible los litros necesarios según el rendimiento para recorrer la distancia (km). Si el combustible alcanza, lo descuenta y retorna `True`; si no, retorna `False`. |
  | `cargar(litros)` | Carga combustible sin sobrepasar la capacidad del estanque. Retorna la cantidad realmente cargada. |
  | `toString()` | Retorna un String con formato: `'Patente – Litros disponible'` |

- Clase `Conductor`

  | Elemento | Detalle |
  |---|---|
  | **Atributos internos** | nombre, autos asignados (lista indexada de autos que puede conducir, sin elementos repetidos) |
  | **Getters/Setters** | setNombre – getNombre, setAutosAsignados – getAutosAsignados |
  | `asignar_auto(auto)` | Asigna el auto al conductor. |
  | `maneja(auto, km)` | Solo permite manejar si: el auto está asignado al conductor **y** el auto tiene combustible suficiente. Si se cumplen ambas condiciones, realiza el viaje y retorna ```True```; caso contrario, retorna `False`. |
  | `toString()` | Retorna un String con formato: `'Nombre_Conductor: [Patente – Litros disponible], …, [Patente – Litros disponible]'` |

+ **(3.0p)** Escriba la función ```SalirAConducir(patente, conductor, distancia)``` — sin receta de diseño, sólo encabezado y cuerpo de la función —, que recibe una patente, el objeto asociado a un conductor y la distancia en kilómetros. La función devuelve alguno de los siguientes CODIGOS (un número entero), según corresponda:
  
  | Código | Significado |
  |---:|---|
  | 1 | El viaje se pudo realizar. |
  | 2 | Error, insuficiente combustible. |
  | 3 | Error, el conductor no tiene asignado el vehículo. |

+ **(3.0p)** Para la clase `Conductor`, escriba los métodos `maneja`, `asignar_auto` y `toString` —sin receta de diseño, sólo encabezado y cuerpo del método—, considerando la siguiente definición de la clase:
 
  ```python
  class Conductor:
      def __init__(self, nombre):
          self.__nombre = nombre
          self.__autos_asignados = [] 
  ```