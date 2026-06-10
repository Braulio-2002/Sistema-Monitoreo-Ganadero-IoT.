
## Arquitectura del Sistema

## Descripción General

El sistema propuesto está diseñado para monitorear y localizar ganado bovino en zonas rurales mediante una arquitectura distribuida basada en tecnologías IoT. La solución está compuesta por tres elementos principales:

1. Nodo Animal.
2. Gateway Fijo.
3. Usuario Final.

La comunicación principal entre el nodo animal y el gateway se realiza mediante tecnología LoRa debido a su bajo consumo energético y capacidad de comunicación a largas distancias. Posteriormente, el gateway utiliza la red GSM para enviar información y alertas al usuario.

⸻

## Arquitectura General

Nodo Animal
     │
     │ LoRa
     ▼
Gateway Fijo
     │
     │ GSM
     ▼
Usuario Final

⸻

## Nodo Animal

Descripción

El nodo animal es el dispositivo instalado en el collar del ganado. Su función principal es obtener información del animal y transmitirla al gateway.

Funciones

* Obtener coordenadas geográficas mediante GPS.
* Detectar movimiento e inmovilidad prolongada.
* Transmitir información mediante LoRa.
* Operar con bajo consumo energético.
* Almacenar temporalmente información cuando no exista comunicación con el gateway.

## Componentes

LilyGO LoRa32

Función:
Microcontrolador principal encargado del procesamiento y comunicación LoRa.

GPS NEO-6M

Función:
Obtención de coordenadas geográficas.

MPU6050

Función:
Detección de movimiento e inmovilidad prolongada.

Batería LiPo

Función:
Alimentación energética del nodo animal.

Antena LoRa

Función:
Transmisión inalámbrica de largo alcance.

⸻

## Gateway Fijo

Descripción

El gateway es el punto central de recepción de información. Se instalará en una ubicación elevada para maximizar la cobertura de comunicación LoRa.

Funciones

* Recibir información de los nodos animales.
* Procesar datos recibidos.
* Generar alertas.
* Enviar notificaciones mediante GSM.
* Almacenar información relevante.

## Componentes

LilyGO LoRa32

Función:
Recepción y procesamiento de información LoRa.

SIM808

Función:
Comunicación GSM para envío de alertas y notificaciones.

Batería LiPo

Función:
Alimentación de respaldo.

Panel Solar

Función:
Recarga de la batería y aumento de la autonomía del gateway.

Antena LoRa

Función:
Recepción de información proveniente de los nodos animales.

⸻

## Usuario Final

Descripción

Corresponde al ganadero o administrador responsable de supervisar el ganado.

Funciones

* Recibir alertas.
* Consultar ubicación del ganado.
* Tomar decisiones basadas en la información recibida.

## Medios de Visualización

* Mensajes SMS.
* Enlaces de ubicación en Google Maps.

⸻

## Flujo de Operación

1. El nodo animal despierta desde modo de bajo consumo.
2. Obtiene la ubicación GPS.
3. Obtiene información de movimiento mediante el MPU6050.
4. Genera un paquete de datos.
5. Transmite la información mediante LoRa.
6. El gateway recibe la información.
7. El gateway procesa los datos.
8. Si existe una situación anormal, genera una alerta.
9. El gateway envía una notificación mediante GSM.
10. El usuario recibe la información.

⸻

## Estrategia Energética

Con el objetivo de maximizar la autonomía del collar, el nodo animal permanecerá la mayor parte del tiempo en modo Deep Sleep.

Proceso energético:

1. Despertar.
2. Obtener datos.
3. Transmitir información.
4. Regresar a Deep Sleep.

Esta estrategia busca alcanzar una autonomía mínima de 15 días y servir como base para futuras optimizaciones orientadas a superar los 60 días de funcionamiento continuo.

⸻

## Consideraciones de Diseño

* La precisión de ubicación esperada será de aproximadamente 20 a 50 metros.
* El sistema prioriza la autonomía energética sobre la actualización en tiempo real.
* La comunicación principal será LoRa.
* La red GSM se utilizará únicamente para la comunicación entre el gateway y el usuario.
* La arquitectura permitirá futuras ampliaciones sin modificar la estructura principal del sistema.
