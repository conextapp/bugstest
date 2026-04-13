📱 Conext App - Automated Bug Testing
Este repositorio contiene la suite de pruebas automatizadas End-to-End (E2E) para la aplicación móvil ConextApp, desarrolladas durante mis prácticas de DAM. El objetivo principal es la detección, documentación y replicación de errores de interfaz y flujo de usuario.

🛠️ Tecnologías utilizadas
Maestro Studio: Framework principal para la automatización de flujos de UI.

Android Studio: Entorno para la ejecución de emuladores y depuración.

YAML: Lenguaje utilizado para la definición de los flujos de prueba.

Plane.so: Plataforma utilizada para el reporte y seguimiento de los bugs detectados.

🏗️ Arquitectura del Proyecto (POM)
El proyecto sigue el patrón Page Object Model (POM) para garantizar que los tests sean mantenibles y escalables.

/common: Contiene flujos reutilizables (como login.yaml). Esto evita la duplicación de código y permite que, si la interfaz de acceso cambia, solo sea necesario actualizar un único archivo.

Raíz (/): Aquí se encuentran los archivos de prueba específicos para cada bug detectado (ej: Bug_Modo_Oscuro.yaml).

🚀 Cómo ejecutar los tests
Requisitos previos
Tener instalado Maestro CLI.

Tener un emulador de Android activo en Android Studio.

Ejecución de un test individual
Para ejecutar una prueba y ver el resultado en tiempo real:

Bash
maestro test Bug_Zona_Segura.yaml
Generación de evidencias (Video)
Para generar una grabación local del flujo (útil para adjuntar en Plane.so):

Bash
maestro record --local Bug_LinkedIn.yaml Bug_LinkedIn.mp4
📋 Bugs Documentados
Actualmente, el repositorio incluye automatizaciones para:

❌ Fallo en Correo de Recuperación.

❌ Enlace roto en sección LinkedIn.

❌ Error visual en Modo Oscuro.

❌ Fallo de vinculación con YouTube.

❌ Problemas de renderizado en Zona Segura.

❌ Flujo de Inicio de Sesión con Google.
