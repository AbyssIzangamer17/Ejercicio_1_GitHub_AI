# Bitácora de Desarrollo: EcoSort-AI

## Ejercicio 1.0 — Sistema Inteligente de Clasificación de Residuos

---

### Descripción del Proyecto

El proyecto consiste en la creación de un sistema de simulación industrial de clasificación de residuos en una cinta transportadora. Los objetos llegan a la línea de escaneo y se identifican mediante visión artificial simulada, derivándose automáticamente a la tolva correspondiente según su material.

---

### Prompt de Origen

**Fuente:** PDF de Instrucciones del Ejercicio (Captura 2026-02-24)

**Prompt original:**
> "Exercici 1. Projecte únic independent. Presentació del producte en format adequat per a la seva utilització com a exemple."

Este prompt establece que el Ejercicio 1 debe ser un proyecto único e independiente, presentado de forma adecuada para su utilización como ejemplo.

---

### Prompts Utilizados

#### Prompt #1
**Prompt:** "El ejercicio 1 no es capaz de simular ni de verse absolutamente nada."

**Para qué sirve:** Se detectó que el proyecto inicial carecía de cualquier funcionalidad visual o simulación. Este prompt fue el punto de partida para transformar el ejercicio en EcoSort-AI, un sistema de cinta transportadora con objetos en movimiento.

**Corrección:** Sí — Se utilizó para corregir la falta total de implementación visual del proyecto.

---

#### Prompt #2
**Prompt:** "El ejercicio 1 tiene que saber de qué material es una vez haya pasado la línea, no antes. Como si cruzara un sensor."

**Para qué sirve:** Implementé la lógica de identificación POST-scan. Los objetos aparecen inicialmente como bloques grises con "?" (desconocidos) y solo revelan su material cuando cruzan la línea del sensor en el punto exacto de clasificación.

**Corrección:** Sí — Se utilizó para corregir la lógica de identificación, pasando de identificación inmediata a identificación en el punto exacto de clasificación.

---

#### Prompt #3
**Prompt:** "Del Ecosort tienes que mejorar el hecho de en que tolva es depositado porque caen de forma aleatoria sin ser clasificados."

**Para qué sirve:** Se implementó la derivación automática a tolvas. Cada objeto ahora se desvía horizontalmente hacia su tolva correcta después del escaneo: Plástico a la tolva izquierda, Metal al centro y Cartón a la derecha, con animación fluida.

**Corrección:** Sí — Este prompt corrigió el error de derivación aleatoria, asegurando que cada material vaya a su tolva correspondiente.

---

#### Prompt #4
**Prompt:** "Del ejercicio 1 está perfecto."

**Para qué sirve:** El proyecto llegó a su versión final estable (v5). El sistema incluye todos los componentes funcionando: cinta transportadora animada, línea de sensor de identificación, identificación POST-scan, derivación a tolvas con animación, panel de control con estadísticas y registro de eventos.

**Corrección:** No — Este prompt marcó la aprobación final del proyecto sin correcciones.

---

### Resumen de Funcionalidades

| Funcionalidad | Descripción |
|--------------|-------------|
| Cinta Transportadora | Simulación visual con objetos en movimiento vertical |
| Sensor de Identificación | Línea verde que actúa como punto de escaneo |
| Identificación POST-scan | Objetos desconocidos (?) hasta cruzar el sensor |
| Derivación a Tolvas | Clasificación automática: Plástico, Metal, Cartón |
| Estadísticas | Contadores en tiempo real por categoría |
| Panel de Control | Botones de inicio/parada y log de eventos |

---

### Conclusión

EcoSort-AI se consolidó como un proyecto independiente, útil y visualmente atractivo que demuestra conceptos de automatización industrial real: sensores inline, derivación neumática simulada, SCADA visual y trazabilidad de procesos.

---

*Documento realizado por Izan Urios — 3R de Automatización y Robótica Industrial*
