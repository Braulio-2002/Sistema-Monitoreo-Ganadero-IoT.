Decisiones Técnicas del Proyecto

DT-001

Decisión

Utilizar tecnología LoRa para la comunicación entre el nodo animal y el gateway.

Justificación

Las zonas de pastoreo presentan poca o nula cobertura WiFi. LoRa proporciona largo alcance y bajo consumo energético, características adecuadas para aplicaciones rurales.

⸻

DT-002

Decisión

Utilizar GPS NEO-6M para la obtención de coordenadas geográficas.

Justificación

Ofrece una precisión suficiente para los objetivos del proyecto y cuenta con amplia documentación para su integración con ESP32.

⸻

DT-003

Decisión

Implementar un gateway fijo ubicado en una zona elevada.

Justificación

Permite maximizar la cobertura LoRa y facilitar la recepción de información proveniente de los nodos animales.

⸻

DT-004

Decisión

Utilizar GSM únicamente en el gateway.

Justificación

Reduce el consumo energético y el costo de cada nodo animal.

⸻

DT-005

Decisión

Implementar detección de inmovilidad prolongada.

Justificación

Permite identificar posibles situaciones anormales sin incrementar significativamente la complejidad del sistema.

⸻

DT-006

Decisión

Utilizar Deep Sleep como estrategia principal de ahorro energético.

Justificación

La autonomía del nodo animal es uno de los objetivos más importantes del proyecto.

⸻

DT-007

Decisión

Establecer una precisión de ubicación aproximada entre 20 y 50 metros.

Justificación

Es suficiente para facilitar la localización del ganado sin requerir sistemas GPS de alta precisión.

⸻

DT-008

Decisión

Definir una autonomía mínima objetivo de 15 días.

Justificación

Permite un equilibrio adecuado entre funcionalidad, consumo energético y costo del sistema.

⸻

DT-009

Decisión

Implementar alimentación solar para el gateway.

Justificación

Facilita el funcionamiento continuo en ubicaciones rurales con acceso limitado a energía eléctrica.

⸻

DT-010

Decisión

Mantener el alcance inicial del sistema en aproximadamente 10 animales.

Justificación

Permite validar la solución antes de escalar a implementaciones de mayor tamaño.
