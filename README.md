# IO_Clock

Diseño electronico de un reloj digital con un RTC (DS1307), con el fin de preveer que este se desconfigure despues de una perdida de alimentacion

=====

## Requisitos
En este proyecto se hace uso de los software listados a continuacion:
* PICC CCS
* Proteus
* EAGLE (Proximamente para el diseño de la PCB con el Hardware seleccionado)

Por parte del Hawrdware:
* P16F1823
* DS1307 + Bateria
* 2 Shift Register 74HC595
* Indicador 7 segmentos tipo **Digital Clock**
* Buzzer
* Botones
* ESP8266
* Rele

=====

## Caracteristicas del dispositivo
- [x] Voltaje de opercaion del dispositivo entre 3.3V y 5V.
- [x] Uso de sistema operativo en tiempo real (RTOS), el cual tiene como fin el manejo de diferentes tareas de forma sincrona y asincrona.
- [x] Shift Registers que permiten uso de un microcontrolador de bajo costo (en este caso P16F1823).
- [x] Circuito integrado RTC (DS1307).
- [ ] Botones para modificar la hora durante el funcionamiento en caso de cambio de Bateria del RTC.
- [ ] Mostrar informacion restante del RTC en la UI.
- [ ] Modulo de WiFi (ESP8266), con el fin de poder manipular GPIO de forma remota.
- [ ] Buzzer como indicador auditivo para alarma y demas estados de la UI.
- [ ] Rele(s) que permitan la manipulacion de dispositivos como luces de forma remota y programada.