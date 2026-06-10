Sistema IoT para Monitoreo y Localización de Ganado Bovino

Descripción

Este proyecto tiene como objetivo desarrollar un sistema IoT capaz de apoyar a los ganaderos en la localización y monitoreo de ganado bovino en zonas rurales mediante tecnologías GPS, LoRa y GSM.

La solución busca reducir el tiempo de búsqueda de animales en libre pastoreo y proporcionar alertas ante posibles situaciones anormales, como periodos prolongados de inmovilidad.

⸻

Problema

En muchas comunidades rurales los animales son llevados a zonas extensas de pastoreo donde la supervisión constante resulta complicada. Esto puede ocasionar pérdidas de tiempo durante la búsqueda de animales, dificultades para detectar incidentes y una menor capacidad de reacción ante situaciones inesperadas.

⸻

Objetivo General

Diseñar e implementar un sistema IoT para monitoreo y localización de ganado bovino utilizando GPS, LoRa y GSM.

⸻

Arquitectura General

Nodo Animal

GPS + MPU6050 + LilyGO LoRa32

↓

LoRa

↓

Gateway

LilyGO LoRa32 + SIM808

↓

GSM

↓

Usuario

⸻

Tecnologías Utilizadas

Hardware

* LilyGO LoRa32
* GPS NEO-6M
* MPU6050
* SIM808
* Baterías LiPo
* Panel Solar

Software

* Arduino IDE
* GitHub
* Draw.io

Comunicaciones

* GPS
* LoRa
* GSM

⸻

Estado Actual

Completado

* Definición del problema.
* Arquitectura del sistema.
* Selección de componentes.
* Documentación inicial.
* Adquisición de dos LilyGO LoRa32.

En Desarrollo

* Comunicación LoRa entre nodos.
* Integración de sensores.
* Desarrollo del firmware.

⸻

Próximos Pasos

1. Validar comunicación LoRa.
2. Integrar GPS.
3. Integrar MPU6050.
4. Implementar alertas.
5. Realizar pruebas de campo.

⸻

Autor

Braulio Emilio Hernández Olvera

Ingeniería en Telemática
