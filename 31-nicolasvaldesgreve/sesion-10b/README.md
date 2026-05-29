# sesion-10b

# Apuntes clase 22/05

Durante esta clase nos dedicamos a trabajar de manera grupal en lo que haríamos para el proyecto 02, por lo que nos juntamos con mi grupo de trabajo (grupo 01 - piezo) y repasamos nuevamente las ideas que habíamos hablado durante la clase anterior.

Para contextualizar, en el proyecto 02 se nos indicó crear grupos de 5 personas para que cada grupo se encargue de una de las siguientes opciones:

1. Piezo
2. Secuenciador
3. Oscilador (1)
4. Oscilador (2)
5. Filtro
6. Percusión

Cada grupo debe entregar dos módulos distintos incluyendo el esquemático, pcb y una prueba de que funcionan en protoboard, por lo que con mi grupo tuvimos las siguientes ideas:

#### Opción 1

Utilizar el piezo como entrada con pequeños golpes utilizando como referente al juego "Taiko no Tatsujin", el cual es un juego rítmico en donde tienes que golpear un tambor taiko (tambor tradicional japonés) al ritmo de la música. Como primera idea queríamos que con cada golpe en el piezo se permita el paso de uno de los steps del 4017, pero como decisión final quedamos en que preferiamos que con un golpe se forme un loop de uno de los steps y que éste se apague dando otro golpe en el piezo.

![Imagen del juego Taiko, rescatado de página de Nintendo](./imagenes/taiko.png)

#### Opción 2

Utilizar el piezo como entrada pero que este responda a las vibraciones que uno puede generar en la garganta, por lo que necesitamos que el piezo se encuentre pegado a la piel lo cual queremos lograr al usarlo como un collar del estilo choker. Al inicio pensamos que se podría hacer con las pcb flexibles, pero en este caso no lo podremos hacer ya que tenemos que utilizar las placas sólidas al igual que el resto de nuestros compañeros.

![PCB flexible, rescatada de <https://www.viasion.com/es/blog/what-is-flexible-pcba-advantages-and-processes/>](./imagenes/pcb-flexible.png)

Como no podemos hacer la placa flexible, decidimos alargar la conexión del piezo para que este se pueda utilizar en el cuello siendo afirmado por un collar tipo choker que se hará aparte. En esta opción lo que permitirá el paso es la vibración que se provocará en el piezo con la garganta del usuario.

Para poder tener algo en lo que podamos basarnos, Misa nos entregó esquemáticos en base a lo que queríamos lograr y nos pusimos a trabajar en lo que sería la pcb. Para poder distribuirnos el trabajo, unos compañeros se encargaron de hacer el esquemático de cada opción y otros nos encargamos de asignar huellas y darle forma a la PCB dentro de KiCad. Este fue el resultado de mi aporte:

![Parte trasera de la PCB](./imagenes/pcb-back.png)

![Parte frontal de la PCB](./imagenes/pcb-front.png)

---

## Capítulo 6 y 7 - Hacia una filosofía de la fotografía, Flusser

+ La información tiende a desintegrarse progresivamente de acuerdo con el segundo principio de la termodinámica, pero el ser humano se distingue de esto ya que adquiere, almacena y transmite información al mismo tiempo que la produce de manera intencional; a esto se le llama "espíritu", que es lo que produce "cultura" (objetos informados).
+ El proceso de manipulación de información (comunicación) tiene dos fases: el _diálogo_, que es en donde se produce la información y el _discurso_ que es como se distribuye la información.

Es decir que como el humano transmite información y eso es lo genera cultura, actualmente en el mundo de las redes sociales se está dejando de lado el verdadero propósito de la comunicación, ya que como todos sabemos dentro de estas aplicaciones, en efecto, se nos muestra una cantidad absurda de información por minuto pero no del tipo que nos hace pensar ni generar cultura, sino que son mayoritariamente contenido basura que de igual manera se nos hace atractivo y nos mantiene haciendo doomscrolling (o tal vez hablo por mí mismo XD)

#### Métodos de discurso:

Por lo que dice, asumo que nos quiere decir que dependiendo de la manera en la que se da el discurso puede variar como entendemos o como reaccionamos al mensaje

1. Situación cultural de "responsabilidad": El emisor está rodeado de receptores que formar un semicírculo.
2. Situación de "autoridad": El emisor utiliza transmisores o "auxiliares" como en la comunicación militar de un rango a otro.
3. Situación de "progreso": El emisor distribuye su información en forma de diálogos que la enriquecen con información nueva antes de transmitirla, como un discurso científico.
4. Situación de "manifestación": El emisor envía su información al espacio vacío, como en la comunicación por radio _(aquí aplica la distribución de fotografías)_.

#### Canales de información

Toda información se puede situar en tres categorías: en información indicativa "A es A", información imperativa "A debe ser A" o en información optativa "deja que A sea A" y las formas ideales de estas opciones son la "verdad", la "bondad" y la "belleza" en el mismo orden.

1. Canales para fotografías supuestamente indicativas: publicaciones científicas, noticias.
2. Canales para fotografías supuestamente imperativas: carteles para publicidad ya sea política o comercial.
3. Canales para fotografías supuestamente optativas (fotografías artísticas): galerías, revistas de arte.

+ "Sin embargo, quien sabe tomar fotografías no necesariamente sabe cómo descifrarlas."

---

## Visita a CEINA - For Want Of (Not) Measuring

> Todas las imagenes que se muestran a continuación fueron tomadas en el Centro Cultural CEINA, lugar en donde se presentaron las obras.

El sábado 23 fuimos al CEINA con unos compañeros a ver la exposición "For Want Of (Not) Measuring", la cual estaba bajo la curatoría de Joselyne Contreras y Jorge Cabieses-Valdés y estaba ubicada en la sala expo 1 de CEINA

![Fotografía del montaje en CEINA](./imagenes/ceina-1.jpg)

![Fotografía del montaje en CEINA](./imagenes/ceina-2.jpg)

En el lugar de la exposición también estaban estas imagenes que muestran las texturas de los árboles, lo cual me gustó como se relacionaba con las otras demostraciones ya que la mayoría eran scans de plantas y naturaleza!

![Imagenes de texturas de árboles](./imagenes/texturas-arboles.jpg)

Al recorrer el lugar no me había dado cuenta de que al fondo de la sala habían dos pantallas que mostraban dos modelos 3D de scaneos distintos, en donde podías interactuar con estos mediante los botones que estaban pegados al vidrio, lo que te permitía hacer zoom-in, zoom-out y moverte al rededor del modelo. Uno estaba completamente funcional, mientras que el otro se despegó:(

![Modelo 3D en pantalla, interactivo](./imagenes/modelo-interactivo.jpg)

![Segundo modelo 3D en pantalla, también interactivo](./imagenes/modelo-interactivo-caido.jpg) 
