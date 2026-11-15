# DR-11 · caja de ritmos de techno en el navegador

Caja de ritmos de 12 pistas con kits sintetizados, secuenciador de 16 pasos y un asistente que sugiere patrones por estilo. Todo en un único `index.html`: sin instalación, sin servidor, sin conexión y sin subir tu audio a ningún sitio.

**Versión:** 0.1.0 · **Licencia:** MIT

## Cómo usarla
- **Online:** abre la web publicada en GitHub Pages (enlace en la descripción del repositorio).
- **Sin conexión:** descarga `index.html` y ábrelo en tu navegador.
- En iPhone, quita el modo silencio (interruptor lateral) o no sonará.

## En 30 segundos
1. Pulsa **▶** (el primer toque activa el audio).
2. En **Asistente**, elige un estilo y pulsa **Generar groove completo**.
3. Toca los pads para activar o quitar pasos. **Sugerir** propone otro patrón para la pista seleccionada.

## Controles
| Zona | Qué hace |
|---|---|
| Cabecera | Play/stop, BPM (60-200), swing, medidor, deshacer/rehacer, patrones, exportar WAV, idioma |
| Rejilla | 12 pistas × 16 pasos. **M** mute, **S** solo. Tocar el nombre selecciona la pista y la hace sonar |
| Toque: Nota / Acento | Qué hace un toque sobre un pad: activar el paso o marcarlo con acento |
| Carril: Velocity / Prob. | Arrastra las barras para dibujar la fuerza o la probabilidad de cada paso |
| Pista | Kit (808-style / 909-style), volumen, pan, afinación, decay, tono, envíos a reverb y delay |
| Efectos | Reverb, delay sincronizado al BPM, feedback, sidechain y volumen master (con limitador) |
| Asistente | Estilo, generar groove, sugerir patrón y aplicar el sonido del estilo a la pista |

Atajos de teclado: `Espacio` play/stop · `Ctrl/Cmd+Z` deshacer · `Ctrl/Cmd+Shift+Z` rehacer.

En el móvil se ve una pista cada vez: cámbiala con la fila de botones de colores.

## Pistas
BD bombo · RB rumble · SD caja · LT/MT/HT toms · RS rimshot · CP palmada · CH hat cerrado · OH hat abierto (CH lo corta) · CC crash · RC ride.

## Guardado
Tu patrón se guarda solo en el navegador (localStorage). En **Patrones** puedes guardar varios con nombre, cargarlos o borrarlos. **WAV** exporta 1-16 compases en estéreo de 16 bits y suena igual que la reproducción.

## Documentación del proyecto
`docs/REVISION.md` · `docs/PLAN.md` · `docs/DECISIONES.md` · `docs/PREGUNTAS.md` · `docs/PRUEBAS.md` · `CHANGELOG.md`
