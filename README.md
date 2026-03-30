# LŌU Brew Calibration

Herramienta de calibración de espresso para **LŌU Brew Bar** — Sombrerete 522, Col. Condesa, CDMX.

Aplicación standalone (HTML/React) diseñada para reducir mermas, mejorar el flujo de calibración y entrenar baristas en la toma de decisiones de extracción.

## Funcionalidades

**Gestión por grano/lote**
- Registro de variedad, nombre personalizado, productor/tostador, tipo de tueste, proceso y fecha de tueste
- Cálculo automático de días de reposo
- Historial completo de shots por grano
- Cierre de lote con generación de reporte

**Registro de shot (3 pasos)**
- Parámetros: dosis entrada/salida, temperatura, tiempo, molienda (Mythos 1, dial 0-10), preinfusión con pausa
- Evaluación sensorial: 10 notas negativas + 10 positivas
- Rating con medios puntos (0.5 - 5.0)
- Pre-llenado desde último shot para agilizar registro

**Motor de calibración inteligente**
- Compara shot actual vs anterior: detecta qué variable cambió más y explica el impacto en sabor
- Diagnóstico cruzado: combina cambios de parámetros con notas sensoriales
- Sugerencias específicas para Victoria Arduino Mythos 1
- Alerta cuando se cambian múltiples variables simultáneamente

**Reporte PDF para tostador**
- Generación con jsPDF y branding LŌU
- Promedios, mejor shot, notas frecuentes, gráfica de progresión
- Recomendaciones contextuales para ajuste de perfil de tueste
- Historial completo en tabla
- Compartible vía Web Share API o descarga directa

**Edición de shots**
- Modificar cualquier shot guardado manteniendo su timestamp original

## Stack

- React 18 (via CDN + Babel standalone)
- jsPDF para generación de reportes PDF
- localStorage para persistencia
- Google Fonts: Oswald + Inconsolata
- Cero dependencias de build — archivo HTML autocontenido

## Uso

Abrir `index.html` en cualquier navegador. Funciona offline después de la primera carga de fuentes.

Para uso móvil: agregar a pantalla de inicio desde Safari/Chrome para experiencia de app nativa.

## Branding

Paleta de LŌU Brew Bar diseñada por VVORKROOM:
- Negro Opaco `#191919`
- Blanco Beige `#E2DED5`
- Verde Olivo `#383A31`
- Rojo Sombrerete `#DF3B3A`
- Azul Gris `#939DA5`

Tipografías: Oswald (sustituto web de Monument Extended Ultrabold) + Inconsolata.

## Roadmap

- [ ] Corregir renderizado de imágenes de marca (logo + emblema)
- [ ] Backend con Supabase/Antigravity para multi-usuario
- [ ] Login por barista con historial individual
- [ ] Dashboard de administrador
- [ ] Notificaciones de reposo de grano
- [ ] Export CSV del historial

## Licencia

Uso interno LŌU Brew Bar. Todos los activos de marca son propiedad de LŌU / VVORKROOM.

---

**@loubrewbar** · Instagram · TikTok
