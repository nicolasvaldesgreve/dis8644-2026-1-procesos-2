# sesion-08a

Martes 28 de Abril, 2026. 

Nota del día: no pude ir a esta clase pero el video me ayudo mucho. 

## Referentes (y otras cosas)

- **Ryosuke Kiyasu** un músico y percusionista japonés conocido por sus solos de caja (snare drum) experimentales y de ruido (noise). Según gemini, Ryosuke Kiyasu es un baterista y percusionista experimental japonés con sede en Tokio, mundialmente reconocido como pionero del "solo de redoblante" (snare drum soloist). Ha redefinido el uso de la percusión dentro de la música de vanguardia y el movimiento noise. En lugar de utilizar una batería completa, centra sus caóticas y expresivas presentaciones en vivo en un único tambor redoblante.
- **Winter Bloom**

## Qué aprendí hoy 

video de la clase: <https://youtu.be/w761LD5B2BQ>

### Kicad 

KiCad es una suite de software libre y de código abierto para la automatización del diseño electrónico (EDA). Permite diseñar esquemas eléctricos y convertirlos en diseños de placas de circuito impreso (PCB). - <https://www.kicad.org/>  

Antes de empezar:

Kicad funciona con dos sistemas/programas distintos integrados en la aplicación. Uno se encarga de la parte de la esquematización y el otro para crear la PCB. 

Estos sistemas utilizan los siguientes lenguajes: 

- **Símbolos:** abstractos, esquemáticos. Representación conceptual de un componente (específicamente en un esquemático). 
- **Huellas:** PCB, el mundo físico. Representación del espacio físico de cada componente en la PCB. 
- (extra) Aristóteles: **"Género – Especie – Individuo"** que en KiCad se traduce como **"THT – Resistor – R2"**

Hay un archivo central (`.kicad_pro`) que enlaza todo lo demás.

El archivo _sch corresponde al esquemático, donde se diseña el circuito de forma abstracta.
El archivo _pcb permite visualizar cómo ese esquemático se materializa en una placa física (PCB).

| Extensión       | Qué es          |
|-----------------|-----------------|
| `.kicad_pro`    | El proyecto    |
| `.kicad_sch`    | El esquemático - donde se diseña el circuito de forma abstracta |
| `.kicad_pcb`    | La PCB - permite visualizar cómo ese esquemático se materializa en una placa física (PCB) | 

#### Flujo de trabajo: 

(En la clase solo se vieron los tres primeros puntos)

1. **Dibujar esquemático en (`kicad_sch`):** Crear el diagrama lógico del circuito. Se abre el archivo y una vez que se tengan todos los componentes se conectan (Se debe hacer doble click en cada componente para asignarle un valor, es importante mantener la misma nomenclatura). 
2. **Asociar huellas (físico) a símbolos (abstracciones/ideas)**
3. **Abrir PCB Editor (PCB New):** Importar el esquemático para comenzar el diseño de la placa. 
4. **Definir tamaño de pistas:** Establecer grosores según requerimientos eléctricos.
5. **Repartir/distribuir componentes:** Ubicar los elementos en la placa de forma estratégica. 
6. **Rutear conexiones**
7. **Adornar o preparar para fabricación:** Añadir bordes, textos, capas, etc.

#### A la hora de buscar los componentes:

| Elemento / Símbolo        | Representación |
|--------------------------|----------------|
| Resistencia              | R              | 
| Capacitor lenteja   | C |
| Capacitor polarizado   | C (polarizado) - C_Polarized| 
| Potenciómetro            | R - R_Potenciometer  | 
| Batería                  | Battery cell   |
| Circuito integrado       | U              | 
| Parlante                 | 8 ohm / 3W     | 
| Ground              | GND     | 
| Energía positiva              | VCC     | 
| Parlante                 | 8 ohm / 3W     | 
| Led             | LED     | 

#### Huellas utilizadas en clase:

- **Capacitor cerámico:** Capacitor_THT:C_Disc_D3.8mm_W2.6mm_P2.50mm                    
- **Capacitor electrolítico:** Capacitor_THT:CP_Radial_D5.0mm_P2.50mm                         
- **Resistencia:** Resistor_THT:R_Axial_DIN0207_L6.3mm_D2.5mm_P10.16mm_Horizontal 
- **Potenciómetro:** Potentiometer_THT:Potentiometer_Alps_RK163_Single_Horizontal  
- **Led:** LED_THT:LED_D5.0mm             

## Qué hice hoy

Para empezar se realizamos el esquemático del Atari Punk (circuito que ya conocíamos previamente). 

### Paso 1: Dibujar esquemático.

Abrimos el .kicad_sch y empezamos a colocar componentes. Luego los conectamos con cables. A cada componente hay que hacerle doble clic para asignarle un valor. Esos valores son referenciales, para que alguien pueda leer el esquemático; no afectan la PCB directamente.

Mi esquemático:

![paso1](./imagenes/paso1.png)
![paso1-1](./imagenes/paso1-1.png)
![paso1-2](./imagenes/paso1-2.png)

### Paso 2: Asociar huellas a símbolos.

Se reemplazan los símbolos por sus equivalentes físicos.
Para esto se abre el diálogo Assign Footprints, donde se asocia cada símbolo con su huella correspondiente según:

![paso2](./imagenes/paso2.png)
![paso2-2](./imagenes/paso2-2.png)
![paso2-3](./imagenes/paso2-3.png)
![paso2-4](./imagenes/paso2-4.png)

### Paso 3: Abrir PCB Editor.

Desde el editor de esquemático se abre el PCB Editor, donde aparecen todos los componentes listos para ser distribuidos. Hay que recordar: ordenar los componentes, dibujar el contorno de la placa, ya que el software arroja errores si no existe y asegurarse de hacerlo en la capa correcta. 

![paso3](./imagenes/paso3.png)
![paso3-1](./imagenes/paso3-1.png)
![paso3-2](./imagenes/paso3-2.png)

