# 🛡️ NodoPin v1.4.9 (65) — Seguridad App Check

NodoPin Android incorpora **Firebase App Check** a las comunicaciones con el Worker oficial, reforzando la identificación de la aplicación frente a solicitudes no autorizadas. Esta versión conserva la mensajería privada y el actualizador premium.

## 🚀 Novedades

- 🛡️ **Integración con Firebase App Check:** soporte para obtener tokens de integridad de la aplicación en Android, con Play Integrity para la edición de distribución.
- 🔐 **Protección del canal oficial:** se incorpora el encabezado `X-Firebase-AppCheck` en las peticiones al Worker de NodoPin cuando hay un token disponible.
- ⚡ **Obtención asíncrona del token:** la aplicación evita detener la mensajería mientras solicita la credencial de App Check.
- 🔄 **Compatibilidad Android ↔ Web:** se mantiene la mensajería cifrada NLDR1 entre dispositivos con PINes diferentes, la sincronización, notas de voz y multimedia.
- ✨ **Actualizador premium conservado:** siguen disponibles el aviso mejorado, los temas claro/oscuro, la descarga protegida y la comprobación SHA-256 antes de instalar.
- 🗂️ **Copias y privacidad:** se conserva el acceso a Copia Integral NPINTEGRAL2, Google Drive y la identidad criptográfica existente.

## 🔒 Alcance y compatibilidad

La aplicación **envía tokens App Check cuando están disponibles**; la exigencia del token (`enforce`) depende de la configuración del servidor Cloudflare y se despliega por separado. Las versiones Android anteriores que no admiten este encabezado podrían recibir HTTP 401 en rutas protegidas si el servidor exige App Check. También puede producirse un primer intento sin token mientras se obtiene de forma asíncrona. No se activa la función V4 de PIN compartido.

## 📦 APK oficial v1.4.9

| Campo | Valor |
| --- | --- |
| Versión | `1.4.9` |
| versionCode | `65` |
| Paquete Android | `org.nodaviva.mesh` |
| Archivo para GitHub Assets | `nodopin.apk` |
| Tamaño | `14,896,185 bytes` |
| SHA-256 del APK | `15d6dc691fe511fce013277bb8d9d86dac2f5c8b5a8bf4ca9fa0283e1cf25a5f` |
| SHA-256 del certificado de firma | `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86` |
| Android mínimo | Android 8.0 (API 26) |

**Verificaciones del archivo aportado:** ZIP íntegro, manifiesto `1.4.9 (65)`, presencia de firma APK v2 y certificado de firma idéntico al de las ediciones oficiales anteriores. Estas comprobaciones no sustituyen las pruebas funcionales completas en dispositivos reales.

**Publicación segura:** adjuntar en esta release un único archivo llamado exactamente `nodopin.apk`. El actualizador solo debe anunciar v1.4.9 después de comprobar que el APK publicado coincide con el SHA-256 indicado.

## 📲 Cómo actualizar

1. Descarga `nodopin.apk` desde **Assets** de esta versión.
2. Instálalo **encima de NodoPin**, sin desinstalar ni borrar tus datos.
3. Conserva tu copia cifrada y tu clave de recuperación.
4. Comprueba mensajes, notas de voz y sincronización después de instalar.

🌐 **Sitio oficial:** https://nodopin.web.app/

**NodoPin — Tu PIN. Tu identidad. Tu conexión.**
