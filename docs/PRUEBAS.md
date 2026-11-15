# Pruebas

## Hechas en navegador sin interfaz (Chromium, 1280×800 y 390×844)
- Sin errores de consola al pulsar todos los botones; cero peticiones de red.
- Un solo AudioContext; ningún `setInterval`.
- Reproducción a 150 BPM y con cambio de BPM en marcha: 0 pasos programados tarde.
- Exportación repetida con probabilidad < 100: resultado idéntico (diferencia ~1e-7).
- WAV: descarga y cabecera correctas. Pico máximo 0,92 con todo al máximo (no recorta).
- Choke CH→OH, sidechain, mute/solo y pan correctos en el render.
- Un arrastre de fader, swing o carril = un solo paso de deshacer.
- Guardar, cargar y borrar patrones; el patrón y el idioma persisten al recargar.

## Pendientes de probar a mano
### iPhone (Safari)
1. Primer toque en ▶ y en el nombre de una pista: ¿suena a la primera? ¿Y con el interruptor de silencio puesto?
2. Tocar el campo BPM, los desplegables y el nombre de patrón: la página no debe hacer zoom.
3. Exportar WAV de 4 y de 16 compases: ¿se guarda el archivo o se abre un reproductor?
4. Bloquear la pantalla o recibir una llamada mientras suena y volver: ¿se recupera el audio?
### Android (Chrome)
1. Deslizar la página empezando sobre los pads y sobre los faders: no deben cambiar pasos por error.
2. Las 12 pistas llenas a 150-200 BPM: ¿hay cortes o desfases?
3. Exportar WAV y abrirlo.
### Ordenador
1. Comparar de oído la reproducción con el WAV exportado.
2. Atajos: Espacio, Ctrl/Cmd+Z y Ctrl/Cmd+Shift+Z.
3. Firefox y Safari: carga, sonido y exportación (solo se ha probado Chromium).
