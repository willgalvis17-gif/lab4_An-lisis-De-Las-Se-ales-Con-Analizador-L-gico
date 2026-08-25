# Análisis de Señales Seriales con Analizador Lógico

Laboratorio de **Comunicaciones Digitales** – Universidad Militar Nueva Granada (UMNG)
Facultad de Ingeniería en Telecomunicaciones

## 📋 Descripción

Este laboratorio estudia la relación entre el **tiempo de bit** y la **tasa de baudios** de una transmisión serial UART, empleando un analizador lógico de 8 canales (24 MHz) y el software **Logic 2**. La señal serial es generada por una **Raspberry Pi Pico 2W** programada en **MicroPython**.

Se analiza también el efecto de la **frecuencia de muestreo** del analizador lógico sobre la precisión de la decodificación, validando experimentalmente el criterio práctico de **N ≥ 10 muestras por bit**.

## 🎯 Objetivos

- Comprobar la relación entre el tiempo de bit y la tasa de transmisión de datos.
- Analizar los niveles y la estructura de una trama UART (bit de inicio, datos, paridad, bit de parada).
- Evaluar el efecto de la frecuencia de muestreo sobre la fidelidad de la decodificación.
- Programar la generación de tramas seriales en MicroPython.

## 🛠️ Equipo y herramientas

- Raspberry Pi Pico 2W
- Analizador lógico USB de 8 canales / 24 MHz
- Software **Logic 2** (Saleae)
- MicroPython / Thonny

## 📁 Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `Informe_Analizador_Logico.docx` | Informe completo del laboratorio (formato APA) |
| `Tabla_4_4_sensibilidad_muestreo.xlsx` | Tabla de sensibilidad al muestreo con fórmulas |
| `lab4/` | Capturas (.sal) y evidencias fotográficas del desarrollo |
| `analizador_logico.pdf` | Guía de laboratorio (Prof. José Rugeles) |

## 📊 Resultados principales

- Tiempo de bit medido a 9600 baudios: **104 µs** (teórico: 104.17 µs)
- Tiempo de transmisión del mensaje `UMNG_2026_LIDER_EN_TELECOMUNICACIONES` (37 caracteres): **≈ 38.54 ms**
- Se evaluó la sensibilidad al muestreo para **1200, 9600, 57600 y 115200 baudios**, con frecuencias de muestreo entre 25 kS/s y 12 MS/s, confirmando que errores relativos bajan de más del 100 % a menos del 5 % al superar el criterio N ≥ 10.

## 👤 Autor

**William Enrique Galvis Correa**
Estudiante de Ingeniería en Telecomunicaciones – UMNG

**Docente:** José Rugeles (jose.rugeles@unimilitar.edu.co)

## 📄 Licencia

Uso académico – UMNG, 2026.
