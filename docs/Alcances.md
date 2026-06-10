# Alcances del Proyecto

## Alcance General

Diseñar e implementar un sistema IoT para monitoreo y localización de ganado bovino en zonas rurales mediante tecnologías ESP32, GPS, LoRa y GSM.

## Funcionalidades

- Obtener ubicación GPS del animal.
- Transmitir información mediante LoRa.
- Recibir información en un gateway fijo.
- Enviar alertas mediante red GSM.
- Mostrar ubicación en Google Maps.
- Detectar periodos prolongados de inactividad.
- Generar alertas por inmovilidad prolongoda o posibles situaciones anormales.

## Cobertura Inicial

- Hasta 10 animales monitoreados.
- Área aproximada de 8 a 10 km².
- Comunicación mediante gateway instalado en un punto elevado.

## Usuarios

- Ganaderos.
- Administradores de ranchos.

## - Alcances Técnicos

* El sistema estará diseñado para operar principalmente mediante comunicación LoRa entre el nodo animal y el gateway.
* El gateway utilizará la red GSM únicamente para el envío de notificaciones al usuario.
* La precisión de ubicación esperada será de aproximadamente 20 a 50 metros.
* El sistema estará orientado a la localización del ganado y detección de inmovilidad prolongada.
* El sistema no realizará diagnósticos veterinarios ni detección automática de enfermedades en esta versión.

⸻

## Alcances Energéticos

* Se buscará una autonomía mínima de 15 días para el nodo animal.
* El sistema utilizará mecanismos de ahorro energético mediante Deep Sleep.
* El gateway estará preparado para operar mediante alimentación solar en futuras pruebas de campo.

⸻

## Alcances de Desarrollo

* Se validará la comunicación LoRa entre dos nodos ESP32.
* Se integrará un módulo GPS para la obtención de coordenadas.
* Se integrará un acelerómetro MPU6050 para detección de movimiento.
* Se realizarán pruebas de alcance y funcionamiento en condiciones reales.
