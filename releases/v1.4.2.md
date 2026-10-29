# 🔐 NodoPIN v1.4.2 (58) — Privacidad y sesiones cifradas sin depender de Google

Esta versión reúne mejoras de privacidad y el trabajo de establecimiento inicial de sesiones cifradas por Internet y conexiones locales. La disponibilidad de cada función depende de permisos, dispositivos y tipo de enlace.

## ✨ Novedades
- **Política de privacidad dentro de Android:** pantalla nativa con explicaciones del tratamiento de datos, seguridad, proveedores, ubicación y derechos del usuario. La información legal no garantiza por sí sola el cumplimiento normativo.
- **Inicio de mensajería online sin Google obligatorio:** actualización del flujo de preclaves y envío cifrado para identidades con o sin vinculación de Google.
- **Intercambio inicial de claves offline:** cambios en el establecimiento de sesiones Double Ratchet mediante Wi-Fi Direct y BLE. Se conserva la verificación de identidad; se recomienda comprobar el primer contacto en teléfonos reales.
- **Bluetooth / Wi-Fi Direct:** se mantiene el alcance de transportes compatibles. Las fotos y notas de voz offline se apoyan en Wi-Fi Direct; no se anuncia transferencia general de multimedia exclusivamente mediante BLE.
- **Pulido de interfaz:** corrección del uso obsoleto de `OpenInNew` en las pantallas de privacidad.

## 📱 Datos del APK
| Campo | Valor |
|---|---|
| Versión | **1.4.2** |
| versionCode | **58** |
| Paquete | `org.nodaviva.mesh` |
| Archivo | `nodopin.apk` |
| Tamaño | **14,896,153 bytes** |
| SHA-256 | `6bb3a268d3e2ea48cfcaa9660e2d9ded3e2bf7bc4d75a3ab20d87909778061ef` |
| Certificado de firma (SHA-256) | `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86` |

**Comprobado:** el APK proporcionado tiene manifiesto 1.4.2 (58), ZIP íntegro y certificado de firma coincidente con el publicado en v1.4.1. **Pendiente:** validación completa en dos teléfonos, especialmente primer contacto cifrado sin Internet, relé multisalto, recuperación de backup y notificaciones. No se afirma que estas pruebas físicas hayan sido realizadas.

## ⬇️ Instalación
1. Descarga `nodopin.apk` desde los archivos de esta versión.
2. Guarda una copia de seguridad cifrada NPBK2 antes de actualizar.
3. Instala encima de la versión existente, sin desinstalar ni borrar datos.
4. Comprueba Ajustes → Privacidad y seguridad, conversaciones, SOS y enlaces locales.

**Página oficial:** https://nodopin.web.app/

**NodoPIN — Tu PIN. Tu identidad. Tu conexión.**
