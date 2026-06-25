FinaPro - Ecosistema de Compilación Móvil para Android

Este repositorio contiene la arquitectura necesaria para empaquetar de manera híbrida la plataforma de gestión FinaPro de Moda Evelyn Bolivia y generar de forma automática un instalador .apk compatible con Android 10+.

Estructura del Repositorio en GitHub

Para que la compilación en la nube (GitHub Actions) funcione correctamente y sin errores, debes subir tus archivos con la siguiente distribución exacta:

MiRepositorio/
├── .github/
│   └── workflows/
│       └── android-build.yml       <-- Archivo de compilación automática
├── www/
│   └── index.html                  <-- Tu index.html interactivo y lógico
├── package.json                    <-- Dependencias de npm y Capacitor
├── capacitor.config.json           <-- Configuración nativa del App Móvil
└── README.md                       <-- Esta guía explicativa


Instrucciones para Carga de Archivos

Crea un repositorio en GitHub (ej. finapro-android).

Crea una carpeta llamada www en tu computadora e introduce tu archivo index.html allí dentro.

Coloca los archivos package.json, capacitor.config.json y el archivo de GitHub Actions .github/workflows/android-build.yml en sus respectivas rutas.

Sube todos los cambios mediante Git:

git init
git add .
git commit -m "Estructura inicial de FinaPro con compilación nativa"
git branch -M main
git remote add origin TU_URL_DE_GITHUB
git push -u origin main


Descarga del APK compilado

Una vez subidos los archivos, dirígete a la pestaña Actions en tu repositorio de GitHub. Verás que se inicia un proceso de construcción automatizado de forma inmediata. Al cabo de un par de minutos, podrás descargar el artefacto comprimido que contiene tu archivo FinaPro-ModaEvelyn-Debug-APK listo para ser instalado en tu teléfono o el de tus socios.
