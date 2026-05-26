# Sesión 10a - martes 19 mayo 2026

Esta sesión tuvo dos partes muy distintas, una charla en el auditorio con artistas invitados y después un repaso técnico de chips con el profe. Las dos me gustaron por razones distintas.

---

### Charla en el auditorio / Jim, Patrick y Simon

Micrófono, era un escáner LiDAR (Light Detection and Ranging), lo que más me voló la cabeza es que nos mostraron el modelo 3D de una flor que hicieron con ese escáner. No era solo la forma, tenía los colores reales, los pétalos, todo el detalle. Tenía un poco de transparencia, pero creo que es porque los puntos no cubren completamente el interior, el láser solo captura la superficie exterior donde rebota, así que el interior queda vacío. Igual se veía increíble, nunca había visto algo así.

---

### Apuntes técnicos / chips para el proyecto

Después de la charla, el profe repasó los chips que podríamos usar para nuestros proyectos. Como grupo de filtros, lo que más nos interesó fue el **TL072** y el **LM358**. 

Chips que nos sirven para el Proyecto de Filtros

Para nuestro segundo proyecto de filtros, no nos sirve cualquier cosa. Necesitamos Amplificadores Operacionales (Op-Amps), que son los que realmente hacen la magia de "limpiar" la señal o dejar pasar solo las frecuencias que queremos. Estuve viendo estas opciones:

* **TL072 / TL082:** Son súper baratos y fáciles de encontrar. Lo mejor es que tienen "bajo ruido", así que si hacemos un filtro de sonido, no se va a escuchar ese siseo molesto de fondo. El TL072 tiene dos operacionales adentro, así que nos ahorramos espacio en la placa.
* **LM324:** Trae cuatro operacionales en un solo chip. Si nuestro filtro es muy complejo (tipo un filtro de cuarto orden que necesita varias etapas), este nos salva la vida porque metemos todo en un solo integrado.
* **NE5532:** Si nos queremos poner realmente pro y el presupuesto da, este es de "grado audiófilo". Es el que usan en las mesas de mezcla caras.
* **LM358:** Es el más básico de todos. Consume súper poca batería, así que si queremos que nuestro filtro sea portátil y funcione con una pila de 9V por mucho tiempo, esta es la opción segura.

---

### Lo que me llevo de hoy

Me quedó dando vueltas lo del escáner de Simon, me hizo un clic con lo que vemos en electrónica. Al final, cada punto que marca el láser es como un dato más que el sistema tiene que procesar, igualito a como funcionan los sensores que usamos, solo que con una precisión que te vuela la cabeza..

Para el proyecto de filtros, estuve dándole vueltas a qué chip usar y sigo convencida de que el TL072 es la mejor opción. Como queremos que el audio se escuche limpio y sin ese ruido de fondo tan pesado, ese chip es ideal. Ahora, si vemos que el presupuesto se nos va o que necesitamos que la batería dure mil años, el LM358 es el plan B perfecto porque consume súper poco.

---

### Referencias

- [Polycam — app de escaneo 3D](https://poly.cam)
- [TL072 — datasheet y aplicaciones](https://www.ti.com/lit/ds/symlink/tl072.pdf)
- [LM358 — características y usos](https://wraycastle.com/es/blogs/knowledge-base/lm358-pinout)
- [LM324 — amplificador operacional cuádruple](https://www.ti.com/lit/ds/symlink/lm324.pdf)

