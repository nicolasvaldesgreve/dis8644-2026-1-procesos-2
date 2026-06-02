# sesion-11a

# Apuntes 26/05

Durante clases nos seguimos dedicando a trabajar en el proyecto 02 por lo que nos dedicamos a resolver el circuito de la opción 01, ya que trabajamos en éste el lunes 25 durante la mañana y logramos que funcionara, pero por alguna razón llegaba a un punto en el que dejaba de prender los LEDs y esto se solucionaba desconectando el cable que estaba en el ``reset`` del 4017, dejarlo interactuar con el aire por unos segundos y volver a conectarlo (o dejarlo en el aire) en donde debía ir XD no entendimos por qué sucedía esto y preferimos guardar las preguntas para la clase de hoy.

![Cable tomando su break para respirar](./imagenes/cable-respirando.png)

Antes de explicar la situación, Misa nos revisó el circuito y nos hizo las siguientes correcciones:

+ Añadir un capacitor de 100μF en el ``pin 5`` del chip 555
+ Arreglar la conexión entre el chip 555 y 4017, ya que estábamos utilizando el ``pin 3`` del 555 como salida y el ``pin 13`` del 4017 como entrada, siendo que tenemos que utilizar el ``pin 14`` del 4017 en vez del 13.
+ Unir el ``pin 13`` del 4017 a tierra mediante una resistencia de 100k

Luego de hacer estos cambios, el esquemático quedó de la siguiente manera:

![Esquemático actualizado](./imagenes/piezov03.jpg)

Con estos cambios el primer circuito quedó funcionando en la protoboard, por lo que nos dividimos el trabajo con nuestros compañeros y mientras unos armaban en la protoboard el segundo circuito, yo hacía cambios en esquemáticos y armaba la pcb. Luego de terminar de hacer esto, nos dimos cuenta que el segundo circuito no estaba respondiendo, pero no pudimos seguir trabajando ya que Misa y Aarón empezaron a presentar a la clase el nuevo estándar, el cual es el siguiente:

![Estándar hecho por les profesores, no me pertenece](./imagenes/estandar.png)

También nos dieron una lista de huellas estándar!! la pueden encontrar dentro de ``dis8644-2026-1-procesos-2/00-proyecto-02
/estandares.md`` o haciendo click en el siguiente link: <https://github.com/nicolasvaldesgreve/dis8644-2026-1-procesos-2/blob/main/00-proyecto-02/estandares.md>. De igual manera, aquí dejo un screenshot de la tabla:

![Huellas para todos!! aporte de Misa](./imagenes/huellas.png)

---

## Capítulo 8 y 9 - Hacia una filosofía de la fotografía, Flusser

En el inicio del capítulo 8 dice "Este cambio constante es precisamente lo que se nos ha hecho habitual: una fotografía redundante remplaza otra fotografía redundante. El cambio mismo es el que se ha hecho habitual y redundante; y es el "progreso" mismo el que se ha vuelto desinformativo y ordinario", ¿esto se refiere a los contenidos que consumimos actualmente en redes sociales? probablemente entendí todo mal, pero por alguna razón mi cerebro al leer esta parte me tiró un mensaje diciendo "jaja como el contenido de reels" lo cual me causó un poco de gracia.

- Imagen implica magia
- Aparato implica automatización y juego
- Programa implica necesidad
- Casualidad e información implica símbolo e improbabilidad

Me gustó como en el último capítulo Flusser hace un resumen con palabras súper sencillas de lo que se habló durante todo el libro, ya que al ser algo más corto y con palabras que si logro comprender se me hace más fácil entender de lo que se estuvo hablando. El cómo justifica la necesidad de una filosofía de la fotografía me hace bastante sentido, cosa que puedo decir que al inicio de la lectura del libro no estaba taaan convencido ya que como mencioné en una bitácora anterior, nunca me detuve a pensar tanto en el concepto de libertad mediante una cámara y la fotografía en si ya que no me asocio mucho con la actividad de fotografiar en si (veo fotos constantemente, si, pero casi nunca soy yo el que está detrás de ese trabajo).

#### Vocabulario

+ Democriteano: Hace referencia a los principios establecidos por Demócrito, centrándose en el atomismo materialista.
+ Biunívoca: Que se establece entre los elementos de dos conjuntos cuando, a cada elemento de un conjunto, le corresponde uno y solo uno de los elementos del otro, y viceversa

Fuentes:

+ <https://www.filosofia.org/enc/fer/materia2.htm>
+ <https://www.rae.es/diccionario-estudiante/biun%C3%ADvoco>
