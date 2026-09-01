# hack-mx-style-termux

Repositorio adaptado para Termux (Android) en español (es-MX).

Este proyecto está basado en: https://github.com/Ades-Azael-hat/Hack-mx-style

Objetivo
- Crear una versión adaptada y propia para uso en Termux (Android).
- Documentación y guías en español (es‑MX).
- Scripts y recomendaciones para facilitar instalación y uso en Termux.

Advertencia
- Esta adaptación busca ser educativa y de uso legítimo. No fomentes actividades ilegales o no éticas.

Requisitos (en Termux)
- Termux actualizado.
- Conexión a internet.

Instalación rápida en Termux
1. Actualiza paquetes base:

   pkg update && pkg upgrade -y

2. Instala herramientas necesarias (ejemplos comunes):

   pkg install git python nodejs wget curl unzip -y

3. Opcional: configura almacenamiento (si requieres acceso a la tarjeta/archivos):

   termux-setup-storage

4. Clona este repositorio:

   git clone https://github.com/Ades-Azael-hat/hack-mx-style-termux.git
   cd hack-mx-style-termux

5. Si el proyecto usa Python (ejemplo):

   pip3 install --user -r requirements.txt

   o, para aislar:
   python3 -m venv .venv
   source .venv/bin/activate
   pip install -r requirements.txt

6. Para proyectos Node.js:

   npm install

Uso básico
- Revisa el README y los scripts dentro del repo. Muchos scripts en esta adaptación están pensados para ejecutarse desde Termux con:

  sh nombre_del_script.sh

Notas para Termux
- Algunas dependencias pueden necesitar compilación; instala build-essential si es necesario:

  pkg install build-essential -y

- Si un script requiere permisos de almacenamiento, asegúrate de ejecutar termux-setup-storage y dar acceso.
- Si usas termux:api (acceso a sensores, cámara, etc.) instala el paquete:

  pkg install termux-api -y

Estructura inicial
- README.md (este archivo traducido y adaptado)
- contributing.md (guía para contribuir)
- LICENSE (MIT)
- .github/ (templates y workflows)

Contribuir
- Lee CONTRIBUTING.md para saber cómo contribuir.
- Por defecto hay una rama de trabajo: termux/adaptacion — abre un PR desde tu fork o rama.

Créditos
- Autores originales: BOCHMEN3 y chukys
- Adaptación: AZAEL ARREDONDO (alias Ad3x)
- Contacto: bochmen3@gmail.com

Nota de adaptación
"Con cariño y éxito para mí gran hat azael" — Ad3x

Licencia
- Este proyecto se publica bajo la licencia MIT (ver LICENSE).
