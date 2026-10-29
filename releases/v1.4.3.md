# 📬 NodoPin v1.4.3 (59) — Mensajes y confirmaciones más fiables en segundo plano

Actualización de fiabilidad centrada en la entrega de mensajes con NodoPin en segundo plano, especialmente en dispositivos con restricciones de batería.

## Novedades
- **Recepción online con Google y sin Google:** el registro del dispositivo para avisos FCM y la sincronización del buzón utilizan la autenticación disponible sin exigir que el PIN esté vinculado a Google. El servidor sigue validando la pertenencia de la sesión al PIN.
- **FCM y sincronización:** mejor recuperación de mensajes pendientes cuando Android permite ejecutar los trabajos en segundo plano. El respaldo periódico está sujeto a Doze y a las políticas del fabricante.
- **Hotfix de entrega D:** se conservan los reintentos de acuses de entrega cifrados; no se considera completado el trabajo cuando la confirmación sigue pendiente.
- **Sin cambios visuales:** no se añaden menús, controles de diagnóstico ni pantallas.
- **Sin cambios en el cifrado existente:** Double Ratchet, preclaves, multimedia, Bluetooth BLE y Wi‑Fi Direct continúan con su implementación anterior.

## Compatibilidad
- Nombre de versión: **1.4.3**
- Código de versión: **59**
- Paquete: `org.nodaviva.mesh`
- Archivo oficial: **nodopin.apk**
- Tamaño: **14,896,153 bytes**
- SHA-256 del archivo: `35f046c2a87ce9ddc81a1fcafe683a7d45de4aae6459ca8d87b7e91735545a5a`
- SHA-256 del certificado de firma: `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86`

## Validaciones y límites
El APK entregado se inspeccionó: archivo ZIP íntegro, manifiesto Android con versión 1.4.3 (59) y certificado incluido coincidente con la APK de 1.4.2. La coincidencia del certificado **no sustituye** una validación completa de la firma criptográfica de Android.

La recepción y el indicador D requieren que el teléfono receptor ejecute la sincronización y confirme el mensaje realmente almacenado. Las políticas de ahorro de energía del fabricante pueden retrasar los trabajos incluso con FCM operativo.

La actualización del Worker Cloudflare para sesiones locales se despliega **por separado** de este APK. El usuario reportó un despliegue correcto; esta release no modifica el backend.

## Instalación
1. Descarga `nodopin.apk` desde los archivos adjuntos de esta publicación.
2. Conserva una copia cifrada NPBK2.
3. Instala sobre la versión anterior **sin desinstalar ni borrar los datos**.
4. Prueba notificaciones, entrega D y lectura R con la aplicación en segundo plano, además de SOS y enlaces locales.

Web oficial: https://nodopin.web.app/
