# TET App — Temporal Experience Tracing (versión compilada)

[🇬🇧 English](README.md) · 🇪🇸 Español

**Apps en línea: <https://gitorivera.github.io/tet-app/>**

- **TET-Kid** (con video): <https://gitorivera.github.io/tet-app/kid/>
- **TET** (sesión completa, sin video): <https://gitorivera.github.io/tet-app/tet/>

Este repositorio solo aloja las **versiones compiladas** de las apps de trazado TET, servidas con GitHub Pages. No contiene código fuente y se reemplaza en cada publicación. El código fuente está en otro repositorio privado de la investigación.

## ¿Qué es?

Dos aplicaciones web progresivas (PWA) usadas en un estudio de doctorado (Universidad Tecnológica de Pereira, Colombia) que compara el engagement de niños en un juego de rehabilitación cognitiva jugado en realidad mixta (Meta Quest) frente a tablet. Después de jugar, el niño traza cómo se sentía a lo largo del tiempo, una dimensión a la vez (Temporal Experience Tracing, adaptado de [Jachs et al., 2022](https://doi.org/10.1101/2022.03.04.482237)). En **TET-Kid** ve la grabación de su partida y traza mientras la mira; en **TET** ve el eje de toda la sesión y dibuja la curva de un tirón. Las trazas resultantes se alinean con el EEG registrado por Lab Streaming Layer.

## Cómo usarla

1. Abre el enlace de la app en Chrome en una tablet Android (o en cualquier navegador moderno).
2. Instálala: menú del navegador → **Instalar app** / **Agregar a la pantalla de inicio**. Cada app se instala aparte, con su propio ícono. Después de la primera carga funciona **sin conexión a internet**.
3. Como investigador, prepara la sesión y entrega la tablet al niño. En **TET-Kid** se escriben el código del participante y las dimensiones y se cargan el video del juego y el CSV de eventos. En **TET** no hay nada que escribir: se carga el **archivo de configuración** (un JSON con el participante, la duración de la sesión, los marcadores del eje, las dimensiones y el tiempo de LSL) que el investigador prepara en el PC de la captura.
4. Al final, descarga los archivos CSV/JSON o compártelos desde la tablet.

## Privacidad

Todo se ejecuta en el navegador. Los videos, las trazas y los datos de sesión se quedan **en el dispositivo** (IndexedDB / almacenamiento local) y nunca se suben a ningún servidor.

## Actualizaciones

Las copias instaladas se actualizan solas la próxima vez que se abre la app con conexión. Si aparece una versión vieja, cierra y vuelve a abrir la app.

## Licencia

[MIT](LICENSE) © 2026 Jorge Rivera.
