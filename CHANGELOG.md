# Changelog

## v0.3.0 — 2026-11-15
Suena mejor y pesa menos.
- **Motor de audio nuevo:** cada sonido se genera una sola vez y después solo se reproduce. Cada golpe usa 2 nodos de audio en lugar de 4 a 10: menos consumo y menos riesgo de cortes en el móvil.
- **Niveles equilibrados automáticamente:** cambiar de sonido, kit, afinación o tono ya no descompensa la mezcla.
- **Rumble real:** el bombo pasa por una reverb oscura, un filtro de graves y saturación, y el sidechain lo hace respirar.
- **Bombo con más pegada** (segunda envolvente de tono) y 808 con armónicos para que se oiga en altavoces pequeños.
- **Hats, platos, caja y palmada con variaciones:** los golpes seguidos ya no suenan idénticos. La variación es la misma en el WAV.
- **Caja con más cuerpo** (resonancia en el ruido).
- **Drive por pista** (modo Avanzado): saturación de suave a agresiva.
- Aviso discreto en el medidor (marca naranja) si el audio llega justo.
- El WAV usa exactamente los mismos sonidos que la reproducción.

## v0.2.0 — 2026-11-15
Más sonidos, más fácil y mejor con los dedos.
- **Sonidos:** kits nuevos 606-style y 707-style, y de 6 a 8 sonidos con nombre por pista (88 en total) que se eligen con un toque y suenan al tocarlos.
- **Modo Simple** (por defecto) con lo esencial, y **Modo Avanzado** con todos los controles. Ayuda breve la primera vez y botón «?».
- **+ Energía / − Energía:** añade o quita instrumentos del groove en orden musical.
- **Vista «Tocar»:** 12 pads grandes para tocar con los dedos; con Grabar, lo que tocas se escribe cuantizado en el patrón.
- **Vista «Todas»** en el móvil: las 12 pistas a la vez; tocar una fila la abre.
- Pads de pasos más grandes en el móvil (4×4), botones de al menos 44 px y faders más gruesos.
- BPM con botones − / + y TAP para marcar el tempo; doble toque en un fader lo devuelve a su valor por defecto.
- Los estilos se eligen con botones; el swing pasa al panel de efectos (modo Avanzado).
- Las versiones anteriores quedan disponibles en `versiones/`.

## v0.1.0 — 2026-11-15
Primera versión.
- 12 pistas sintetizadas por código con dos kits (808-style y 909-style), elegibles por pista.
- Secuenciador de 16 pasos con acento, velocity y probabilidad por paso; BPM 60-200, swing, mute y solo.
- Por pista: volumen, pan, afinación, decay, tono y envíos a reverb y delay.
- Choke: el hat cerrado corta al abierto.
- Reverb (impulso generado), delay sincronizado al BPM, sidechain desde el bombo y limitador en el master.
- Asistente con 6 estilos (Berlin Warehouse, Hypnotic, Peak Time, Hard Techno, Dub Techno, Detroit): generar groove completo, sugerir patrón por pista y sonido del estilo.
- Deshacer/rehacer de todas las acciones, incluidas las del asistente (hasta 200 pasos).
- Guardado automático, patrones con nombre y exportación WAV de 16 bits idéntica a la reproducción.
- Interfaz en español e inglés, adaptada a móvil y escritorio.
