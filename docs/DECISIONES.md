# Decisiones

| Decisión | Por qué |
|---|---|
| Usar el repositorio `TR11` en vez de crear `dr-11` | La sesión no puede crear repositorios; `TR11` estaba vacío. Se puede renombrar en Settings |
| Pages y Release los activa el propietario | No hay herramienta para hacerlo desde la sesión |
| Un constructor + agente productor + agente QA (no 5 agentes) | Un solo archivo: 5 autores se pisan y gastan más |
| Licencia MIT | Simple y permisiva para un proyecto personal público |
| Una función `buildGraph` para directo y exportación | Garantiza que el WAV suene igual que la reproducción |
| Probabilidad con tirada determinista (compás, pista, paso) | Mismo resultado al reproducir desde el inicio y al exportar |
| Ruido e impulso de reverb con semilla fija | Mismo timbre en directo y en el WAV |
| El WAV usa la frecuencia de muestreo del dispositivo (44,1 kHz si no hay audio activo) | Evita diferencias de timbre entre directo y exportación |
| Deshacer por instantáneas del estado, 200 pasos | Cubre todas las acciones sin casos especiales; memoria acotada |
| Un arrastre de fader o de carril = un solo paso de deshacer | Evita cientos de pasos por gesto |
| Limitador = compresor rápido + recorte suave | Web Audio no tiene limitador real; nunca supera 0 dBFS |
| Mute/solo actúan sobre la ganancia de la pista | Efecto inmediato; un bombo silenciado no dispara sidechain |
| Rumble como capa sub sintetizada de ataque lento | Suena bien con poco coste; la cadena completa va en v0.2 |
| Hats con buffer metálico pregenerado | Mucho más barato en móvil que 6 osciladores por golpe |
| Faders horizontales | Los verticales fallan en táctil según navegador |
| Móvil: una pista, pads 8×2, carril y pestañas Pista/Efectos/Asistente | Todo cabe en una pantalla con pads de más de 40 px |
| 6 estilos en vez de 4 | El coste extra era mínimo |
| Mute, solo y estilo forman parte del patrón (y del deshacer) | Un solo modelo de datos, sin estados paralelos |
