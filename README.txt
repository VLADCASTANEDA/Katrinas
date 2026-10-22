CRONO MTB — PROYECTO ANDROID (FUENTE)
=====================================

Este paquete contiene un proyecto Android Studio que envuelve el prototipo
Crono MTB v5 en una app Android local basada en WebView.

Incluye:
- HTML guardado dentro de la app (no necesita internet para abrirlo).
- JavaScript y almacenamiento local del WebView habilitados.
- Selector de archivos para importar participantes desde CSV.
- Exportaciones encaminadas a Descargas/CronoMTB en Android moderno.
- Identificador de aplicación: mx.laguna.cronomtb

CÓMO GENERAR EL APK
-------------------
1. En una computadora, instala Android Studio estable.
2. Descomprime CronoMTB_Android.zip.
3. Android Studio > Open > selecciona la carpeta CronoMTB_Android.
4. Acepta la sincronización de Gradle e instala Android SDK Platform 35
   cuando Android Studio lo solicite.
5. Menú Build > Build Bundle(s) / APK(s) > Build APK(s).
6. Android Studio mostrará un enlace para localizar el APK de depuración.
   Normalmente queda en app/build/outputs/apk/debug/app-debug.apk.
7. Copia ese APK al Android, ábrelo y autoriza la instalación desde esa
   fuente si el sistema lo solicita.

IMPORTANTE
----------
- Este ZIP es el proyecto fuente; no es un APK ya compilado.
- En este entorno no hay Android SDK/Gradle instalados para compilar y
  verificar un APK aquí.
- Antes de usarlo en una carrera real, prueba importación CSV, exportación,
  respaldo JSON, corrección/auditoría, bloqueo de pantalla y recuperación
  tras cerrar/reabrir la app.
- El cronómetro se basa en el comportamiento del prototipo HTML y aún no
  debe considerarse equipo de cronometraje certificado.
- Conserva copias externas de los respaldos. Desinstalar la app o borrar
  sus datos puede borrar el almacenamiento local.


ALTERNATIVA SIN COMPILAR EN EL TELÉFONO: GITHUB ACTIONS
1. Abre https://github.com desde el navegador del teléfono e inicia sesión.
2. Crea un repositorio llamado CronoMTB-Android.
3. Sube los archivos y carpetas de este proyecto, incluida .github/workflows.
4. Abre Actions, elige "Build Crono MTB APK" y pulsa "Run workflow".
5. Al terminar, descarga el artefacto "CronoMTB-debug-APK" y extrae app-debug.apk.
Se requiere internet y cuenta de GitHub. Subir carpetas desde móvil puede ser
laborioso; si te atoras, dime qué pantalla ves. No publiques datos personales.
