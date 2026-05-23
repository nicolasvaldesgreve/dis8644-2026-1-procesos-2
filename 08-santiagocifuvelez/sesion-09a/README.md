# sesion-09a

12 de mayo del 2026

¡Hola profe Aaron, Misa y Emi!, volvimos del holiday break, y es momento de refrescar y retomar lo ya aprendido en clase.
La clase de hoy fue un repaso + un agregado de súper valor…, Así que veamos que tenemos para hoy:

> Primeramente, siempre partimos con estos pasos en orden:  
>
> 1. Dibujar esquemático (.Kicad_sch)
> 2. Asociar huella a símbolos
> 3. Abrir PCB new (para crear la PCB), interprete del esquemático
> 4. Definir tamaño de las pistas
> 5. Repartir componentes físicamente
> 6. Rutear componentes
> 7. Ornamentar y exportar fabricación.

Ya con estos pasos en cuenta, continuemos con la clase:  

1. Como abrir archivos de trabajo.
2. Atajos de teclado.
3. La pcb (nuestra placa real)

## 1. Como abrir archivos de trabajo

Cuando un archivo ya está creado y guardado, se abre desde la extensión:
`.Kicad_pro`, ya que es todo el proyecto:

![kicadpreee](./imagenes/img1.png)

## 2. Atajos de teclado

|Tecla (atajo)|Lo que hace|
|-------------|-----------|
|**`A`**|Abrir tabla para agregar componentes |
| *Puedes buscar los símbolos que solemos usar +, así:* | `R = Resistors`  |
|                     |`C = Unpolarized capacitor`|  
|                     |`Gnd = Ground (tierra)`|  
|                     |`Vcc = Voltaje corriente continuo (Cielo)`|  
|                     |`NE555P = Chip 555` |
|                     |`R_pot = Potenciómetro`|  
|                     |`Led = Led`|  
|                     |`Battery_cell = Batería`|
|                     |`Speaker = parlante`  
|**`ESC (escape)`**| Para deseleccionar todo, y tener el cursor libre para seleccionar u hacer otras cosas.|
|**`R`**| Rotar componente 360. |
|**`X`**| Mirror componente en el eje X. |
|**`Y`**| Mirror componente en el eje y. |
|**`M (move)`**| Mover solo componentes sin cables (igualmente te aparecerá un warning cuando esto suceda). |
|**`G (grab)`**| Mover todo lo seleccionado con el mouse; aquí si se mueve todo lo que selecciones; cables, textos, etc. |
|**`E`**| Editamos el valor, y varias propiedades de un componente. |
|**`V`**| Podemos escribir/cambiar los valores a los componentes. |
|**`Ctrl + S`**| **Save (SIEMPRE HACER CTRL + S).** |
|**`Ctrl + D`**| Duplicar |
**`Ctrl + Z`**| Volver atrás  |

> *Antes de pasar a la placa PCB, debemos dejar en claro las “Huellas” (footprints); pues estas son prácticamente el sentido de vida de nuestras placas, ya que ellas son el estado físico, real, y tangible de nuestros componentes en la vida real.*

> *Entonces, primeramente, siempre asegurarnos de las medidas de nuestros componentes y ponerlos en coherencia con el que corresponda.*

## 3. La pcb (nuestra placa real)

**Primeramente, know your grids (grillas), vamos a usar 5mm para nuestras placas, ya que es un grosor perfecto.**
![img2](./imagenes/img2.png)

 **Además, siempre se debe hacer los contornos de las placas, en la capa de edges.cuts:**
![img3](./imagenes/img3.png)

**Listo, ahora que ya hicimos el contorno de nuestra placa, sigue definir los caminos de conexiones (las pistas):**
![img4](./imagenes/img4.png)

En Kicad, puedes escoger el tamaño de las pistas para que fluya más o menos energía por ciertos caminos.  
Antes de continuar, quiero hacer mención de que hay posibilidades muy específicas con las que podemos trabajar: Por ejemplo, la capacidad mínima de pista, es de 0.10mm / 0.10mm (4 / 4 mil). En kicad se puede hacer de menos, pero al momento de esta ser realizada en china, no la van a leer.

También existe un espaciado mínimo entre pistas, para que no se toquen las unas con las otras.
(En cualquier caso, más de 0.3mm es lo mejor).

**Para hacer las pistas, las encontramos aquí:**  
![img5](./imagenes/img5.png)

**Luego se nos despliega esto, y aquí podemos poner las anchuras de nuestras pistas. Ya luego de eso, nos van a aparecer como “pinceles”, con las anchuras que hicimos.**  
![img6](./imagenes/img6.png)

**Y primero, comenzamos a organizar los componentes en el contorno que creamos:**  
![img7](./imagenes/img7.png)

**Luego de haber organizado los componentes en la placa, podemos hacer nuestras pistas, en estas dos capas: `F.cu` (front). y `B.cu` (back)**  
![img8](./imagenes/img8.png)

**Luego le hundimos enrutar pista única (o podemos oprimir la letra x):**
![img9](./imagenes/img9.png)

**Luego, cuando le hundimos nos aparecen todos los lugares donde debería ir conectado ciertas pistas:**  
![img10](./imagenes/img10.png)

