# Requerimientos del Sistema

## Introducción

El sistema busca apoyar a los ganaderos en la localización y monitoreo de ganado bovino en zonas rurales con baja cobertura celular, reduciendo el tiempo de búsqueda y permitiendo la detección temprana de posibles incidentes.

---

# Requerimientos Funcionales

## RF-01 Obtención de Ubicación

El sistema debe obtener la ubicación geográfica del animal mediante GPS.

---

## RF-02 Transmisión de Datos

El nodo animal debe transmitir la información de ubicación al gateway mediante tecnología LoRa.

---

## RF-03 Recepción de Datos

El gateway debe recibir información proveniente de múltiples nodos animales.

---

## RF-04 Generación de Alertas

El sistema debe generar alertas cuando un animal permanezca inmóvil durante un periodo de tiempo configurable.

---

## RF-05 Envío de Notificaciones

El gateway debe enviar alertas al usuario mediante la red GSM.

---

## RF-06 Consulta de Ubicación

El usuario debe poder visualizar la última ubicación registrada mediante Google Maps.

---

## RF-07 Identificación de Animales

Cada nodo debe contar con un identificador único para distinguir a cada animal monitoreado.

---

## RF-08 Monitoreo Multianimal

El sistema debe permitir monitorear inicialmente hasta 10 animales.

---

# Requerimientos No Funcionales

## RNF-01 Bajo Consumo Energético

El nodo animal debe optimizar el consumo de energía para maximizar la duración de la batería.

---

## RNF-02 Resistencia Ambiental

El dispositivo debe soportar condiciones normales de uso en exteriores.

---

## RNF-03 Tamaño Compacto

El dispositivo debe ser lo suficientemente compacto para colocarse en un collar o accesorio del animal.

---

## RNF-04 Cobertura Rural

El sistema debe operar en zonas con cobertura celular limitada utilizando LoRa como medio principal de comunicación.

---

## RNF-05 Escalabilidad

La arquitectura debe permitir agregar más nodos en futuras versiones.

---

# Requerimientos del Usuario

## RU-01

El ganadero debe recibir alertas sin necesidad de recorrer constantemente el cerro.

---

## RU-02

El ganadero debe poder localizar rápidamente un animal perdido.

---

## RU-03

El ganadero debe recibir información útil para reducir pérdidas de ganado.

---

## RU-04

El sistema debe ser sencillo de utilizar desde un teléfono móvil.

RF-09 Almacenamiento Temporal de Datos

El nodo animal debe almacenar temporalmente la información cuando no exista comunicación con el gateway y transmitirla cuando la conexión sea restablecida.

⸻

## RF-10 Monitoreo de Batería

El sistema debe monitorear el nivel de batería del nodo animal y generar alertas cuando se detecte un nivel bajo de energía.

⸻

## RNF-06 Autonomía Energética

El nodo animal debe operar con una autonomía mínima objetivo de 15 días bajo condiciones normales de funcionamiento.

⸻

## RNF-07 Precisión de Ubicación

El sistema debe proporcionar una precisión aproximada de entre 20 y 50 metros, suficiente para facilitar la localización del ganado.

⸻

## RNF-08 Operación en Modo de Bajo Consumo

El nodo animal debe utilizar mecanismos de ahorro energético, como Deep Sleep, para maximizar la duración de la batería.

⸻

## RNF-09 Arquitectura Modular

La arquitectura debe permitir la incorporación futura de sensores adicionales sin requerir cambios significativos en el diseño general.

⸻

## RU-05 Facilidad de Mantenimiento

Los componentes principales del sistema deben ser fáciles de reemplazar o actualizar en caso de falla.

⸻

## RU-06 Tiempo de Respuesta Aceptable

El usuario debe recibir alertas de eventos críticos en un tiempo razonable para permitir la toma de decisiones oportunas.
