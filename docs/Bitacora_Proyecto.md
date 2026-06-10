# Bitácora del Proyecto

## Información General

*Proyecto:* Sistema IoT para Monitoreo y Localización de Ganado Bovino

*Autor:* Braulio Hernández

*Carrera:* Ingeniería en Telemática

# Objetivo
Desarrollar un sistema IoT capaz de monitorear ganado bovino mediante un collar inteligente que obtenga información de ubicación y movimiento,
utilizando comunicación LoRa para transmitir los datos a un gateway y posteriormente enviarlos al usuario mediante GSM.

# Estado Actual
## Hardware Disponible

### Comunicación LoRa
- 2 × LilyGO LoRa32 (ESP32 + LoRa + OLED)
- 2 × Antenas LoRa

### Comunicación GSM
- 1 × Módulo SIM808
- 1 × Antena GPS para SIM808

## Hardware Pendiente
### Nodo Animal
- GPS NEO-6M
- MPU6050
- Batería LiPo 2500-5000 mAh

### Gateway
- Batería LiPo 10000 mAh
- Panel solar 6V 5W
- TP4056

# Arquitectura Definida

Nodo Animal:
- ESP32 LoRa
- GPS NEO-6M
- MPU6050
- Batería

Funciones:
- Obtener ubicación GPS
- Detectar movimiento
- Detectar inmovilidad prolongada
- Transmitir datos mediante LoRa

Gateway:
- ESP32 LoRa
- SIM808
- Batería
- Panel solar

Funciones:
- Recibir datos LoRa
- Generar alertas
- Enviar información al usuario mediante GSM
  
# Decisiones Tomadas
## Precisión GPS
No se requiere precisión centimétrica.
Precisión aceptable:
- 20 metros
- 50 metros
## Comunicación
Tecnología principal:
LoRa
Razón:
- Largo alcance
- Bajo consumo energético
## Estrategia de Energía
El collar permanecerá en Deep Sleep la mayor parte del tiempo.
Proceso:
1. Despertar
2. Obtener ubicación
3. Obtener movimiento
4. Transmitir datos
5. Regresar a Deep Sleep
## Estrategia de Reporte
Modo normal:
- Envío de información cada hora
Modo alerta:
- Envío inmediato cuando se detecte inmovilidad prolongada
# Próximos Pasos
## Fase 1
- Validar comunicación LoRa entre los dos LilyGO
## Fase 2
- Definir formato de mensajes
## Fase 3
- Integrar GPS NEO-6M
## Fase 4
- Integrar MPU6050
## Fase 5
- Realizar pruebas de autonomía
# Historial
## 10/06/2026

- Se recibió el segundo LilyGO LoRa32.
- Se completó el hardware mínimo para realizar pruebas LoRa.
- Se confirmó que el alcance de comunicación debe ser grande.
- Se definió que la precisión GPS requerida es de 20 a 50 metros.
