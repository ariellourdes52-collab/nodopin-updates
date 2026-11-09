# 🚀 NodoPin v1.5.2 (68) — Notificaciones FCM/FID recuperadas

**Actualización de estabilidad y privacidad de las notificaciones de NodoPin Android.**

## 🔔 Notificaciones restauradas y registro FID

- 📲 **Migración al identificador de instalación Firebase (FID):** integración Android con el registro actual de Firebase Cloud Messaging para vincular de forma individual la instalación con los avisos push.
- 🔄 **Revalidación al iniciar y regresar a NodoPin:** sincronización del registro FID existente con el servidor, sin borrar ni recrear innecesariamente la identidad de instalación.
- 🛡️ **Registro protegido:** prueba de posesión FCM antes de activar la asociación de una instalación con su cuenta/PIN, manteniendo las comprobaciones de autenticación y App Check.
- 🧩 **Corrección del fallo HTTP 500:** se corrigió en Cloudflare la incompatibilidad del registro temporal de desafíos FID con el índice único existente en D1, sin migrar ni alterar el esquema de la base.
- ✅ **Recepción FCM recuperada:** tras activar la corrección del Worker, se confirmó de nuevo la llegada de notificaciones en Android.

## 🔐 Privacidad y continuidad

- 🧹 **Diagnóstico temporal retirado:** la versión distribuida elimina los registros de depuración `NodoPin-FID` utilizados durante la investigación.
- 🔒 **Seguridad existente conservada:** continúan las protecciones P1/P2, App Check, cifrado y controles del backend sin cambios ajenos al flujo FID.
- ☁️ **Datos existentes preservados:** la actualización no exige borrar los datos de la aplicación ni sustituir copias de seguridad.

## 📦 Datos del APK

- **Versión:** 1.5.2
- **Código de versión:** 68
- **Paquete:** `org.nodaviva.mesh`
- **Archivo:** `nodopin.apk`
- **Firma:** certificado de publicación coincidente con v1.5.1
- **SHA-256:** `8ca8997bbb5201e3eaea75b13ee03cfff75aa8ffef222d235d6fc7b8ba5a4240`

**Descarga:** https://github.com/ariellourdes52-collab/nodopin-updates/releases/download/v1.5.2/nodopin.apk
