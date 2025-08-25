# Robot Recolector de Basura con Raspberry Pi Pico W

Este proyecto implementa un **robot recolector de basura autónomo** utilizando una **Raspberry Pi Pico W** y una **cámara OV7670**. El sistema identifica objetos que simulan basura mediante procesamiento de imagen básica y se dirige hacia ellos para simular su recolección.

---

## Descripción

El robot funciona de la siguiente manera:

- **Captura de Imagen:**  
  La cámara OV7670 toma imágenes de baja resolución (formato YUV) para facilitar su análisis.

- **Detección de Basura:**  
  El sistema analiza la imagen para detectar objetos con ciertas características (por ejemplo, colores brillantes o formas contrastantes) que simulan basura.

- **Recolección con Brazo Robótico:**  
  Una vez identificado el objeto, el robot se desplaza hasta él y activa un brazo robótico tipo **MeArm**, que utiliza servomotores para simular el proceso de recolección de basura.

---

## Integrantes del Proyecto

- **Nicolás Moreno Ovalle** - 20212005140  
- **Johan Sebastián Cáceres Rodríguez** - 20212005111

---

## Hardware

- Raspberry Pi Pico W  
- Cámara OV7670  
- Driver de motor y motores DC  
- LEDs  
- Brazo robótico tipo MeArm (mínimo 4 servomotores)  
- Chasis con ruedas  
- Batería recargable o pack de baterías  
- Sensor ultrasónico HC-SR04  
- Giroscopio (MPU6050 u otro compatible)  
- Imanes (para sistema de cierre o recolección magnética)

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
   - Activar el brazo robótico tipo MeArm para recolectar el objeto.  
   - Encender un LED como indicación.  

---

## Estimación de Costos de Materiales

| Componente                            | Precio Aproximado (COP) |
|--------------------------------------|--------------------------|
| Raspberry Pi Pico W                  | $40,000 – $50,000        |
| Cámara OV7670                        | $15,000 – $25,000        |
| Módulo driver motor L298N            | $8,000 – $12,000         |
| Motores DC (x2)                      | $10,000 – $20,000        |
| Chasis con ruedas                    | $20,000 – $30,000        |
| Servomotores SG90 (x4)               | $24,000 – $32,000        |
| Estructura de brazo MeArm (acrílico) | $35,000 – $50,000        |
| **Sensor ultrasónico HC-SR04**       | $5,000 – $8,000          |
| **Giroscopio MPU6050**               | $8,000 – $12,000         |
| **Imanes (pack pequeños)**           | $4,000 – $8,000          |
| Batería recargable (LiPo o pack)     | $20,000 – $35,000        |
| LEDs, cables y misceláneos           | $10,000 – $15,000        |

**Total estimado:** $199,000 – $297,000 COP  

---
