# 🔐 NodoPin v1.3.10 (55) — Cierre de grupos para todos y limpieza del servidor

**Más control sobre tus grupos, manteniendo la mensajería privada por Internet, Bluetooth y Wi-Fi Direct.**

## ✨ Novedad principal: eliminar un grupo para todos

- El **creador** puede utilizar **«Eliminar grupo para todos»** para cerrar definitivamente un grupo.
- La aplicación envía órdenes de cierre autenticadas y **cifradas de extremo a extremo** a los participantes por los transportes compatibles.
- Los teléfonos actualizados que reciben una orden válida del creador salen automáticamente y limpian los datos locales del grupo que pueden identificar sin afectar otras conversaciones.
- Si un integrante está desconectado, la orden permanece en la cola cifrada del emisor y se reintenta cuando vuelve a estar disponible la conexión correspondiente. **No se garantiza una eliminación instantánea en dispositivos desconectados.**
- El servidor registra el cierre e impide reutilizar el identificador del mismo grupo.

## 🗂️ Multimedia y almacenamiento

- Nuevo índice de adjuntos de grupo en Cloudflare D1 para los archivos enviados y registrados **desde esta actualización**.
- Al cerrar un grupo registrado, se depuran en D1 las fotos y notas de voz cifradas asociadas explícitamente a él.
- Los videos del grupo asociados a Backblaze B2 dejan de estar accesibles por el endpoint y quedan pendientes de la limpieza existente.
- Se preservan los archivos de chats privados y los demás grupos.
- Los adjuntos anteriores al despliegue, los objetos sin índice de grupo, las capturas, las copias NPBK2 antiguas y la multimedia exportada a galerías o carpetas externas **no pueden eliminarse retroactivamente de todos los dispositivos**.
- El borrado definitivo de versiones históricas en buckets B2 versionados depende de sus políticas de retención; no se promete destrucción física inmediata.
- Los mensajes E2EE opacos enviados mediante el relay existente siguen las reglas de retención del servidor; no se realiza borrado selectivo de mensajes históricos por grupo.

## 🛡️ Seguridad y compatibilidad

- Solo el creador autenticado puede cerrar un grupo mediante el nuevo endpoint del backend.
- Las órdenes de cierre verifican autoría y revisión del grupo; no se desactiva la verificación de identidad E2EE.
- Cloudflare D1 añade las tablas `nodopin_group_registry` y `nodopin_group_media`.
- Se mantienen el identificador Android, la firma oficial, Double Ratchet, las conversaciones privadas, NPBK2, SOS, Centro DR, Bluetooth, Wi-Fi Direct y retransmisión mesh compatible.

## 📦 Datos de esta compilación

| Campo | Valor |
|---|---|
| Versión | **1.3.10** |
| versionCode | **55** |
| Paquete Android | `org.nodaviva.mesh` |
| Android mínimo | **8.0 / API 26** |
| Android objetivo | **API 37** |
| Archivo oficial | `nodopin.apk` |
| Tamaño | **14,863,381 bytes** (aprox. 14.18 MiB) |
| SHA-256 | `0dc79ad62f14e1a587ebbd4db2cf40295ca0d6e6bac07651055334befcabe4c6` |
| Certificado SHA-256 | `8E:6F:7A:BC:CB:3D:51:53:3E:C3:6C:CC:72:CB:19:E3:30:8B:79:2F:73:A2:F4:98:56:F9:6E:3D:06:C0:1B:86` |

## 📲 Cómo instalar

1. Descarga **`nodopin.apk`** desde los archivos adjuntos de esta versión de GitHub.
2. Instálalo **encima de NodoPin 1.3.9**, sin desinstalar ni borrar los datos. Conserva la misma firma.
3. Antes de actualizar, comprueba tu copia cifrada NPBK2 y conserva la clave de recuperación.
4. Para las nuevas funciones grupales, **todos los miembros** deben actualizar a una versión compatible.

**Verificación:** se comprobó el manifiesto Android, el SHA-256, la integridad ZIP, la firma frente a la versión 1.3.9 y la presencia del endpoint de grupos en el APK. El usuario confirmó que pasaron las pruebas del backend, el Worker fue desplegado y su health check devolvió HTTP 200; D1 confirmó las tablas nuevas. **Quedan pendientes las pruebas funcionales de cierre y limpieza con los teléfonos A/B/C.**

---

❤️ **NodoPin — Comunicación privada cuando más importa.** 🔐📡
