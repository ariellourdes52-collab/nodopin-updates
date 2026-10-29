# 🚨 NodoPIN v1.4.0 (56) — SOS inteligente, ubicación precisa y alertas bajo control

**Más claridad cuando importa: alertas que se detienen al abrir la app, localización SOS con mapa y una experiencia de emergencia más intuitiva.**

NodoPIN es una aplicación de mensajería privada para Android que combina Internet y conexiones locales por Bluetooth y Wi-Fi Direct entre dispositivos compatibles, con retransmisión mesh multisalto cuando los enlaces lo permiten. El contacto se comparte mediante PIN, QR o NFC sin necesidad de entregar el número telefónico.

## 🚨 Alertas SOS y sísmicas que dejan de sonar al atenderlas
- Al abrir o reanudar NodoPIN, acceder desde la notificación o entrar al chat correspondiente, la aplicación detiene el reproductor dedicado de alarma SOS y sísmica y su vibración.
- El aviso continúa disponible en la aplicación; detener el sonido **no borra la emergencia ni confirma que se haya resuelto**.
- Se evita que una tarea de alarma anterior vuelva a iniciar el sonido después de abrir la app.
- Se mantienen los sonidos y canales de notificación propios, sin alterar NOD! ni el transporte de mensajes.

## 📍 NodoPIN SOS: mapa, detalles y GPS más útil
- La tarjeta de emergencia incorpora un **mapa dentro del mensaje**, detalles separados y botón **«Abrir ubicación»**.
- Cuando Android suministra los datos, muestra coordenadas y **precisión estimada (± metros)**, para distinguir un punto aproximado de uno más confiable.
- El envío intenta obtener una ubicación nueva de **alta precisión** usando los servicios de localización disponibles, comparando posiciones recientes (máximo aproximado de 45 segundos) y limitando la espera a unos 10 segundos.
- Si no hay señal, permisos o coordenadas confiables, el SOS **se envía igualmente**, sin inventar ubicación ni presentar una lectura antigua como actual.
- El mapa y la información se organizan sin texto superpuesto ni datos ocultos.

## ⚡ SOS sencillo, incluso desde la barra de Android
- Guía breve dentro de la aplicación sobre qué hace SOS, cómo elegir favoritos y confirmar el envío.
- Instrucciones para colocar **NodoPIN SOS** en los Ajustes rápidos de Android; en versiones compatibles aparece el diálogo del sistema para añadirlo, con alternativa manual.
- El mosaico ofrece acceso rápido a la preparación del SOS: **tocarlo por sí solo no envía la emergencia**.
- Los contactos de emergencia y favoritos continúan disponibles.

## 👤 Notificaciones con identidad visual consistente
- La foto de contacto utilizada en notificaciones se procesa como **miniatura circular con esquinas transparentes**, sin modificar la imagen original del perfil.
- El aspecto final puede variar porque Android y el fabricante controlan parte de la presentación de notificaciones.

## 🔐 Compatibilidad, privacidad y funciones conservadas
- Los textos visibles emplean la marca **«NodoPIN SOS»**. El marcador técnico heredado **«NexLink SOS»** se conserva internamente para reconocer las alertas entre versiones anteriores y nuevas.
- No cambia la firma oficial, el paquete Android ni los protocolos existentes de cifrado de extremo a extremo Double Ratchet.
- Permanecen las conversaciones individuales y grupales, NPBK2, Private Vault, QR/NFC, Centro DR con DR Radar y DR Agenda, NOD!, SOS y los enlaces por Internet, BLE y Wi-Fi Direct.
- El funcionamiento de GPS y alertas depende del dispositivo, los permisos, Android y las condiciones de conexión. SOS es una función de apoyo, **no sustituye los servicios oficiales de emergencia**.

## 📦 Información de esta APK

| Campo | Valor |
|---|---|
| Versión | **1.4.0** |
| Código | **56** |
| Paquete | `org.nodaviva.mesh` |
| Android mínimo | **8.0 (API 26)** |
| Android objetivo | **API 37** |
| Archivo para GitHub | `nodopin.apk` |
| Tamaño | **14,863,385 bytes (14.18 MiB)** |
| SHA-256 | `1dc173a2f1ef0f5e8c0fbc860262eec412e5744bc3be80ee91acf83534d95548` |
| Certificado SHA-256 | `8E:6F:7A:BC:CB:3D:51:53:3E:C3:6C:CC:72:CB:19:E3:30:8B:79:2F:73:A2:F4:98:56:F9:6E:3D:06:C0:1B:86` |

## 📲 Actualización segura

1. Descarga `nodopin.apk` desde los archivos de esta versión en GitHub Releases.
2. Haz primero una copia NPBK2 y conserva la clave de recuperación.
3. Instala sobre la versión anterior **sin desinstalar y sin borrar los datos**.
4. Permite ubicación precisa cuando desees incluir un punto de alta precisión en el SOS.
5. Añade «NodoPIN SOS» a la barra desde las indicaciones de la app si tu Android lo permite.

**Alcance de la verificación:** se inspeccionó la APK suministrada, su manifiesto Android (1.4.0/56), la integridad ZIP, el SHA-256 y la firma v2; el certificado coincide con la versión anterior. Estas comprobaciones **no equivalen a pruebas funcionales en los teléfonos A/B/C** de GPS, tonos y navegación. Antes de distribución general se recomiendan pruebas SOS extremo a extremo y de regresión.

🌐 **Sitio oficial:** https://nodopin.web.app/

**NodoPIN — Tu PIN. Tu identidad. Tu conexión.**
