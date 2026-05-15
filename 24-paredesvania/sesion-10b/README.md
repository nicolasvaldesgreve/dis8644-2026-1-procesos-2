# sesion- 15.05.26
## Símbolos
Para modificar/personalizar nuestros símbolos, lo seleccionamos, apretamos la "e" y seleccionamos "edit symbol" para editar sus propiedades específicas.

Si queremos nuestra propia biblioteca de símbolos, primero debemos crear una carpeta en donde deben estar guardadas, para eso primero nos vamos a "Symbol Editor" en nuestra carpeta con extensión ".pro"

![pantallazo](./imagenes/editsymbol.png)

luego en el panel de arriba nos vamos a view/panels/library tree

![pantallazo](./imagenes/panels.png)

Con las bibliotecas activadas nos vamos a file/new library para crear nuestra carpeta que deberá aparecer una vez guardada en la lista de libraries, así que voy al componente que quiero personalizar, lo copio y lo pego en el nombre de mi carpeta, lo edito y guardo.

![pantallazo](./imagenes/micarpeta.png)

[`Las imágenes nos confunden de la realidad, ¿quién soy yo?, limitan nuestra imaginación.`]

### Botones:
**temporales**
  * pulsadores
  * timbres
  * pushbuttons
  * no-abierto
  * nc-conectado

**Interruptores**
  * palanca
  * switch

> Para encontrar el interruptor, buscamos SW_SPST o ST_SPDT y le ponemos la huella Button_switch de 6mm

### Etiquetas
Conectar sin cableado en el esquemático

* Para activarlo ocupamos la "L" de Label.

La podemos usar para evitar el error de pin no conectado a la salida, debemos conectar desde la bateria y al output la etiqueta "PWG_FLAG".
