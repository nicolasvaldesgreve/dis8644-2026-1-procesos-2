# sesion-10a
## 19, May
### Apuntes
Esta clase fue muy dinamica e hicimos muchas 

Elian radigue - kyema

(drone): El estilo de música drone se caracteriza por el uso de sonidos sostenidos y repetitivos, creando una atmósfera constante y envolvente. Estos sonidos, llamados "drones", pueden ser producidos por instrumentos acústicos, electrónicos o una combinación de ambos.

**Apuntes capitulos del libro de Flusser**

1)imagen= prehistórico = mundo (mito) 

2)imagen técnica = poshistórico = "literal"

3)los aparatos 
+ herramienta: extensión del cuerpo ocupaba objetos culturales (chinchineo)
+ maquina: la herramientas eran variables y después de la revolución industrial fue al revés
estas dos se unen por el trabajo
+ aparato en la capara lo que entra (input) es la acciona de apretar el botón y lo que sale es la imagen (output)  las cámaras están reguladas por las empresas pero las empresas están reguladas por el mundo el capitalismo (el programa) es un circulo vicioso.

"investigar dentro de la caja para salir del programa" 

### Notas de la charla for want of (not) measuring
En español por querer (no) medir

#### Jim Hobbs: La Grilla, el Proyecto de Medición y el Archivo Colectivo

* **Origen de la grilla:** La idea de trabajar con la "grilla" o cuadrícula surge gracias al trabajo de su padre.
* **La tensión de la estructura:** La cuadrícula se entiende como un espacio estructurado donde se pueden contener y ordenar muchas cosas; sin embargo, dentro de esa misma idea estructural rígida también habita una constante inestabilidad.  
* **Exposición expandida y colaborativa:** En su proyecto sobre la medición, el interés principal era que la exposición no se limitara a la perspectiva de ellos dos, sino que se expandiera orgánicamente hacia otros artistas, comunidades y culturas. 
* **Un proyecto mutante:** La exposición cambia por completo dependiendo del lugar físico al que se traslada; cada montaje es una versión completamente nueva y adaptada del proyecto original. 
* **Redefiniendo la publicación:** Investigan activamente qué significa realmente una "publicación". La idea es que cada una de ellas sea diferente a la anterior.  
* **El archivo como propuesta artística:** Lo que construyen en el tiempo es un gran archivo del proyecto que conecta las ideas de otros creadores y curadores. Cada publicación final es única y constituye una propuesta artística en sí misma. El valor fundamental para ellos radica en generar conexiones significativas entre artistas, curadores y diferentes culturas.

#### Simon: Escaneo 3D, Escalas del Tiempo y Tecnología

* **La nube de puntos (Tecnología LiDAR):** Explicó el funcionamiento de un escáner que posee un vidrio giratorio multiaxis. Este dispositivo lanza millones de puntos láser hacia el entorno físico que, al rebotar y devolverse, generan una imagen tridimensional detallada del espacio conocida técnicamente como una *nube de puntos*.
* **La flexibilidad de lo vivo:** Al escanear los árboles, recuerdan que estos son seres vivos. Aunque visualmente los percibamos como estructuras sólidas y estáticas, en el escaneo digital se revela su flexibilidad y movimiento a través de una compleja malla tridimensional.
* **Un asunto de escalas y tiempo:** El tiempo y la velocidad son relativos. Para nuestra escala humana, el árbol se mueve muy lento; pero para la escala del árbol, los humanos nos movemos demasiado rápido. A su vez, para la escala temporal de una montaña, el árbol es el que resulta extremadamente rápido y efímero.
* **Magia y tecnología:** Se rescata la célebre frase de Arthur C. Clarke: *"La tecnología, en un punto avanzado de su desarrollo, no se distingue de la magia"*.
* **El arte más allá de la medición:** Es muy divertido cuando una herramienta tecnológica (como un escáner industrial) se deja de utilizar únicamente para medir con fines científicos y se empieza a usar de forma creativa; ahí es donde realmente comienza lo interesante.
* **Herramientas a la mano (Polycam):** Mencionó aplicaciones accesibles como *Polycam*, que utilizan los sensores de nuestros teléfonos inteligentes para permitirnos experimentar y capturar el mundo en mallas 3D por nosotros mismos.
* **La belleza del fallo:** Todos interactuamos y usamos las tecnologías de maneras muy diferentes, pero el momento en que un dispositivo o un sistema se rompe, falla o se "glitchea" es cuando se vuelve verdaderamente interesante para la exploración artística.
---

### Apuntes de Clase: Chips, Osciladores y Control de Voltaje
despues en la clase missa hablo de los chips y de cuales podrian funcionar para cada grupo en nuestro caso osciladores 

**CD4093 (Oscilador por Resistencia):**

* Es como una caja negra que convierte el valor de una resistencia en una frecuencia (sonido/tono).
* Para cambiar el tono podemos conectarle distintos tipos de resistencia en el circuito: una fotorresistencia (**LDR**) que reacciona a la luz, un potenciómetro (**pot**) para moverlo con una perilla, o una **resistencia fija** si queremos un tono estático. Básicamente: más resistencia = oscilación más lenta; menos resistencia = oscilación más rápida.

**Control de Voltaje (CV) y Divisor de Voltaje:**

* **CV (Control de Voltaje):** Es el lienzo en blanco para la síntesis musical. En lugar de mover perillas con la mano, usamos electricidad (voltaje) para controlar los parámetros de los chips de forma automática.
* **Divisor de Voltaje:** Es un circuito simple que nos ayuda a modular un voltaje alto de entrada ($V_{input}$) y transformarlo en un voltaje menor de salida ($V_{output}$) que podamos controlar de forma segura.

**IC PLL 4046 (Convertidor de Voltaje a Frecuencia):**

* Este chip funciona al revés del 4093: convierte directamente el **voltaje en frecuencia**.
* Si le tiras un voltaje alto, el chip va a reaccionar entregando una frecuencia rápida (un tono muy agudo). Si le tiras un voltaje bajo, tendrá una frecuencia lenta (un tono grave o pulsos lentos).
* **El camino de la señal en el protoboard:** Primero generas un voltaje desde la fuente o batería ➝ ese voltaje pasa por el potenciómetro o divisor para poder regularlo manualmente ➝ el voltaje regulado entra al pin de control del **CD4046** ➝ el chip convierte ese voltaje en frecuencia, haciendo variar el tono del parlante según la cantidad de corriente que dejes pasar.

**VCO (Oscilador Controlado por Voltaje):**

* Significa *Voltage Controlled Oscillator*. Es un oscilador que no depende de que cambies una resistencia física, sino de los cambios de voltaje que le inyectas para generar ondas y notas musicales.

