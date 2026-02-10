# Prueba técnica: Sistema de motor de precios para E-commerce

## Tiempo límite: 35 minutos

---

## Contexto

Has sido asignado a un proyecto de e-commerce que presenta problemas críticos reportados por el cliente. La aplicación tiene una interfaz básica con un listado de productos y un sistema de cálculo de precios, pero **el código actual tiene errores y problemas de rendimiento**.

### Reporte del Cliente:

> _"Los totales del carrito no cuadran correctamente. Además, la página se vuelve muy lenta cuando agregamos productos o aplicamos cupones de descuento. Necesitamos que esto se solucione urgentemente antes del lanzamiento."_

---

## Objetivos de la prueba

Tu tarea es **analizar, depurar y optimizar** el código existente utilizando una herramienta de IA de tu preferencia como asistente (ChatGPT, Claude, Copilot, etc.).

---

## Tareas a Completar

### Tarea 1: Limpieza de datos

- Los precios de los productos están almacenados como strings con símbolos (ej: `'19.99$'`).
- **Debes convertirlos a números** para que los cálculos funcionen correctamente.
- Considera los problemas de precisión decimal en JavaScript.

### Tarea 2: Corregir Bug de Renderizado

- La función `renderCart()` tiene un bug que **duplica los productos** cada vez que se ejecuta.
- Identifica la causa y corrígela.

### Tarea 3: Optimizar Algoritmo de Descuentos

- La función `aplicarDescuento()` es extremadamente ineficiente.
- Actualmente usa bucles anidados innecesarios que causan lentitud.
- **Refactoriza el código** para mejorar su rendimiento sin complejidad algorítmica.

### Tarea 4: Implementar Lógica de Impuestos

- Existe una función vacía llamada `calcularImpuestosDinamicos(pais)`.
- **Implementa la lógica** para calcular impuestos según el país:

    | País      | Impuesto  | Tasa |
    | --------- | --------- | ---- |
    | España    | IVA       | 21%  |
    | México    | IVA       | 16%  |
    | Argentina | IVA       | 21%  |
    | USA       | Sales Tax | 7%   |
    | UK        | VAT       | 20%  |
    | Alemania  | MwSt      | 19%  |
    | Sin país  | Default   | 15%  |

### Tarea 5: Corregir Bug Visual

- El botón "Finalizar Compra" tiene un problema de visualización.
- Revisa el CSS y corrígelo.

---

## Entregables

1. **Código corregido**: Los 3 archivos (`index.html`, `styles.css`, `script.js`) con tus correcciones.

2. **CHAT.md** **OBLIGATORIO**:
    - Guarda tu conversación completa con la IA que utilizaste.
    - Puedes exportarla como archivo Markdown o incluir un enlace compartido al chat.
    - Este archivo es **fundamental** para evaluar cómo interactúas con herramientas de IA.

---

## Consejos

- Lee todo el código antes de empezar a hacer cambios.
- Usa la consola del navegador para identificar errores.
- No tengas miedo de pedirle a la IA que te explique conceptos que no entiendas.
- Prioriza las tareas: empieza por los bugs críticos.
- Si no alcanzas a completar todo, está bien. Queremos ver tu proceso de pensamiento.

---
