# sesion-09b

# Apuntes clase 15/05

Esta clase se dedicó para resolver todo tipo de dudas que se nos hayan generado en el proceso del encargo anterior el cual fue armar dos PCB dentro de KiCad en base a nuestros sintetizadores. Como se abordaron dudas de todo tipo, esta bitácora será un punteo de cosas que no sabía y me alegro de que se hayan mencionado:

### 1- Huella con tamaño predeterminado para chips

Al momento de asignar huellas, siempre usaremos la siguiente "base" para encontrarlas: ``dip-(cant. de pins) W (ancho) 7.62 - long pads``, el que sea "long pads" no es obligatorio pero es lo ideal ya que esto nos ayudará a que sea más fácil el soldado de la pieza. Aquí un ejemplo de la huella en el símbolo del chip NE555P:

![Huella longpads en 555](./imagenes/longpads-555.png)

### 2- Cómo editar un símbolo en el esquemático

Esta fue mi duda, ya que en el caso del chip 555 el pin 5 que va directo a GND está en la parte superior del chip, lo cual me molestaba ya que es más simple si todos los pins que van directo a GND se mantienen abajo.

Para poder editar el símbolo, tenemos que seleccionarlo dentro del esquemático y presionar la tecla ``E`` para poder ver las propiedades del símbolo. Una vez nos aparezca la ventana de propiedades, tenemos que seleccionar la opción de ``Editar símbolo`` y **NINGUNA OTRA OPCIÓN!!** ya que podemos dañar archivos de KiCad y llevarnos la pala (quedaría la pura escoba.. perdón).

![Opciones dentro de las propiedades](./imagenes/editar-simbolo.png)

Una vez ya estemos dentro del editor de símbolos, podemos mover los pines como queramos, añadir más, cambiar el color del símbolo, cambiar los textos, etc. Cuando ya tengamos todo modificado, tenemos que guardar y listo!! 

### 3- Agregar modelos 3D de componentes que no tenga KiCad

Como en el render del modelo 3D de la PCB no se ven los modelos del potenciómetro ni de los terminal blocks, tenemos que añadirlos a mano por lo que Misa envió por discord el archivo ``.step`` de los modelos ya que KiCad funciona principalmente con archivos ``.step``.

Una vez ya tengamos el archivo descargado, tenemos que abrir el visualizador de la pcb (archivo ``.kicad_pcb``), seleccionamos el componente al que le queremos asignar el modelo 3D y apretamos la tecla ``E`` para poder ver las propiedades de este componente. Cuando ya estemos en la ventana de propiedades, tenemos que cambiarnos a la sección llamada ``Modelo 3D`` que se encuentra en la parte superior.

![Cambiar de sección](./imagenes/modelo-3d.png)

Una vez ya estemos en la sección del modelo 3d podemos ver que nos aparece una opción para cambiar la ruta del modelo del componente, en donde tenemos que hacer click y actualizarlo a la ruta del modelo que acabamos de descargar (en mi caso es el que sale en pantalla).

![Cambiar ruta del modelo](./imagenes/ruta.png)

Cuando ya hayamos agregado la ruta, nos va a aparecer el modelo en el visualizador que tenemos en la ventana. Ahora lo único que queda es encajar el modelo dentro de los espacios que tiene la PCB!! para ésto tenemos que ir modificando las variantes de ``Rotación`` y ``Desfase``.

![Modelo ya encajado](./imagenes/ajuste.png)
