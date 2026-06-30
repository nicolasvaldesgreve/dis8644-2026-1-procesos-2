# examen-grupo-02

## integrantes

- Isidora Alvarez / [isidoraalvarez](https://github.com/isidoraalvarez/dis8644-2026-1)
- Dayana Pañitrur / [dayanapanitrur](https://github.com/dayanapanitrur/dis8644-2026-1)
- Camila Ramirez / [Estrabismx](https://github.com/Estrabismx/dis8644-2026-1)
- Angel Sabogal / [angel-udp](https://github.com/angel-udp/dis8644-2026-1)
- Tomas Catrileo / [tomascatri](https://github.com/tomascatri/dis8644-2026-1)

## criterios de diseño del sistema

inspiración para construir, desde donde partieron

contexto desde Chile, desde nuestra disponibilidad material

nombre de sistema/instrumento construido por medio de módulos

## placas soldadas

nombres de placas armadas

principio de funcionamiento de cada una

qué tipo de señal entrega a la salida, qué recibe

lista de materiales con costos. Incluir tiempo de soldadura

## carcasa

decisiones materiales y formales de la carcasa

inspiración y referentes (con cita)

## Proceso

## BOM (Bill of materiales)

### Reloj

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C polarizado   | 47µF   |  1   | C1          |
| C polarizado   | 100µF  | 1    | C2          |  
| C polarizado   | 10µF   | 1    | C4          |
| C polarizado   | 220µF  | 1    | C5          |
| Capacitor      | 100nF  | 2    | C3 C6       |
| LED            | -----  | 2    | D2 D3       |
| Diodo          | 1N4007 | 1    | D1          |
| Resistencia    | 1kΩ    | 4    | R1 R2 R3 R4 |
| LDR            | ------ | 1    | RV1         |  
| Switch         | SPDT   | 1    |  SW1        |
| Chip           | 555    | 1    | U1          |
| Chip           | L7805  | 1    | U2          |
| Base Dip       | 8 pin  | 1    | U1          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J2       |
| Conector       | Jack   | 1    | J3          |

<br>

### Secuenciador 1 / Grupo 02

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C polarizado   | 100µF  |  1   | C4          |
| C polarizado   | 10µF   | 1    | C5          |
| Capacitor      | 100nF  | 1    | C6          |
| Led            |        | 7    | D8 D9 D10 D11 D12 D13 D14 |
| Diodo          | 1N4007 | 1    | D6          |
| Transistor     | 2N2222 | 6    | Q1 Q2 Q3 Q4 Q5 Q6 |
| Resistencia    | 1KΩ    | 19   | R7 R8 R9 R10 R11 R12 R13 R14 R15 R16 R17 R18 R19 R21 R22 R23 R24 R25 R26 |
| Resistencia    | 100KΩ  | 1    | R20         |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 4040   | 1    | U2          |
| Chip           | L7805  | 1    | U4          |
| Base Dip       | 16 pin | 1    | U2          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 8    | J6 J7 J8 J9 10 J11 J12 |

<br>

### Secuenciador 2 / Grupo 02

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C polarizado   | 100µF  |  1   | C7          |
| C polarizado   | 10µF   | 1    | C8          |
| Capacitor      | 100nF  | 1    | C9          |
| Led            |        | 9    | D1 D2 D3 D4 D5 D6 D7 D8 D12 |
| Diodo          | 1N4007 | 1    | D11         |
| Transistor     | 2N2222 | 8    | Q1 Q3 Q4 Q5 Q6 Q7 Q8 Q9 Q10 |
| Resistencia    | 10KΩ   | 1    | R2          |
| Resistencia    | 1KΩ    | 18   | R3 R12 R15 R16 R17 R18 R19 R20 R21 R22 R23 R24 R25 R26 R27 R28 R29 R30 |
| Resistencia    | 220Ω   | 8    | R4 R5 R6 R7 R8 R9 R10 R11 |
| Resistencia    | 100KΩ  | 1    | R13         |
| Switch         | SPDT   | 1    | SW          |
| Chip           | 4015   | 1    | U2          |
| Chip           | L7805  | 1    | U4          |
| Base Dip       | 16 pin | 1    | U2          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 8    | J6 J7 J8 J9 10 J11 J12 J13 J14 |

<br>

### Oscilador 01 / Grupo 03

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| Capacitor      | 10nF   | 1    | C1          |
| Capacitor      | 100nF  | 1    | C5          |
| C. polarizado  | 100µF  | 3    | C2 C6 C7    |
| C. polarizado  | 10µF   | 2    | C3 C4       |
| Diodo          | 1N4007 | 1    | D1          |
| LED            | ------ | 1    | D2          |
| Resistencia    | 100KΩ  | 1    | R1          |
| Resistencia    | 1KΩ    | 1    | R2          |
| LDR            | ------ | 2    | RV1 RV2     |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 4046   | 1    | U1          |
| Chip           | L7805  | 1    | U2          |
| Chip           | 40106  | 1    | U3          |
| Base Dip       | 16 pin | 1    | U1          |
| Base Dip       | 14 pin | 1    | U3          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 1    | J1          |

<br>

### Oscilador 02 / Grupo 03

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| Capacitor      | 1µF    | 2    | C2 C7       |
| C. polarizado  | 4µF    | 1    | C3          |
| C. polarizado  | 100µF  | 1    | C4          |
| C. polarizado  | 10µF   | 2    | C5 C8       |
| Capacitor      | 100nF  | 1    | C6          |
| Led            | -----  | 2    | D1 D3       |
| Diodo          | 1N4007 | 1    | D2          |
| Resistencia    | 470KΩ  | 2    | R1 R2       |
| Resistencia    | 330KΩ  | 1    | R3          |
| Resistencia    | 1KΩ    | 1    | R4          |
| LDR            | ------ | 2    | RV1 RV2     |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 4017   | 1    | U1          |
| Chip           | 4046   | 1    | U2          |
| Chip           | 40106  | 1    | U3          |
| Chip           | L7805  | 1    | U4          |
| Base Dip       | 16 pin | 2    | U1 U2       |
| Base Dip       | 14 pin | 1    | U3          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J3       |
| Conector       | Jack   | 1    | J4          |

<br>

### Oscilador 01 / Grupo 04

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C. polarizado  | 10µF   | 3    | C2 C3 C10   |
| Capacitor      | 100nF  | 2    | C4 C11      |
| C. polarizado  | 100µF  | 1    | C9          |
| Diodo          | 1N4007 | 1    | D1          |
| LED            | -----  | 1    | D2 D8       |  
| Diodo          | 1N4148 | 4    | D3 D4 D5 D6 |
| Resistencia    | 1KΩ    | 7    | R2 R3 R4 R5 R6 R7 R8 |
| LDR            |        | 4    | RV1 RV2 RV3 RV4 |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 40106  | 1    | U1          |
| Chip           | L7805  | 1    | U2          |
| Chip           | LM324  | 1    | U3          |
| Base Dip       | 14 pin | 2    | U1 U3       |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J3       |
| Conector       | Jack   | 1    | J4          |

<br>

### Oscilador 02/ Grupo 04

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C. polarizado  | 1µF    | 3    | C1 C2       |
| C. polarizado  | 10µF   | 2    | C3 C5       |
| C. polarizado  | 100µF  | 1    | C4          |
| Capacitor      | 100nF  | 1    | C6          |
| Diodo          | 1N4148 | 1    | D1          |
| Diodo          | 1N4007 | 1    | D2          |
| LED            | ------ | 1    | D8          |
| Resistencia    | 1KΩ    | 3    | R1 R2 R9    |
| LDR            |        | 2    | RV1 RV2     |
| Switch         | SPDT   | 1    | SW1         |
| Chip           | 40106  | 1    | U1          |
| Chip           | L7805  | 1    | U5          |
| Base Dip       | 14 pin | 1    | U1          |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J1 J3       |
| Conector       | Jack   | 1    | J4          |

<br>

### Percusión 01 / Grupo 06

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| Capacitor      | 100nF  | 4    | C2 C3 C4 C11 |
| Capacitor      | 10nF   | 1    | C6          |
| C. polarizado  | 100µF  | 1    | C9          |
| C. polarizado  | 10µf   | 2    | C10 C14     |
| C. polarizado  | 0.22µF | 1    | C12         |
| Diodo          | 1N4007 | 1    | D1          |
| Resistencia    | 100KΩ  | 2    | R1 R2       |
| Resistencia    | 1KΩ    | 1    | R4          |
| LDR            |        | 4    | RV1 RV2 RV3 RV5 |
| Switch         | SPDT   | 1    | SW3         |
| Chip           | 40106  | 1    | U2          |
| Chip           | 4069   | 1    | U3          |
| Chip           | L7805  | 1    | U8          |
| Base Dip       | 14 pin | 2    | U2 U3       |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 2    | J4 J5       |

<br>

### Percusión 02 / Grupo 06

| Componente     | Valor  | Cant | PCB         |
| -------------- | ------ | ---- | ----------- |
| C. polarizado  | 10µF   | 3    | C1 C4 C6    |
| C. polarizado  | 100µF  | 2    | C2 C5       |
| C. polarizado  | 1µF    | 1    | C3          |
| Capacitor      | 100nF  | 1    | C7          |
| Diodo          | 1N4007 | 1    | D1          |
| Led            |        | 2    | D8 D9       |
| Resistencia    | 1KΩ    | 2    | R4 R5       |
| LDR            |        | 4    | RV1 RV2 RV3 RV4 |
| Switch         | SPDT   | 1    | SW3         |
| Chip           | 40106  | 1    | U1          |
| Chip           | L7805  | 1    | U8          |
| Chip           | 4070   | 1    | U9          |
| Base Dip       | 14 pin | 2    | U1 U9       |
| Perno M3       |        | 4    | H1 H2 H3 H4 |
| Conector       | Barrel | 2    | J2 J3       |
| Conector       | Jack   | 1    | J4          |

## composición

partitura e interpretación

detallar operación de la partitura, como se creó, cuales fueron los referentes (citando), cual es la simbología

## bibliografía

# REFERENTES

| Referencia | Imagen |
|------------|--------|
| https://www.lovehulten.com/ | ![Love Hultén](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |

# MATERIALIDAD

| Referencia | Imagen |
|------------------------|--------|
| https://www.acryl.cl/ | ![Acryl](./imagenes/) |
| https://abingraf.cl/collections/planchas-de-acrilico/products/acrilico-mgraf-blanco-fundido-3-mm-liner-plastico-1-22-x-2-44-mts | ![Acrílico](./imagenes/) |
| https://www.mundotransfer.cl/vinilo-de-corte-soft-cut-51-cm-ancho.html | ![Vinilo Soft Cut](./imagenes/) |
| VINILO DE CORTE BRILLANTE METAMARK M4 0.61 MTS – Abingraf S.A. | ![Metamark M4](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |

# CONSTRUCTIVO

| Referencia | Imagen |
|------------|--------|
| https://www.matrixsynth.com/2013/04/folktek-feedscape-one-of-kind-hand-made.html?m=1 | ![Feedscape](./imagenes/) |
| https://www.yankodesign.com/2023/01/24/this-strange-looking-plant-box-uses-science-to-create-eerie-music/ | ![Plant Box](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
|  | ![](./imagenes/) |
