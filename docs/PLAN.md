# Plan por fases

## v0.1.0 (publicada) — instrumento usable
12 pistas, kits 808/909-style, 16 pasos con acento/velocity/probabilidad, BPM, swing, mute/solo, parámetros por pista, choke CH→OH, reverb, delay, sidechain, limitador, 6 estilos con Sugerir y Generar groove, deshacer/rehacer, guardar/cargar patrones, WAV, ES/EN, móvil.

## v0.2 — profundidad de secuenciador y sonido
- Kits 606-style y 707-style; drive por pista.
- Rumble real: bombo → reverb → pasa-bajos → sidechain, con canal propio.
- 32 y 64 pasos, longitud por pista (polimetría), ratchet/flam, micro-desplazamiento.
- Patrones A/B/C/D y cadena; exportar/importar patrón como JSON.
- Asistente: Variar, densidad, candado, Fill, Más/Menos energía, Humanizar; 4 estilos más (Acid, Minimal, Industrial, Melodic).
- WAV de 24 bits.

## v0.3 — samples y master
- Samples propios (WAV/MP3, edición básica, IndexedDB), kits de usuario.
- Master: EQ de 3 bandas, compresor, medidor RMS.
- Bloqueo de parámetros por paso; generador euclidiano; aleatorizar.
- Stems y exportación MIDI.

## v0.4 — asistente completo
- Modo Guía, consejos en vivo (clip, choque de graves, afinación del bombo), "Guardar como Mi estilo", comparación A/B.

## Frentes abiertos
| # | Frente | ¿Lo haría? | Versión | Por qué |
|---|---|---|---|---|
| 1 | Pads en directo con grabación cuantizada | Sí | v0.2 | Barato y hace el instrumento más divertido |
| 2 | Modo actuación (mutes, scatter, cambio al final del compás) | Sí | v0.3 | Necesita antes patrones A/B/C/D |
| 3 | Pista de bajo tipo acid | Sí | v0.4 | Completa el track, pero es otro instrumento entero |
| 4 | Planificador de arreglo de 6-8 min | Sí, simple | v0.4 | Depende de la cadena de patrones |
| 5 | Web MIDI | Solo escritorio/Android | v0.5 | No funciona en iOS Safari |
| 6 | IA con clave del usuario | No por ahora | — | Rompe "sin red" y aporta poco frente a los estilos |
| 7 | Grabar la actuación a WAV | Sí | v0.3 | Junto al modo actuación |
| 8 | LFO/envolventes al tempo | Sí | v0.4 | Tras el bloqueo de parámetros por paso |
| 9 | Analizador de track de referencia | Quizá | v0.5+ | Útil pero lejos del núcleo |
| 10 | Quitaría | ZIP sin librerías | — | Mucho código para poco valor; basta JSON |
