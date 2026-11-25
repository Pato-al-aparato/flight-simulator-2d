# Arquitectura inicial

Este documento recoge las decisiones de arquitectura del simulador a medida que se vayan definiendo.

## Áreas principales

### Modelo físico

Responsable de representar el entorno y calcular magnitudes como gravedad, velocidad, aceleración y, más adelante, resistencia atmosférica.

### Nave

Agrupará el estado y los componentes principales de la nave, como masa, combustible, motor y posibles daños.

### Control

Separará el control manual del modo automático para que ambos puedan actuar sobre la misma lógica de simulación.

### Interfaz

JavaFX mostrará tanto la representación 2D del vuelo como la instrumentación necesaria para interpretar el estado de la nave.

## Criterio de diseño

La prioridad será mantener responsabilidades claras entre clases y evitar que la lógica de simulación dependa directamente de la interfaz gráfica.
