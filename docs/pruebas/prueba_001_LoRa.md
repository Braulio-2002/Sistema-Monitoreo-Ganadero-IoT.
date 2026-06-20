Prueba 001 - Comunicación LoRa Punto a Punto

Información General

Fecha: 20 de junio de 2026

Responsable: Braulio Hernández

Objetivo:

Validar la comunicación inalámbrica mediante tecnología LoRa entre dos placas LILYGO TTGO LoRa32 V1.6.1.

⸻

Hardware Utilizado

Nodo Transmisor

* LILYGO TTGO LoRa32 V1.6.1
* Antena LoRa 915 MHz
* Alimentación mediante USB

Nodo Receptor

* LILYGO TTGO LoRa32 V1.6.1
* Antena LoRa 915 MHz
* Alimentación mediante USB

⸻

Configuración Utilizada

Frecuencia:

915 MHz

Pines LoRa:

SCK: GPIO 5
MISO: GPIO 19
MOSI: GPIO 27
SS: GPIO 18
RST: GPIO 14
DIO0: GPIO 26

⸻

Descripción de la Prueba

Se configuró una placa como transmisor y una segunda placa como receptor.

El transmisor envió mensajes de texto consecutivos mediante LoRa cada dos segundos.

El receptor recibió los paquetes correctamente y mostró el mensaje recibido junto con el valor RSSI correspondiente.

⸻

Resultado Obtenido

La comunicación entre ambos dispositivos fue exitosa.

Se recibieron correctamente todos los mensajes enviados durante la prueba.

La medición RSSI obtenida fue aproximadamente de:

RSSI = -28 dBm

Este valor indica una señal muy fuerte debido a la corta distancia entre ambos dispositivos.

⸻

Evidencia Experimental

Mensajes enviados:

Enviado: Nodo Animal #17
Enviado: Nodo Animal #18
Enviado: Nodo Animal #19

Mensajes recibidos:

Recibido: Nodo Animal #18
RSSI: -28

Recibido: Nodo Animal #19
RSSI: -28

Recibido: Nodo Animal #20
RSSI: -28

⸻

Conclusiones

La prueba permitió validar el funcionamiento del módulo LoRa integrado en las placas LILYGO TTGO LoRa32 V1.6.1.

La comunicación punto a punto quedó demostrada y constituye la base de la arquitectura de comunicación del sistema de monitoreo de ganado bovino.

Esta prueba confirma la viabilidad de utilizar LoRa como tecnología principal para la transmisión de información entre el nodo animal y el gateway.
