# sesion-10a
## Clase 120526

### pre-clase (teloneo mixto)

La clase de hoy fue distinta ya que el día anterior el edificio aledaño a nuestra facultad (república 180) se incendió dejando muchos daños y el establecimiento deshabilitado. 

En mi basta experiencia de clases online puedo decir que no me gustan para nada ya que me desconcentro muchísimo y este fue el caso, sé que tengo muchas cosas que hacer, me pongo a realizarlas y no prestar atención, entonces mi retención de esta clase no fue basta.

Primero comenzamos hablando sobre lo que había sucedido y que hicieron Aaron y Misaa en la semana de receso. Entre todo lo que conversamos, Misaa nos entregó un repositorio que llamó bastante mi atención porque anteriormente habíamos hablado sobre este mismo tema, bueno, fue unas “simples” 7 palabras, pero como mencione en mi bitácora anterior, resonaron tanto en mi que no deje de pensar en todo lo que hago. De hecho ahora cada vez que dejo que el algoritmo me recomienda cosas, siento que están vacías, a veces repetitivas que me aburren y termino viendo/escuchando algo que conozco pero sabiendo que tienen un riqueza detrás —sentimiento, pensamiento,pureza, etc—

https://github.com/misaaaaaa/multiples-musicas

“Pivotear en torno a productores y sellos”  “seguir sellos, en vez de música” ¿todo el peso de que te guste una canción es solo del artista que lo interpreta? es una muy buen apregunta, ya que el el/ella/elle es la cara visible, lo que tu ves y te gusta o te hace seguir escuchando, pero si es que te gusta tanto la forma en que está compuesta una canción/tema/pieza musical porque no seguir a las personas que estuvieron detrás de eso, ya que el artista que lo interpreta no siempre va a tocar el mismo estilo y a partir de esto, podrás descubrir más música fundamentada en tus gustos y volvemos al punto anterior, sin algoritmos que te quieren lavar el cerebro y que escuches las nuevas tendencias. Hay veces que yo escucho nuevas cosas porque sigo casas de diseño y me gusta mucho el trabajo detrás, otro tipo de algoritmo vivo.


### clase

- Misaa

En esta clase resolvimos dudas sobre kicad que se nos había solicitado la clase anterior.

- A → Herramienta agregar símbolo
- ESC → Herramienta selección
- M → Mover componentes
- G → Mover // con todo el entramado
- V → Asignar valor
- CMD + S / CTRL + S → Guardar
- E → Editar.
- F → Footprint.
- Ctrl + D → duplicar.
- R → rotar
- X → reflejo en eje X
- Y → reflejo en eje Y
- Alt + 3 → visor 3D
- F8 → actualizar espaciado en plano
- Botón verde → controlar planos



—•— → Sí hay conexión

—X → No conexión

✱ Agregar huellas a símbolos

→ Espacio que ocupa una huella en el espacio

→ Los espacios tienen incertidumbres.
 
F → Footprint.

Leds 5mm → típico 

Asignar a uno el footprint y después duplicar para no hacerlo todos uno tras uno.

Origen de 50 x 50. ← eje

Contorno es la placa.

Pistas → cables output (recorrido de neto)

terminal block.

✱ líneas aéreas → verificar orientación que está conectado a qué.

X → ruta.

Pista intermedia entre componentes.

Perno M3.

### imagenes de proceso

### post-clase

Después de tener esta clase remota, estuve pensando varias cosas

Por ejemplo, en una de nuestras clases, llegamos a una conversación sobre cómo era la carga del taller y nosotras sin argumentos dijimos que era poca, pero pensándolo bien, no creo que la carga académica de taller sea poca, si no que es la que corresponde y la que debe ser, pero a lo que nos quisimos referir era o por lo menos lo que pienso es que el taller es tan flexible a nuestros aprendizajes, que cada uno aprende a su ritmo. No debes tener todo de manera inmediata porque si no tu calificación es la mínima, si no que cumple esto en este periodo —que es un periodo bastante extenso para poder hacerlo a nuestro tiempo— y ahí será evaluado. 

En este minuto de mi vida estoy experimentando muchas cosas y esta es una de ellas, tengo muchos trabajos como diseñadora las cuales les estoy dando mucha importancia en mi vida porque son instancias que no pensé jamás tener en mi cuarto año de carrera —en este minuto me es relevante agradecer textualmente a Manuel Córdova y Ariel Altamirano por todo lo que me inculcaron el año pasado sobre mis gustos y cómo disfrutarlos y a esa lista se suman Misaa y Aaron— los primeros mencionados siempre me dieron mencionaron que les diera prioridad a esos divertimentos pero obviamente no ser irresponsable con la universidad, siempre cumplir con mis deberes. Ellos jamás me retuvieron por nada, como digo, ellos siempre me motivaron a más, trabajando ahora con uno de ellos.

¿A que voy con todo esto además de una pequeña reflexión?, es que a veces pienso que nada es de vida o muerte, todo tiene su tiempo y nadie aprende de la nada algo o no vamos todos al mismo ritmo. Entonces realmente prefiero hacer 1 cosa bien a 2 mal. Realmente yo entre a este taller porque conocía a Aaron y me acuerdo perfectamente cuando en primer año me invitó a su taller explícitamente porque me encontraba una persona motivada —me lo dijo textual— que él quería personas como yo en su taller, no sé si eso lo seguirá pensando, pero a mi mercaron sus palabras, pero estoy dispuesta aprender cosas nuevas a pesar de que esa fue mi razón por la cual estoy aquí ahora. 

