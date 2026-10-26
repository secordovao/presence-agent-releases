# Alliance Presence agent (Windows)

Registro de entrada, salida y adherencia para Alliance BPO Services.

**Descarga:** la versión actual está en [Releases](https://github.com/secordovao/presence-agent-releases/releases/latest)
(`presence-agent.exe`). Este repositorio solo contiene los instaladores; el código está en un repositorio privado.

## Instalación (3 minutos)

1. Descarga `presence-agent.exe`.
2. Ejecútalo con `--install` (o doble clic): se copia a `%LOCALAPPDATA%\AlliancePresence`, se registra en el
   arranque de tu usuario y abre la página de inicio de sesión en `http://127.0.0.1:47321/`.
   Windows SmartScreen puede pedir "Más información → Ejecutar de todas formas" mientras el binario no esté firmado.
3. Pega el código de registro que te dio tu director.
4. Entra con tu número de empleado y PIN.

## Qué registra

Durante tu horario: entrada y salida, la aplicación que tienes al frente y el título de su ventana, el tiempo sin
actividad y si el micrófono está en uso. No graba pantalla, teclas ni contenido. Fuera de una sesión iniciada solo
se registra que la PC está encendida.

El agente se actualiza solo. Para desinstalar: `presence-agent.exe --uninstall`.
