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

## v0.2.0: hechas en navegador sin interfaz
- Sin errores de consola en 1280×900 y 390×844 (táctil).
- Energía: de 8 pistas baja a 1 (solo bombo), sube a 12 y se deshace por completo.
- Grabar con pads escribe pasos en el patrón mientras suena.
- Kits 606 y 707 suenan en todas las pistas probadas; exportación idéntica entre renders; 0 pasos tarde a 150 BPM.

## v0.2.0: pendientes de probar a mano (móvil)
1. Vista «Tocar»: ¿responden los pads al instante? ¿Se pueden tocar dos a la vez?
2. Grabar: ¿los golpes caen donde esperas?
3. Faders: ¿se arrastran bien con el dedo sin mover la página? ¿Funciona el doble toque?
4. Modo Simple: ¿se entiende sin leer nada más que la ayuda inicial?

## v0.3.0: hechas en navegador sin interfaz
- Generar los 12 sonidos tarda unos 80 ms; 0 pasos tarde a 150 BPM.
- Niveles medidos por pista en los 4 kits: equilibrados entre kits.
- Exportación idéntica entre renders; pico máximo 0,92 con todo al máximo y drive a tope.

## v0.3.0: pendientes de probar a mano
1. Escuchar los 6 estilos en el móvil y con auriculares: ¿algún instrumento sobra o falta? (es lo que no puedo comprobar yo)
2. Rumble: ¿se nota el grave «respirando» entre bombos, sin tapar el bombo?
3. Mover Tono, Decay o Drive mientras suena: el cambio debe oírse casi al instante y sin cortes.
4. En un Android modesto, las 12 pistas a 150-200 BPM: ¿aparece la marca naranja en el medidor?

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
