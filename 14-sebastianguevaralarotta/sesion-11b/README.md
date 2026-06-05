# sesion-11b

# Trabajo en proyecto 

El dia de hoy estamos hablando de el capitulo 5 de el libro de fotografia. 

recitaron un poema de un poeta que esta funado, pero era vanguardista en su epoca, causo el despido de un profesor en su momento. Creo que es interesante como se conecta el arte con la poesia o la expresion humana, reflejada en diversos hambitos academicos. 

Apuntes de conexion realizadoa en la clase: 

# Conexiones del Circuito

## CD4046 (PLL)

### Pin 1
- Conectado al pin 2.

### Pin 2
- Conectado al pin 1.
- Conectado al pin 3.

### Pin 3
- Conectado al pin 2.
- Conectado a GND.

### Pin 4
- Conectado al pin 3 del TL072.
- Conectado a una resistencia de 100 kΩ.

### Pin 5
- Conectado a GND.

### Pin 6
- Conectado al pin 7.
- Conectado a un capacitor de 1 µF.

### Pin 7
- Conectado al pin 6.
- Conectado a un capacitor de 1 µF.

### Pin 8
- Conectado a GND.
- Conectado mediante un capacitor de 100 nF (104) al pin 14.

### Pin 9
- Conectado a la pata 2 del potenciómetro B1M.

### Pin 10
- Sin conexión.

### Pin 11
- Conectado a la pata 2 del potenciómetro B500k.
- Conectado a una resistencia de 100 kΩ.
- Conectado a GND.

### Pin 12
- Conectado a una resistencia de 100 kΩ.
- Conectado a GND.

### Pin 13
- Conectado al pin 14.
- Conectado a GND.

### Pin 14
- Conectado al pin 13.
- Conectado a GND.
- Conectado mediante un capacitor de 100 nF (104) desde el pin 8.

### Pin 15
- Conectado a GND.

### Pin 16
- Conectado a VCC (+5 V).
- Conectado a un capacitor de desacople de 100 nF (104).

### Capacitor de desacople 100 nF
- Una pata al pin 16.
- La otra pata a GND.

---

## TL072

### Pin 1
- Conectado a un capacitor de 10 nF (103).
- Conectado al pin 2.
- Conectado a la pata 1 del potenciómetro B250k.
- Conectado a la pata 1 del potenciómetro B100k.
- Conectado al pin 3 del LM386.

### Pin 2
- Conectado a un capacitor de 10 nF (103).
- Conectado a la pata 2 del potenciómetro B250k.
- Conectado a una resistencia de 10 kΩ.
- Conectado a GND.

### Pin 3
- Conectado a una resistencia de 100 kΩ.
- Conectado al pin 4 del CD4046.
- Conectado a un capacitor de 100 nF (104).
- Conectado a GND.

### Pin 4
- Conectado a GND.
- Conectado a un capacitor de 100 nF (104).

### Pin 5
- Sin conexión.

### Pin 6
- Conectado a una resistencia de 10 kΩ.
- Conectado al pin 7.

### Pin 7
- Conectado a una resistencia de 10 kΩ.
- Conectado al pin 6.

### Pin 8
- Conectado a VCC (+5 V).
- Conectado al pin 6.
- Conectado al pin 7.

---

## LM386

### Pin 1
- Sin conexión.

### Pin 2
- Conectado a GND.

### Pin 3
- Conectado al pin 1 del TL072.
- Conectado a la pata 2 del potenciómetro B100k.

### Pin 4
- Conectado a GND.
- Conectado al terminal negativo de un capacitor de 100 µF.

### Pin 5
- Conectado al terminal positivo del capacitor de 100 µF.
- Conectado al terminal negativo del capacitor de salida hacia el parlante.
- Conectado a una pinza caimán.
- Conectado al terminal positivo del parlante.

### Pin 6
- Conectado a VCC (+5 V).

### Pin 7
- Conectado al terminal positivo de un capacitor de 1 µF.
- El terminal negativo del capacitor va a GND.

### Pin 8
- Conectado al terminal positivo del capacitor de 100 µF conectado al pin 4.

---

## Potenciómetros

### B1M (Control de melodía)
- Pata 2 conectada al pin 9 del CD4046.

### B500k (Rango de melodía)
- Pata 2 conectada al pin 11 del CD4046.

### B250k
- Pata 1 conectada al pin 1 del TL072.
- Pata 2 conectada al pin 2 del TL072.

### B100k
- Pata 1 conectada al pin 1 del TL072.
- Pata 2 conectada al pin 3 del LM386.

---

## Alimentación

### VCC (+5 V)
- Pin 16 del CD4046.
- Pin 8 del TL072.
- Pin 6 del LM386.

### GND común
- CD4046: pines 3, 5, 8, 11, 12, 13, 14 y 15.
- TL072: pin 4.
- LM386: pines 2 y 4.
- Terminales negativos de los capacitores indicados.
- Línea de tierra común de la protoboard.


  
