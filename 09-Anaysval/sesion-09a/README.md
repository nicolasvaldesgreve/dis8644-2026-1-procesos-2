# sesion-09a

Martes 12 de mayo de 2026

La clase fue online debido al incendio.

- Continuación de aprendizaje en KiCAD.

### Atajos importantes

| Tecla        | Función                                         |
|--------------|-------------------------------------------------|
| A            | Agregar componente                              |
| R            | Girar componente                                |
| G            | Mover componente manteniendo cables             |
| M            | Mover componente libremente                     |
| E            | Editar propiedades                              |
| V            | Cambiar valor o cambiar de capa                 |
| Esc          | Volver al modo selección                        |
| Cmd + D      | Duplicar                                        |
| Cmd + Z      | Deshacer                                        |
| Option + 3   | Abrir vista 3D                                 |

### ꩜ Paso 4 — Definir pistas

En esta parte comenzamos a trabajar con las pistas de cobre de la PCB. Primero aprendimos que no todas las conexiones usan el mismo grosor, ya que depende de la corriente que pasa por ellas.

| Tipo de pista            | Medida  |
|-------------------------|---------|
| Alimentación (VCC)      | 0.8 mm  |
| Conexiones normales     | 0.4 mm  |

Las pistas más gruesas se usaron para la alimentación y las más delgadas para señales entre componentes.

### Contorno de la PCB

Antes de ordenar los componentes, se crea el borde de la placa.

#### Procedimiento

- Seleccionar la capa Edge.Cuts
- Dibujar un rectángulo
- Ajustar tamaño haciendo doble clic
- Redondear esquinas
  
Métodos para redondear esquinas

| Método                 | Descripción                         |
|----------------------|-------------------------------------|
| Herramienta arco     | Elegir centro, inicio y final       |
| Rectángulo redondeado| Configurar radio de 5 mm            |

El contorno siempre debe dibujarse en Edge.Cuts, ya que hacerlo en otra capa genera errores.
### ꩜ Paso 5 — Distribuir componentes

Después de definir las pistas, organizamos los componentes dentro del contorno de la PCB.

Para esto se toma en cuenta:

- Mantener un diseño ordenado
- Dejar espacio entre componentes
- Facilitar las conexiones
- Mantener todos los componentes orientados correctamente

Además, se recomienda revisar constantemente el visor 3D para ver cómo se verá físicamente la placa.

### ꩜ Paso 6 — Rutear conexiones

En esta etapa se realizaron las conexiones entre componentes utilizando pistas de cobre. Primero se hicieron las conexiones de alimentación con pistas de 0.8 mm y luego las señales normales con pistas de 0.4 mm.

Cuando las pistas se cruzaban y no podían pasar por el mismo lugar en la misma capa, se utilizaron vías para cambiar hacia la cara trasera de la PCB.

### Uso de vías

Las vías permiten conectar la capa frontal y trasera de la placa.

Para utilizarlas se debía:

- Dibujar la pista normalmente
- Presionar la tecla V
- Crear la vía automáticamente
- Continuar el trazado en la otra capa

### GND

Para las conexiones de tierra no se trabajó pista por pista.

En cambio, se creó un plano de cobre GND ocupando gran parte de la PCB.

- Seleccionar la herramienta de zona de cobre
- Elegir la red GND
- Dibujar la zona sobre la PCB
- Confirmar la creación del plano
  
Después de crear la zona, se presionó la tecla:

- B

para que el programa rellenara automáticamente el área con cobre.

### ꩜ Paso 7 — Preparar fabricación

En la etapa final agregamos detalles necesarios antes de enviar la PCB a fabricar.

### Elementos añadidos

- Bordes finales
- Textos
- Nombres
- Agujeros de montaje
- Diseños gráficos

### Agujeros de montaje

En el esquemático agregamos el componente:

- MountingHole

Estos agujeros sirven para fijar físicamente la placa con tornillos o soportes.

Luego fueron posicionados dentro de la PCB como cualquier otro componente.

### Importación de gráficos

También aprendimos a importar diseños o imágenes en formatos:

- SVG
- DXF

La importación se realiza desde:

- Archivo → Importar → Gráficos

Importante:

- Los gráficos deben colocarse en capas de serigrafía (Silkscreen) y no en capas de cobre.

### Revisión final — DRC

Antes de terminar el diseño de la PCB, realizamos una revisión usando la herramienta:
- DRC (Design Rule Check)

Esta herramienta sirve para detectar errores en la placa antes de enviarla a fabricar.

¿Cómo se hace?

- Abrir el editor PCB en KiCad
- Buscar el ícono de verificación o checklist en la parte superior derecha
- Hacer clic en DRC
- Presionar el botón para iniciar la revisión
- Esperar a que el programa analice la PCB
  
Después de eso, KiCad muestra una lista con los posibles errores encontrados.

---

- encargo-09a
  
esquemáticos y PCB en KiCad

cada estudiante debe tomar 2 de las 4 secciones distintas del sintetizador realizado en el proyecto 1, y crear un proyecto en KiCad por cada una, que contenga tanto el esquemático y la PCB de cada sección.

anotar cada paso en la bitácora, incluyendo mayores aprendizajes y dificultades encontradas, además de problemas y dudas que quieran que abordemos en la próxima clase.

- No tomé capturas de todos los procesos del n.1 porque se me olvidó, ya que estaba concentrada entre hacer la placa y volver a ver la clase de KiCad.

### Esquemático y PCB 1 

1.  Crear esquemático (555)

![foto](./imagenes/uno.png)

2. Asociar huellas

![foto](./imagenes/dos.png)

3. Abrir PCB Editor 

4. Definir pistas

5. Distribuir componentes

6. Rutear conexiones

 ![foto](./imagenes/tres.png) 
 
7. Preparar fabricación

![foto](./imagenes/cuatro.png)  

Stay coo /inserte ruido de paloma

![foto](./imagenes/cinco.png)  
![foto](./imagenes/seis.png)

Aquí revisé la parte de DRC y me aparecieron esos avisos. Por lo que entendí, el texto y los dibujos están tapando algunas partes de la placa, pero no sé si eso realmente afecta su funcionamiento.

![foto](./imagenes/siete.png)  

También me pasó que no había dejado espacio para los agujeros, así que tuve que mover un poco los componentes. No estoy segura de si todo está bien colocado y aún me falta aprender más cómo ubicar los componentes de manera estratégica.

### Esquemático y PCB 2

1.  Crear esquemático (Mix)

![foto](./imagenes/unoo.png)  

2. Asociar huellas

![foto](./imagenes/doss.png)

3. Abrir PCB Editor 

![foto](./imagenes/tress.png)

4. Definir pistas

![foto](./imagenes/pistas.png)

5. Distribuir componentes

![foto](./imagenes/cuatroo.png)

6. Rutear conexiones

![foto](./imagenes/cincoo.png)

GND 

![foto](./imagenes/seiss.png) 
 
7. Preparar fabricación

![foto](./imagenes/sietee.png)  

Acá quería intentar que todos los componentes se vieran en 3D, no entendí por qué no se ponen todos automáticamente. Intenté colocarlos, pero me salían cosas nada que ver, no sé si eran los correctos y, según yo, no, porque no se veían como los componentes que buscabaAAAAAaaaaaaaaa(,,•᷄‎ࡇ•᷅ ,,)? tampoco investigué mucho más a fondo ¯\_(ツ)_/¯

![foto](./imagenes/idk.png)  
