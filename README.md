# ♻️ EcoSort-AI — Sistema Inteligente de Clasificación de Residuos

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5&logoColor=white)](https://developer.mozilla.org/es/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?logo=javascript&logoColor=black)](https://developer.mozilla.org/es/docs/Web/JavaScript)
[![Canvas API](https://img.shields.io/badge/Canvas-API-orange)](https://developer.mozilla.org/es/docs/Web/API/Canvas_API)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)

> **Ejercicio 1** — Proyecto único e independiente de alta utilidad industrial.

EcoSort-AI es una simulación interactiva de un sistema de clasificación de residuos en cinta transportadora, diseñada para demostrar cómo la Inteligencia Artificial puede integrarse en procesos de reciclaje industrial automatizado.

---

## 🎯 Objetivo del Proyecto

Desarrollar un sistema visual que demuestre el proceso completo de clasificación automatizada de residuos industriales, desde la detección hasta la derivación a la tolva correspondiente, integrando conceptos de visión artificial, sensores en línea y actuadores de derivación.

---

## 🚀 Características Principales

### Cinta Transportadora Animada
- Simulación visual de una cinta industrial con carriles marcados.
- Objetos que se desplazan verticalmente a velocidad constante.
- Animación fluida a 60 FPS mediante `requestAnimationFrame`.

### Sensor IA de Identificación
- **Línea de escaneo verde** que actúa como punto de identificación.
- Los objetos llegan como **bloques grises con "?"** (desconocidos).
- La identificación ocurre **únicamente al cruzar la línea del sensor**, no antes.
- Al pasar el sensor: se revela el icono, la etiqueta del material y el color de identificación.

### Derivación a Tolvas
- Tras la identificación, cada objeto se **desvía horizontalmente** hacia la tolva correcta:
  - ♻️ **Plástico** (izquierda) — Botellas PET, envases HDPE
  - 🔩 **Metal** (centro) — Latas de aluminio, tornillos
  - 📦 **Cartón** (derecha) — Cajas de cartón
- La derivación se realiza con una transición CSS suave de 0.7 segundos.
- Cada tolva tiene su **contador individual** actualizado en vivo.

### Panel de Control
- Estadísticas en tiempo real por categoría (Plástico, Metal, Cartón, Total).
- Botón de activación/desactivación de la línea.
- Registro de eventos con timestamps.

---

## 📋 Tipos de Objetos Detectados

| Icono | Material | Categoría | Tolva |
|-------|----------|-----------|-------|
| 🥤 | Botella PET | Plástico | Izquierda |
| 🧴 | Envase HDPE | Plástico | Izquierda |
| 🥫 | Lata Aluminio | Metal | Centro |
| 🔩 | Tornillo FE | Metal | Centro |
| 📦 | Caja Cartón | Cartón | Derecha |

---

## 🛠️ Tecnologías Utilizadas

| Tecnología | Uso |
|------------|-----|
| **HTML5** | Estructura de la aplicación |
| **CSS3** | Diseño visual, animaciones y transiciones |
| **JavaScript ES6+** | Lógica de simulación, spawning, detección |
| **DOM Manipulation** | Creación dinámica de objetos y actualización de UI |
| **CSS Transitions** | Derivación suave de objetos a tolvas |

---

## 🚀 Inicio Rápido

### Opción 1: Abrir directamente
```
Abrir ecosort_ai.html en cualquier navegador moderno
```

### Opción 2: Clonar repositorio
```bash
git clone https://github.com/AbyssIzangamer17/Ejercicio_1_GitHub_AI.git
cd Ejercicio_1_GitHub_AI
# Abrir ecosort_ai.html en el navegador
```

### Uso
1. Pulsa **ACTIVAR LÍNEA** para iniciar la cinta transportadora.
2. Observa cómo los objetos llegan como bloques desconocidos (?).
3. Al cruzar la línea verde del sensor, se identifican y desvían a su tolva.
4. Consulta las estadísticas y el log en tiempo real.
5. Pulsa **DETENER LÍNEA** para pausar la simulación.

---

## 📁 Estructura del Proyecto

```
Ejercicio_1_GitHub_AI/
├── ecosort_ai.html     # Aplicación principal (simulación completa)
└── README.md           # Este archivo
```

---

## 🔬 Conceptos Industriales Aplicados

- **Sensores inline**: Detección de materiales en el punto exacto de clasificación.
- **Derivación neumática**: Simulación de actuadores que desvían objetos a tolvas.
- **SCADA visual**: Panel de control con métricas en tiempo real.
- **Trazabilidad**: Registro de cada objeto procesado con timestamp.

---

## 👤 Autor

**Izan Urios** — 3R de Automatización y Robótica Industrial

---

## 📄 Licencia

Proyecto de código abierto bajo licencia **MIT**.
