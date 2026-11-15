# Revisión crítica del encargo (única, antes de construir)

## Inviable tal como estaba escrito
- Crear el repositorio `dr-11`, activar Pages y crear la Release: la sesión solo tiene acceso al repositorio `TR11` y no dispone de herramientas para Pages ni Releases.
- "Sin desfases a 150 BPM en un móvil de gama media": no se puede verificar sin un móvil real. Se mide en navegador sin interfaz y queda como prueba manual.

## Contradicciones
- "El WAV suena igual que la reproducción" frente a la probabilidad por paso (aleatoria). Solución: tirada determinista por compás, pista y paso.
- "Deshacer ilimitado" frente a la memoria del móvil. Solución: historial de 200 pasos.
- "5 agentes en paralelo" frente a "un solo index.html" y "ahorro de tokens": se pisan y multiplican el coste.
- "Limitador en el master": Web Audio no trae un limitador real; se aproxima con compresor rápido y recorte suave.
- "Faders verticales" frente a "táctil": los rangos verticales son poco fiables entre navegadores.

## Qué sobra en la v0.1.0
- Revisión crítica con 2-3 agentes: basta una pasada.
- Rumble como cadena de reverb + filtro + sidechain propia: se sustituye por una capa sub sintetizada.

## Qué faltaba
- Qué longitud tiene el WAV exportado (se elige: 1-16 compases, más cola).
- Qué ocurre al primer arranque (se carga un groove base para sonar al primer toque).
- Aviso del modo silencio de iPhone.
- Lista de pruebas manuales por dispositivo (`docs/PRUEBAS.md`).

## Opinión por rol
- **Productor:** un bombo, hats y clap que suenen bien valen más que 10 estilos; el sidechain y el rumble son lo que hace que suene a techno, así que entran desde el principio.
- **Ingeniero:** el riesgo real es la paridad directo/exportación y el reloj; por eso una sola función construye la cadena de audio y otra programa cada paso, y ambas se usan en los dos casos.
