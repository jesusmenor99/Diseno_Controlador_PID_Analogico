# Diseño de un Controlador PID Analógico con Amplificadores Operacionales
Diseño de un Controlador PID Analógico con Amplificadores Operacionales para un Sistema de Posicionamiento de Ascensor.
# Controlador PID Analógico para Posicionamiento de Ascensor | LM741 + Etapa Push-Pull


> Diseño, simulación e implementación de un sistema de control de posición analógico para ascensor, utilizando amplificadores operacionales LM741, inspirado en técnicas de control para convertidores DC-DC.
>
> **Unidades Tecnológicas de Santander (UTS) - 2025**

---

## 📌 Descripción General

Este proyecto implementa un **sistema de control de posición analógico** para un ascensor a escala, utilizando exclusivamente componentes analógicos:

- **Controlador Proporcional (P)** basado en amplificadores operacionales LM741
- **Etapa restadora** para calcular la señal de error
- **Etapa de potencia push-pull** (TIP41C + TIP32C) para manejar el motor DC
- **Sensor de posición** (potenciómetro lineal de 10kΩ) acoplado mecánicamente

El sistema logra posicionar el motor con un **error en estado estacionario del 2.39%** utilizando una ganancia proporcional Kp = 10, demostrando la viabilidad del control analógico para aplicaciones de posicionamiento.

---

## 🎯 Objetivo del Proyecto

Diseñar, simular e implementar un lazo de control de posición analógico utilizando amplificadores operacionales LM741, que permita controlar la dirección y posición de un motor DC (simulando un ascensor), sentando las bases para la implementación de un controlador PID analógico completo.

---

## ⚙️ Tecnologías y Componentes

| Categoría | Componente | Especificación |
|-----------|------------|----------------|
| **Amplificadores operacionales** | LM741 ×3 | Compensado internamente, ±12V de alimentación |
| **Etapa de potencia** | TIP41C + TIP32C | Par complementario NPN/PNP (push-pull) |
| **Sensor de posición** | Potenciómetro lineal | 10kΩ, acoplado al eje del motor |
| **Actuador** | Motor DC | 12V, control por polarización |
| **Resistencias** | Varios valores | 270kΩ, 39kΩ, 10kΩ, 1kΩ |
| **Herramientas de simulación** | PsPice, MATLAB | Análisis transitorio y sintonización |
| **Implementación** | Protoboard | Fuente de alimentación dual ±12V |

---



El circuito de control consta de **tres etapas principales** implementadas con LM741:
