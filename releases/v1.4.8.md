# ✨ NodoPin v1.4.8 (64) — Actualizador Premium

Esta actualización de NodoPin Android mejora la experiencia al recibir una nueva versión. **Se concentra en la pantalla de actualización y en la persistencia del aviso**, sin cambiar el sistema de mensajería, los respaldos ni el cifrado.

## 🚀 Novedades

- 🔔 **Avisos de actualización más estables:** el aviso ya no debe desaparecer al cambiar temporalmente el estado del inicio de la aplicación, los permisos o las pantallas de recuperación.
- 🛡️ **Sin perder actualizaciones por fallos de red:** si ya se detectó una versión nueva, un fallo temporal de conexión no oculta automáticamente el aviso.
- ⏳ **«Ahora no» funciona como aplazamiento temporal:** se puede posponer la instalación sin silenciar indefinidamente la nueva versión.
- ✨ **Diseño premium:** presentación renovada con el logotipo oficial de NodoPin, encabezado de actualización oficial, versión destacada y tarjeta de novedades.
- 🌗 **Compatible con temas claro y oscuro:** colores integrados con la apariencia de NodoPin.
- 📱 **Mejor adaptación a pantallas pequeñas:** contenido desplazable sin perder los controles.
- 📥 **Progreso conservado:** la descarga iniciada sigue disponible al regresar a la aplicación, cuando Android DownloadManager mantiene el archivo.
- 🔐 **Instalación protegida:** se conservan la validación del SHA-256, la comprobación de la firma del APK y la confirmación de Android antes de instalar.

## 🧩 Cambios técnicos limitados

- `NodaApp.kt`: el actualizador permanece montado mientras otras pantallas reciben prioridad.
- `NodoPinStartupUpdates.kt`: se ajusta el ciclo de vida del aviso y se presenta el nuevo diseño.
- `app/build.gradle` o `app/build.gradle.kts`: `versionName = 1.4.8` y `versionCode = 64`.
- **Sin cambios** en `NodoPinUpdater.kt`, la verificación criptográfica, Google Drive, NPINTEGRAL2, NLDR1, chats, grupos, SOS ni el backend.

## 🪪 Funciones que permanecen

- 📌 Hasta 5 chats fijados.
- 💬 Mensajería E2EE por Internet entre Android y Web, con PINes diferentes.
- 📷 Tarjetas de contacto, QR/NFC, perfiles verificados y sus cargos cuando el servidor confirma el estado.
- 🗂️ Acceso a Copia Integral NPINTEGRAL2 desde la configuración inicial, incorporado en v1.4.7.
- 🎙️ Notas de voz, multimedia, grupos y Centro DR.

## 📦 Identificación prevista del APK

| Campo | Valor |
| --- | --- |
| Versión | `1.4.8` |
| versionCode | `64` |
| Paquete Android | `org.nodaviva.mesh` |
| Archivo oficial | `nodopin.apk` |
| Android mínimo | Android 8.0 (API 26) |
| Firma | La misma firma del APK oficial v1.4.7 |

**Importante:** las mejoras se prepararon a partir de código fuente. Su funcionamiento en dispositivos reales debe comprobarse tras compilar y firmar la APK. El flujo de GitHub comprueba el paquete, la versión y el certificado antes de activar el manifiesto de actualizaciones.

## ⬇️ Cómo actualizar

1. Descarga `nodopin.apk` desde **Assets** de esta versión.
2. Conserva tus respaldos y las frases de recuperación.
3. Instala sobre la versión existente **sin desinstalar la aplicación ni borrar los datos**.
4. Comprueba la pantalla de actualización en el próximo lanzamiento que tenga una versión posterior disponible.

🌐 **Web oficial:** https://nodopin.web.app/

**NodoPin — Tu PIN. Tu identidad. Tu conexión.**
