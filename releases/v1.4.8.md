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

## 📦 Identificación del APK v1.4.8 verificado

| Campo | Valor |
| --- | --- |
| Versión | `1.4.8` |
| versionCode | `64` |
| Paquete Android | `org.nodaviva.mesh` |
| Archivo oficial en GitHub | `nodopin.apk` |
| Tamaño exacto | `14,896,185 bytes` |
| SHA-256 del APK | `76e2a06bb2dde7e33ffadd74c4ea433b986e17c3c6f0d5c0a6a9f85d8ec5e394` |
| SHA-256 del certificado de firma | `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86` |
| Android mínimo | Android 8.0 (API 26) |

**Verificación técnica del archivo entregado:** estructura ZIP íntegra, manifiesto Android 1.4.8 (64), firma APK v2 presente y certificado coincidente con la edición oficial v1.4.7. También se observaron cambios en el código DEX respecto a v1.4.7. Estas comprobaciones no sustituyen pruebas funcionales completas ni una auditoría criptográfica de todos los contenidos en dispositivos reales.

**Publicación segura:** el archivo adjunto a la release debe llamarse exactamente `nodopin.apk` y su SHA-256 debe coincidir con el indicado. La actualización del manifiesto del actualizador se habilita solamente tras verificarlo.

## ⬇️ Cómo actualizar

1. Descarga `nodopin.apk` desde **Assets** de esta versión.
2. Conserva tus respaldos y las frases de recuperación.
3. Instala sobre la versión existente **sin desinstalar la aplicación ni borrar los datos**.
4. Comprueba la pantalla de actualización en el próximo lanzamiento que tenga una versión posterior disponible.

🌐 **Web oficial:** https://nodopin.web.app/

**NodoPin — Tu PIN. Tu identidad. Tu conexión.**