**Una vez ya conectados todos los positivos, vamos a ver una manera de como conectar los negativos:**  
![img11](./imagenes/img11.png)

**Vamos a esta herramienta:**  
![img12](./imagenes/img12.png)

**Hacemos click en cualquier parte de la pantalla y se nos va a desplegar este menú, y allí seleccionamos ambas caras de las placas: Front y Back, y luego en red, seleccionamos: GND:**  
![img13](./imagenes/img13.png)

**Luego le hundimos aceptar, y hacemos el contorno alrededor de la placa, y hay que ser muy cuidadoses en cerrar bien el contorno; y se vería algo así:**  
![img14](./imagenes/img14.png)

**Luego hundimos la letra `B`, se rellena todo:**  
![img15](./imagenes/img15.png)

**Aquí ya tenemos todos los GND conectados, ahora vamos a ver si hay algún error, o si algo no está conectado:**  
![img16](./imagenes/img16.png)

**Vamos allí, y luego le hundimos “ejecutar DRC”, para evaluar que todo está bien.**  
![img17](./imagenes/img17.png)

En este caso todo está bien. Period

Ahora, vamos a abrir unos huequitos para poder integrar nuestra PCB a la superficie.

**Para esto, vamos a nuestro archivo del esquema (SCH)  para a buscar `MountingHole`, que sería nuestro hoyito de montaje, y luego ese lo traemos a nuestro archivo de la PCB.  
*(recordar asignar huellas, etc.):***  
![img18](./imagenes/img18.png)

**Listo:**  
![img19](./imagenes/img19.png)

**Y ya está.**  
![img20](./imagenes/img20.png)

Para este corte del semestre vamos a leer un libro llamado; “Hacia una filosofía de la fotografía”, y para esta bitácora, leeremos el primer capítulo del libro, el cual se llama:

1.	La imagen.  
Antes de entrar en materia con el capítulo como tal, vamos a hablar primeramente de la presentación del libro y la introducción; El autor hace este libro como objeto de reflexión sobre la tecnología y su permeancia en la sociedad en la actualidad, pues la tecnología se ha encargado de crear una realidad no real, donde todo se disfraza, y se alinea a lo que nos gusta, por eso el autor hace mención sobre la coerción de libertad (generada por la determinación que la tecnología nos impone), en realidad…¿Lo que nos gusta, nos gusta?, o ¿Es lo que le gusta al algoritmo que nos guste?

A esto el autor hace una división en la línea del tiempo hasta la actualidad, en la cual menciona que las historias de la sociedad se han experimentado dos momentos fundamentales desde su comienzo; “La invención de la escritura lineal” (alrededor de la última mitad del segundo milenio a. de C. El segundo (del cual somos testigos) “La invención de las imágenes técnicas”. Lo anteriormente mencionado, lo debemos tener en cuenta para el resto de la lectura.

También un warning súper fundamental, es que este libro es un ensayo hipotético. Ahora sí, con lo anteriormente mencionado, comencemos en materia con el capítulo 1.

El capítulo 1, titulado “La imagen”, hace una serie de comparaciones; Imagen técnica (obtenida de las cámaras) e imagen imaginaria (nuestra imagen mental); Textos lineales (o textos escritos) e imágenes; La mediación entre la escritura y el hombre; La mediación entre la imagen y el hombre…, entre otras.

Como menciona el autor, las imágenes son el significado de algo “exterior”, y tienen como propósito hacer ese algo exterior en algo “imaginable” para otrxs (eso en cuanto a la imagen técnica). Pero también está la imagen mental que realizamos con nuestros ojos y re-proyectamos en nuestra mente, eso dándole paso al “imaginario”. Y aquí es donde el autor interrumpe y hace su reflexión, pues las imágenes son susceptibles a la interpretación propia del ser humano, son un conjunto de símbolos connotativos. Esto a su vez se complementa con que, gracias a este ejercicio de remembranza, y decodificación, todas las relaciones que hacemos en este momento entre objetos, espacio-tiempo, todo tiene una relación, y a cambio de esas relaciones obtenemos un significado. Y Aquí el autor hace un llamado, pues “es un error descifrar las imágenes como si fueran eventos congelados”. Por el contrario, las imágenes son traducciones de hechos a situaciones; éstas sustituyen con escenas los hechos”.

También, el autor menciona que las imágenes tienen la finalidad de hacer que el mundo sea más entendible y/o accesible e imaginable a través de las imágenes, pero allí existe un problema que lo contradice, pues el hombre viviría en función de las imágenes y de sus perspectivas de lo que se creería que es la realidad por las imágenes (que pretenden ser la realidad, pero no lo es). O sea, ya no se descifra ni se descubre más el mundo tangible/real, y esto lleva a que se proyecte al mundo exterior sin haberlo conocido, o como dice el autor “sin descifrarlo”.

Hay muchísima reflexión alrededor de este capítulo, Dios mío, pero para no hacerlo más largo, vamos a pasar a una de las contradicciones de las cuales el autor hizo mucho énfasis, y fue la lucha entre “texto lineal” e “imagen”, pero al final…, se terminan complementando la una la otra. 

Reverse colonization. 

