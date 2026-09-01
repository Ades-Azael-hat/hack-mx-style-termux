# hack-mx-style-termux

![hack-mx-banner](awesome_hacking.svg)

Versión adaptada para Termux (Android) en español (es‑MX).

Basado en: https://github.com/Ades-Azael-hat/Hack-mx-style

Objetivo
- Crear una versión propia y optimizada para ejecutarse y usarse desde Termux en Android.
- Documentación completa en español (es‑MX) con pasos claros para instalación y uso.
- Scripts y recomendaciones específicas para Termux.

Advertencia y uso responsable
Este proyecto es para uso educativo y legal. No fomentes ni realices actividades ilegales o no éticas. El autor y colaboradores no se hacen responsables por el uso indebido.

Créditos y adaptación
- Autores originales: BOCHMEN3 y chukys
- Adaptación y mantenimiento: AZAEL ARREDONDO (alias Ad3x)
- Contacto: bochmen3@gmail.com

Nota de adaptación
"Con cariño y éxito para mí gran hat azael" — Ad3x

Licencia
Este proyecto se publica bajo la licencia MIT. Consulta el archivo LICENSE para más detalles.

Requisitos mínimos (en Termux)
- Termux actualizado desde F-Droid o Termux app (no desde Play Store si está desactualizada).
- Conexión a Internet.
- Espacio suficiente para instalar dependencias.

Instalación paso a paso (Termux)
1) Actualiza Termux y los paquetes base:

   pkg update && pkg upgrade -y

2) Instala herramientas básicas (ejemplo recomendado):

   pkg install git python nodejs wget curl unzip -y

   - Si necesitas compiladores o herramientas de construcción:
     pkg install build-essential -y

3) (Opcional) Da acceso al almacenamiento interno (si vas a guardar archivos fuera del directorio de Termux):

   termux-setup-storage

   Acepta los permisos cuando el sistema lo solicite.

4) Clona este repositorio y cambia a la rama de adaptación:

   git clone https://github.com/Ades-Azael-hat/hack-mx-style-termux.git
   cd hack-mx-style-termux
   git checkout termux/adaptacion

5) Instala dependencias del proyecto (si existen)

- Si el proyecto usa Python y tiene requirements.txt:

   pip3 install --user -r requirements.txt

  O para entorno aislado:

   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt

- Si usa Node.js:

   npm install

Uso y ejemplos (Termux)
- Ejecutar scripts shell incluidos:

   sh scripts/ejemplo.sh

- Ejecutar un script Python:

   python3 scripts/ejemplo.py

- Ejecutar comandos Node:

   node scripts/ejemplo.js

Consejos para Termux
- Si un script requiere acceso a la tarjeta SD o archivos externos, asegúrate de ejecutar `termux-setup-storage` y otorgar permisos.
- Algunas dependencias necesitan compilación: instala `build-essential` y `clang` si es necesario.
- Para ejecutar servicios en segundo plano usa `nohup comando &` o `tmux` (si instalas `pkg install tmux`).
- Para editar rápidamente archivos puedes usar `nano`, `vim` o `micro` (`pkg install nano`).

Estructura propuesta del repositorio
- README.md — documentación principal (este archivo)
- LICENSE — licencia MIT
- contributing.md — cómo contribuir
- CODE_OF_CONDUCT.md
- SECURITY.md
- .github/ — templates y workflows
- scripts/ — carpeta recomendada para scripts compatibles con Termux
- examples/ — ejemplos de uso y pruebas

Buenas prácticas
- No subas credenciales ni información sensible.
- Documenta los scripts y su propósito en comentarios.
- Prueba los scripts en una instalación limpia de Termux antes de publicar.

Pruebas locales (comandos útiles en Termux)
- Actualizar e instalar paquetes:

   pkg update && pkg upgrade -y
   pkg install git python nodejs -y

- Clonar y cambiar rama:

   git clone https://github.com/Ades-Azael-hat/hack-mx-style-termux.git
   cd hack-mx-style-termux
   git checkout termux/adaptacion

- Ejecutar verificación rápida (si incluyes scripts de prueba):

   sh scripts/test.sh

Siguientes pasos que voy a realizar
1) Traducir y adaptar el resto de la documentación y comentarios seguros en el código, en commits separados.
2) Revisar scripts y ajustar shebangs y permisos para que funcionen en Termux (por ejemplo `#!/data/data/com.termux/files/usr/bin/sh` si hace falta, o usar `#!/usr/bin/env sh`).
3) Intentar traducir cadenas y textos internos si es seguro (te avisaré antes de cambios intrusivos).
4) Mantener la rama `termux/adaptacion` con commits claros y te avisaré cuando abra un PR para revisión final.

Cómo revisar y abrir el Pull Request
- URL del repositorio: https://github.com/Ades-Azael-hat/hack-mx-style-termux
- Rama con cambios: termux/adaptacion

Para abrir el PR desde la web:
1. Ve a la página del repo
2. Cambia a la rama "termux/adaptacion"
3. Haz clic en "Compare & pull request" o "New pull request"
4. Usa este título sugerido: "Adaptación inicial para Termux (es‑MX)"
5. Copia la descripción sugerida (a continuación) y crea el PR.

Descripción sugerida para el PR
---
Adaptación inicial del proyecto para ejecutarse y usarse en Termux (Android). Incluye:
- README traducido y ampliado en español (es‑MX) con instrucciones de instalación y uso en Termux.
- LICENSE (MIT) con créditos y contacto.
- CONTRIBUTING.md, CODE_OF_CONDUCT.md, SECURITY.md.
- Templates para issues y PR.
- Workflow básico de CI para lint y verificaciones.

Puntos a revisar:
- Instrucciones de instalación y comandos para Termux.
- Créditos y texto de autoría.
- Archivos añadidos: LICENSE, contributing.md, CODE_OF_CONDUCT.md, SECURITY.md y workflow CI.

---

¿Quieres que abra yo el PR (puedo darte el texto exacto para copiar) o lo abres tú desde la web? Si quieres, puedo abrir el PR por ti; dime si prefieres que lo haga y el mensaje final que quieres poner.
