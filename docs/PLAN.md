# Plan por fases

## v0.1.0 (publicada) — instrumento usable
12 pistas, kits 808/909-style, 16 pasos con acento/velocity/probabilidad, BPM, swing, mute/solo, parámetros por pista, choke CH→OH, reverb, delay, sidechain, limitador, 6 estilos con Sugerir y Generar groove, deshacer/rehacer, guardar/cargar patrones, WAV, ES/EN, móvil.

## v0.2.0 (publicada) — sonidos, facilidad y táctil
Kits 606/707-style, 88 presets de sonido por pista, modo Simple/Avanzado con ayuda inicial, + / − energía, vista Tocar con grabación cuantizada, vista Todas en móvil, pads 4×4, faders gruesos, BPM − / + y TAP.

## v0.3.0 (publicada) — sonido y rendimiento de audio
Sonidos pre-renderizados y normalizados, rumble real, bombo con pegada, variaciones por golpe, drive por pista, aviso de carga.

## v0.4 — mezcla y master
- Limitador con anticipación (AudioWorklet), compresor de bus, EQ de 3 bandas, graves en mono, sidechain por pista, dos tamaños de reverb.

## v0.5 — visual
- Repintado selectivo, cabecera de una fila en móvil, pads con la fuerza visible, destello por pista, medidores por pista, forma de onda del sonido.

## Después — profundidad de secuenciador
- 32 y 64 pasos, longitud por pista (polimetría), ratchet/flam, micro-desplazamiento.
- Patrones A/B/C/D y cadena; exportar/importar patrón como JSON.
- Asistente: Variar, densidad, candado, Fill, Más/Menos energía, Humanizar; 4 estilos más (Acid, Minimal, Industrial, Melodic).
- WAV de 24 bits.

## Después — samples
- Samples propios (WAV/MP3, edición básica, IndexedDB), kits de usuario.
- Master: EQ de 3 bandas, compresor, medidor RMS.
- Bloqueo de parámetros por paso; generador euclidiano; aleatorizar.
- Stems y exportación MIDI.

## Después — asistente completo
- Modo Guía, consejos en vivo (clip, choque de graves, afinación del bombo), "Guardar como Mi estilo", comparación A/B.

## Frentes abiertos
| # | Frente | ¿Lo haría? | Versión | Por qué |
|---|---|---|---|---|
| 1 | Pads en directo con grabación cuantizada | Hecho | v0.2.0 | Barato y hace el instrumento más divertido |
| 2 | Modo actuación (mutes, scatter, cambio al final del compás) | Sí | v0.3 | Necesita antes patrones A/B/C/D |
| 3 | Pista de bajo tipo acid | Sí | v0.4 | Completa el track, pero es otro instrumento entero |
| 4 | Planificador de arreglo de 6-8 min | Sí, simple | v0.4 | Depende de la cadena de patrones |
| 5 | Web MIDI | Solo escritorio/Android | v0.5 | No funciona en iOS Safari |
| 6 | IA con clave del usuario | No por ahora | — | Rompe "sin red" y aporta poco frente a los estilos |
| 7 | Grabar la actuación a WAV | Sí | v0.3 | Junto al modo actuación |
| 8 | LFO/envolventes al tempo | Sí | v0.4 | Tras el bloqueo de parámetros por paso |
| 9 | Analizador de track de referencia | Quizá | v0.5+ | Útil pero lejos del núcleo |
| 10 | Quitaría | ZIP sin librerías | — | Mucho código para poco valor; basta JSON |
