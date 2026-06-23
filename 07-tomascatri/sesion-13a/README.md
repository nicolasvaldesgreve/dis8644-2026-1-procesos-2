# sesion-13a

Martes 9 de junio

## Apuntes

* **Gambiarra** = solución improvisada o arreglo rápido utilizando los recursos disponibles.

* En Cuba se desarrolló tecnología utilizando chatarra. Debido a bloqueos internacionales, fue necesario reutilizar y reparar constantemente los recursos disponibles en lugar de adquirir equipos nuevos.

* **Exploratorio Medellín** = laboratorio ciudadano de innovación y experimentación enfocado en aprendizaje y creación colaborativa.

* **P2P (Peer to Peer)** = comunicación de persona a persona, sin un servidor central; la información se comparte directamente entre usuarios.

---

## Exportación de PCB

* Para exportar una PCB se utiliza el formato **.gerber**.

* Se deben exportar **7 capas**:
  * `F.Cu`
  * `B.Cu`
  * `F.Silkscreen`
  * `B.Silkscreen`
  * `F.Mask`
  * `B.Mask`
  * `Edge.Cuts`

* También se debe generar el **archivo de taladros (Drill)**.

* A partir de ahí se utilizan los archivos **Gerber + Drill** para fabricación.

* **KiCad** permite revisar el resultado mediante un **visor Gerber** para verificar que todo esté correctamente configurado.

* Se pueden agregar más opciones o componentes usando una placa similar a una **protoboard**, pero diseñada para soldadura.

---

## Conceptos adicionales

* **Tape loops (bucles de cinta)** = consisten en cortar un tramo de cinta magnética y unir sus extremos para crear una pista continua.

* Las placas pasaron por un proceso de mejora; debemos revisar los cambios realizados por los profesores, procesarlos y comparar las diferencias existentes.

* Se observó un cambio en los resistores de entradas y salidas.

---

## Cambios realizados

### g-02-sec-01-rev-a

#### En esquemático

* Agregaron un resistor desde **Clock In** a **GND** para implementar **pull-down**.
* Agregaron un resistor entre **4040 Q0 (patita 9)** y la salida.
* Agregaron un resistor a cada salida de **jack switch**.
* Cambiaron las huellas de transistores a la versión **inline_wide** para aumentar el espacio disponible.
* Se agregaron **mounting holes** faltantes.

#### En PCB

* Actualizaron los conectores **jack** a la huella de la biblioteca para facilitar el ruteo de los nuevos resistores y evitar errores.

---

### g-02-sec-02-rev-a

#### En esquemático

* Agregaron resistores de protección en entradas y salidas.
* Se agregaron **mounting holes** faltantes.
