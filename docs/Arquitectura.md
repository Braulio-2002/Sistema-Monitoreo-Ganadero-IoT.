# Arquitectura del Sistema

## Descripción General

El sistema está compuesto por tres elementos principales:

1. Nodo Animal.
2. Gateway Fijo.
3. Usuario Final.

---

## Nodo Animal

Función:

- Obtener ubicación GPS.
- Detectar movimiento.
- Transmitir información mediante LoRa.

Componentes:

- ESP32
- GPS NEO-6M
- Módulo LoRa SX1278
- Sensor de movimiento (acelerómetro)
- Batería

---

## Gateway Fijo

Función:

- Recibir información de los nodos.
- Procesar datos.
- Generar alertas.
- Enviar información mediante GSM.

Componentes:

- ESP32
- Módulo LoRa SX1278
- SIM808
- Fuente de alimentación
- Antena LoRa
- Antena GSM

---

## Usuario Final

Función:

- Recibir alertas.
- Consultar ubicación del ganado.

Medios de visualización:

- SMS
- WhatsApp
- Google Maps

---

## Flujo de Información

Nodo Animal
↓
LoRa
↓
Gateway Fijo
↓
GSM
↓
Teléfono del Ganadero
