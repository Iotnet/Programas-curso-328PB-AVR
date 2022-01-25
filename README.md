# Iotrack


Introduccion
--------------
En este repositorio se muestra la información relacionada al uso del dispositivo Iotrack asi como ejemplos de programas.

Requerimientos
--------------
-   Es necesario descargar e instalar el IDE de [Atmel Studio](https://www.microchip.com/en-us/tools-resources/develop/microchip-studio#Downloads)
-   Descargar e instalar [AVRDUDESS](https://blog.zakkemble.net/avrdudess-a-gui-for-avrdude/)
-   Programador USB/ASP
-   (opcional) convertidor TTL a USB a 3.3V

Consideraciones
-----------------
-   EL modulo Wisol para el envio de datos por medio de Sigfox, es energizado por medio del regulador de 3.3V, el cual es el mismo que la salida de 3.3V del conector para I/O.
-   Para reducir el consumo energetico, los reguladores de 3.3V y 5V deben ser habilitados por medio de los pines PC1 y PE3 del microcontrolador, respectivamente. Despues de su uso, estos deben deshablitarse para reducir el consumo.
-   El modulo de comunicacion Wisol esta conectado al puerto UART0 del microcontrolador.
-   En caso de usar baterias, se tienen señales para monitoreo del voltaje de salida de los reguladores. El regulador de 3.3V pone en alto el PIN PC0 si el voltaje de salida es menor al 92% de 3.3V. El pin PD7 cambia a alto si la tension de salida del regulador cae por debajo del 92% de 5V.

Calculo de duracion de  baterias
--------------
Copnsidernado las 4 Pilas AAA
Num. mensajes al dia
Consumo de sensores
Tiempo activo (toma de lecturas)

Recomendaciones
-------
 
Ejemplos
--------
- [Boton y Led](https://github.com/Iotnet/Iotrack/tree/main/Boton_y_led)
- Envio de mensaje (Hola mundo)
- Timmer
- ADC
- Modo Sleep para bajo consumo
- Sensor I2C (TWI)
- One wire (DSB18b20)
- Sensor Serial (GPS, RS232, RS485)
- Downlink
