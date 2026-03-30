# Changelog

Todas las versiones notables de LŌU Brew Calibration.

Formato basado en [Keep a Changelog](https://keepachangelog.com/es-ES/1.0.0/).
Versionamiento semántico: `vMAJOR.MINOR.PATCH`

## [v0.4.0] - 2026-03-29

### Agregado
- Motor de calibración inteligente: compara shot actual vs anterior, detecta qué variable cambió y explica el impacto sensorial
- Sugerencias contextuales que cruzan cambios de parámetros con notas de sabor
- Alerta cuando se modifican múltiples variables simultáneamente
- Imágenes de marca con fondo transparente (logo + emblema)

### Corregido
- Loading fallback cuando `window.storage` no está disponible

### Cambiado
- Sugerencias de calibración ahora son detalladas y educativas en lugar de genéricas

## [v0.3.0] - 2026-03-29

### Agregado
- Generación de reporte en PDF con jsPDF
- PDF con branding completo: header, promedios, mejor shot, gráfica de progresión, historial en tabla
- Footer con dirección y @loubrewbar
- Web Share API para compartir PDF directamente en móvil
- Edición de shots guardados (mantiene timestamp original)
- Ícono de edición (lápiz) junto a cada shot en el historial

## [v0.2.0] - 2026-03-29

### Agregado
- Campo de molienda para Victoria Arduino Mythos 1 (dial micrométrico 0-10)
- Campo de productor/tostador
- Campo de nombre personalizado para el grano
- Rating con medios puntos (click en mitad izquierda = 0.5, derecha = entero)
- Pre-llenado de parámetros desde último shot

### Corregido
- Inputs perdían foco al escribir (componentes inline + functional setState)
- Imágenes base64 se corrompían al pasar por bash

### Cambiado
- Tipografía de labels a Oswald weight 800 (sustituto de Monument Extended)
- Sugerencias de Mythos referencian ajustes de dial específicos

## [v0.1.0] - 2026-03-29

### Agregado
- Gestión de granos por lote (variedad, tueste, proceso, fecha)
- Registro de shot en 3 pasos (parámetros, sensorial, resumen)
- 10 notas negativas + 10 positivas como tags seleccionables
- Rating de 1-5 estrellas
- Motor de sugerencias básico por notas sensoriales
- Historial de shots con eliminación
- Reporte de lote compartible (texto plano)
- Cierre de lote y archivo
- Persistencia en localStorage
- Navegación: Granos, Agregar (+), Archivo
- Paleta de marca LŌU (Negro Opaco, Blanco Beige, Verde Olivo, Rojo Sombrerete, Azul Gris)
- Tipografías Oswald + Inconsolata via Google Fonts