(La verdad es que vengo a reflexionar de mi vida y las cosas que estoy haciendo, mi bitácora se ha convertido en eso ahora)

-----

- KICAD

Volví a instalar kicad ya que tenía muchos archivos deambulando entre la versión anterior y la nueva.

![kicad 1](imagenes/kicad_1.png)

Esta es la interfaz que nos presenta kicad cuando queremos iniciar un proyecto. 
1. El esquemático/símbolos es el *formato _sch*
2. El pcb es *formato _pcb*

Con estos dos formatos nos bastan ya que son los que utilizaremos, también puedes instalar plantillas. 

El formato kicad es kicad_pro.

El primer paso que debemos desarrollar es crear la partitura que nos guiará en todo nuestro proceso que es el esquemático, pero antes de ello será modificar nuestro espacio de trabajo a nuestro gusto o comodidad en preferencias>preferencias>ratón y panel táctil

Después de eso, comenzaremos a colocar símbolos. Con comando A pasaremos a la herramienta “símbolos”

En kicad se trabaja con una hoja técnica, muy típica —relacionado en el mundo del diseño— con lo que hacen los diseñadores industriales, la cual contiene un viñera y esa se puede modificar en la zona superior en la opción “configuración de esquema”.

Comenzaremos a colocar valores a nuestros símbolos con el comando “V”

En mi caso estaré realizando el clock (555) entonces mi primer paso será recolectar todos los símbolos necesarios para componerlo. Como quiero copiar uno ya realizado, quiero pegar una foto en el software, pero con la tecla eliminar no funciona para poder sacarlo después entonces apretando click derecho>eliminar

![kicad 3](imagenes/kicad_3.png)

esc > para eliminar si hiciste una conexión indeseada

Me aparecieron estos puntos naranjas 

![kicad 4](imagenes/kicad_4.png)

Debes acercar los símbolos que quieras conectar porque si no, estás haciendo cables sin ningún fin y no puedes arrastrarlos.

Yo sistematice que todo gnd y vcc estén en la misma altura para tener un límite y guía.  

Después escogí el secuenciador, los cuales tienen marcado los step y eso se llama Etiqueta de red (Net Label) la cual se realiza con el comando CTRL + L

![kicad 9](imagenes/kicad_9.png)

Ahora, apareció algo que no sé qué significa ya que fue automático: en 14 aparecio un triangulo y en 13 un círculo

![kicad 8](imagenes/kicad_8.png)

Teniendo el esquemático listo, empezaremos a realizar las huellas, en nuestro caso vamos a utilizar de la familia THT ya que son las que ocupamos. 

Existen dos formas, ir presionando cada uno de los símbolos y otorgarle una huella o ir al panel de “asignar huellas” que es una especie de excel para hacerlo una tras otra. También se podría desde un inicio, cuando seleccionas todos tus “ingredientes” designarles de inmediato a cada una su huella y así no tienes que ir una tras otra. 

Aquí hay que tener cuidado con no confundir los condensadores polarizados (u) y no polarizadores(n)

Terminando de designar huellas a símbolos, debemos pasar a PCB NEW

Una de las mayores dificultades que hay es que son muchos pasos por hacer y si en uno de estos te equivocas, puede “joderse” el proyecto, entonces eso me cuesta un poco. El aprendizaje que me llevo hasta este punto es que hay que fijarse mucho en cada cosa que hagas. 

*Por salud mental y bueno, porque me confundí en algunas cosas, el viernes quedé hasta aquí, pero quiero seguir trabajando después de clases.*

-----

*Soy de re-leer los textos y no había tenido la oportunidad de hacerlo el día anterior, así que lo hice en camino a la universidad.*

- HACIA UNA FILOSOFÍA DE LA FOTOGRAFÍA—VILÉM FLUSSER

Siempre antes de comenzar a leer un texto nuevo, se debe saber un poco de quien es el autor, ya que gracias a eso podemos saber cómo ve y aprecia el mundo:

Vilém Flusser fue un escritor, filósofo, pensador y periodista checo-brasileño con familia judía, pero viviendo casi todo el tiempo en Brasil. Él ha adquirido mucho significado para el estudio sobre el vínculo entre la cultura y las tecnologías, particularmente las tecnologías de la comunicación. De él recuerdo haber leído la filosofía del diseño en primer año junto a  Juaquin Zerene, me gustaría recordar más sobre ese texto. 

¨Hacia una filosofía de la fotografía” es una de sus grandes y reconocidas obras según los lectores que habla sobre la exploración innovadora de la intrincada relación entre imágenes, tecnología y existencia humana.

¿El ser humano es capaz de entender y apreciar el poder de imaginación que tiene? ¿La sociedad de hoy en día tiene más capacidad de generar imágenes, textos o ninguno?

La imagen inmortaliza lo que tenemos a nuestro alrededor, dejándolo a nuestra disposición cuando nosotros lo necesitemos sin tener que volver a ese lugar y así poder traer esa imaginación a otro espacio, compartirlo y comentarlo pero la comunicación de la imagen este se ve atropellada con el sentimiento e interpretación del que genera imágenes, osea teniendo así un lenguaje connotativo. 

