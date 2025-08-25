# Robot Recolector de Basura con Raspberry Pi Pico W

Este proyecto implementa un **robot recolector de basura autónomo** utilizando una **Raspberry Pi Pico W** y una **cámara OV7670**. El sistema identifica objetos que simulan basura mediante procesamiento de imagen básica y se dirige hacia ellos para simular su recolección.

---

##  Descripción

El robot funciona de la siguiente manera:

- **Captura de Imagen:**  
  La cámara OV7670 toma imágenes de baja resolución (formato YUV) para facilitar su análisis.

-  **Detección de Basura:**  
  El sistema analiza la imagen para detectar objetos con ciertas características (por ejemplo, colores brillantes o formas contrastantes) que simulan basura.

---

##  Integrantes del Proyecto

- **Nicolás Moreno Ovalle** - 20212005140  
- **Johan Sebastián Cáceres Rodríguez** - 20212005111

---

## Hardware

- Raspberry Pi Pico W  
- Cámara OV7670  
- Driver de motor y motores DC  
- LEDs  
- Brazo de madera

### Software

- MicroPython en la Raspberry Pi Pico W  
- Bibliotecas:
  - `adafruit_ov7670`  
  - `digitalio`  
  - `pwmio`  
  - `board`

---

## Uso

1. Conecta la Raspberry Pi Pico W a una batería o fuente de energía.
2. El robot comenzará a capturar imágenes automáticamente.
3. Al detectar basura (según el color/luminancia predefinida), se moverá hacia ella.
4. Una vez cerca, el robot puede:
   - Detenerse.
   - Recojer elemento o basura
   - Encender un LED como indicación.

---
