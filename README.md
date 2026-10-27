# Alliance Presence agent (Windows)

Registro de entrada, salida y adherencia para Alliance BPO Services.

**Descarga:** la versión actual está en [Releases](https://github.com/secordovao/presence-agent-releases/releases/latest)
(`presence-agent.exe`). Este repositorio solo contiene los instaladores; el código está en un repositorio privado.

## Instalación (2 minutos)

1. Descarga `presence-agent.exe`.
2. Ábrelo con doble clic. Se instala solo: se copia a `%LOCALAPPDATA%\AlliancePresence`, se registra en el
   arranque de tu usuario, crea "Alliance Presence" en el menú Inicio y abre la ventana de la aplicación.
   Windows SmartScreen puede pedir "Más información → Ejecutar de todas formas" mientras el binario no esté firmado.
3. En la ventana, pega el código de registro que te dio tu director (una sola vez por computadora).
4. Entra con tu número de empleado y PIN. La aplicación está en inglés.

Para abrirla después: menú Inicio → "Alliance Presence", o el icono junto al reloj → "Open Alliance Presence".
Para instalar una versión nueva basta con abrir el archivo descargado: reemplaza la anterior sin cerrar tu sesión.

## Qué registra

Durante tu horario y solo con sesión iniciada: entrada y salida, la aplicación que tienes al frente y el título de su
ventana (según la política de tu campaña, con números largos y correos ocultos), el tiempo sin actividad y si el
micrófono está en uso. No graba pantalla, teclas ni contenido. Sin sesión solo se registra que la PC está encendida.
Bloquear la computadora (Win+L) cierra tu sesión.

El agente se actualiza solo. Para desinstalar: `presence-agent.exe --uninstall`.
