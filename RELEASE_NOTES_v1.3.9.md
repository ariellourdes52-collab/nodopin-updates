# 🔐 NodoPin v1.3.9 (54) — Grupos premium, copias NPBK2 y recuperación segura

**Más sencilla desde el primer inicio, más completa para conversar y preparada para conservar tus chats y tu identidad.**

NodoPin es una aplicación de mensajería privada para Android que combina **conexión por Internet** con comunicación **local mediante Bluetooth y Wi-Fi Direct** entre dispositivos compatibles. Cuando la topología y los dispositivos lo permiten, los mensajes también pueden retransmitirse por una red mesh de varios saltos. Esta versión amplía los grupos, simplifica el uso diario y evoluciona el sistema de recuperación cifrada.

## ✨ Novedades destacadas de v1.3.9

### 💾 Copias de seguridad portátiles NPBK2
- **Nuevo sistema de copia cifrada NPBK2** para conservar historial de chats, contactos, grupos y miembros, ajustes, identidad criptográfica restaurable y archivos locales compatibles cuando estén disponibles.
- **Recuperación desde una carpeta elegida** en el dispositivo o un proveedor compatible con el selector de archivos de Android, como Google Drive. La sincronización remota efectiva depende del proveedor elegido.
- **Copias automáticas programadas cada 24 horas**, sujetas a las condiciones de ejecución y batería de Android. Es posible crear copias con Wi-Fi o datos móviles; una carpeta local también puede utilizarse sin Internet.
- **Configuración de clave de recuperación desde el primer inicio**: crearla, restaurar una copia existente o elegir «Más tarde». No es obligatorio configurar una copia para empezar a utilizar NodoPin.
- En **Ajustes → Respaldo y almacenamiento** ahora se puede **crear la clave** o **cambiarla para futuras copias**, además de elegir carpeta, crear copia y restaurar.
- Mejor continuidad de la carpeta seleccionada y recuperación guiada de los permisos tras reinstalar. Android puede requerir volver a autorizar la carpeta.
- **Migración desde copias antiguas NLBAK**: el backend ya no acepta nuevas escrituras del formato antiguo, pero mantiene la lectura para recuperación histórica durante la transición. Las copias antiguas no se eliminan automáticamente.
- **Importante:** la clave de una copia antigua sigue siendo necesaria para restaurarla. Cambiar la clave actual no cambia la contraseña de los archivos anteriores. Crear una clave no crea por sí solo un respaldo.

### 🔐 Identidad, cifrado y recuperación
- Mayor continuidad de la **identidad E2EE** tras recuperar una copia, preservando las claves y huellas originales cuando coinciden y evitando la publicación prematura de identidades provisionales.
- Mejor reconciliación de conversaciones por Internet después de una restauración, sin exigir un primer contacto por Bluetooth.
- Las **advertencias auténticas de cambio de identidad** siguen presentes; no se aceptan automáticamente claves nuevas que no coincidan con las verificadas.
- Alta inicial **sin Internet y sin cuenta Google**, con PIN e identidad local. Vincular Google posteriormente busca conservar el PIN y la identidad existentes; los conflictos de titularidad deben resolverse de forma segura.
- Se mantienen el cifrado **de extremo a extremo con Double Ratchet**, las comprobaciones de identidad y las protecciones del backend.

### 👥 Grupos mucho más completos
- Pantallas y perfiles de grupo con la estética premium ya conocida de NodoPin.
- **Fotos de grupo de mayor calidad**, visualización ampliada y mejoras de sincronización; también se corrige la foto propia en la lista de integrantes.
- **Agregar participantes a grupos existentes** mediante invitaciones y actualización de membresía.
- El creador puede **retirar integrantes**; se sincronizan cambios y se restringe el acceso a los mensajes nuevos de acuerdo con las revisiones de membresía implementadas.
- Compositor de grupo mejorado con **emojis, mensajes, notas de voz y adjuntos compatibles**, además de **ubicaciones con tarjeta de mapa** y apertura en mapas externos.
- Opciones de **responder, reenviar, copiar, compartir y borrar localmente** cuando correspondan.
- **Silenciar grupos** y usar **NOD! grupal**, conservando las funciones de conversación privada.
- Separación más clara de invitaciones y mensajes internos de grupos frente a los chats individuales.
- **Limitación de seguridad:** retirar un integrante no elimina mensajes que ya había recibido ni puede revocar inmediatamente información retenida en dispositivos desconectados o aplicaciones anteriores.

### 💬 Chats, contactos y experiencia cotidiana
- Inicio y navegación más intuitivos, con instrucciones claras para **compartir el PIN, añadir un contacto e iniciar un chat** mediante PIN, QR o NFC.
- Mejor orientación en el primer inicio, explicaciones de Google opcional y mensajes comprensibles al gestionar respaldos.
- **Buscador compacto en Inicio**, mejoras en la organización de nombre/hora e **indicadores de no leídos** para conversaciones y grupos.
- Menos avisos técnicos repetitivos cuando los mensajes se entregan correctamente; los errores reales y las advertencias de seguridad no se ocultan.
- **Confirmaciones al actualizar el estado y la foto de perfil**; los mensajes distinguen éxito, cambios solo locales y fallos de publicación.
- Perfil propio y fotos de contactos con mejor calidad y decodificación optimizada de miniaturas.
- En **Mi tarjeta** y en la tarjeta compartida se unifica el texto **«Cuenta verificada por NodoPin»** cuando se muestra la verificación.
- Mejoras de enlaces, ubicación en mapas y controles habituales de chats, incluyendo silenciar y bloquear contactos.

### 🚨 SOS más rápido y completo
- **Activación de SOS con un solo botón:** acceso inmediato desde el control de emergencia, sin tener que recorrer varios menús.
- **Mensaje SOS con ubicación:** el aviso de emergencia incluye la ubicación del usuario cuando está disponible y se han otorgado los permisos necesarios.
- **Contactos favoritos para SOS:** permite organizar los contactos prioritarios de emergencia y acceder a ellos más fácilmente.
- **Atajo SOS en la barra:** acceso directo a la función de emergencia desde la barra de accesos de la aplicación.
- **Atajo SOS en Home:** botón visible desde la pantalla principal para actuar con rapidez.
- Se conservan las rutas de comunicación disponibles según la conexión y compatibilidad del dispositivo.

### 🌎 Centro DR y comunicación híbrida
- **Centro DR** integra **DR Radar** (incluidas alertas sísmicas y su sonido diferenciado) y **DR Agenda**, con acceso a eventos y funciones de calendario compatibles.
- Mensajes por **Internet**, enlaces **Bluetooth y Wi-Fi Direct**, y retransmisión **mesh multisalto** en condiciones compatibles.
- Notificaciones por canales diferenciados, alertas de mensajes y controles de privacidad disponibles en Android.
- **Nota:** la conexión offline depende del alcance físico, los permisos, la compatibilidad y las condiciones de radio; no garantiza cobertura ilimitada ni sustituye los servicios de emergencia.

### ⚡ Rendimiento y confiabilidad
- Decodificación más eficiente de las fotos mostradas como miniaturas, para reducir memoria utilizada sin modificar el original de alta resolución.
- Limpieza de caché ampliada para mosaicos de mapas, sin borrar copias NPBK2, conversaciones ni archivos privados.
- Correcciones de compatibilidad Kotlin/Compose en chats, grupos, notificaciones y restauración.
- Backend Cloudflare actualizado, con verificación saludable de servicios, límites antiabuso y política de retención de privacidad activos.
- **Se mantienen** la firma de la aplicación, el identificador Android y los protocolos existentes de mensajes y cifrado.

## 🛡️ Funciones de NodoPin que siguen disponibles
- Mensajería cifrada entre dispositivos por Internet o enlaces locales compatibles; mensajes de texto, notas de voz y multimedia según el transporte.
- PIN personal para contactos, tarjetas con QR/NFC, perfil y estado.
- Chats privados y grupales, vista previa de mapas, notificaciones, control de silencio y privacidad.
- **Private Vault opcional**, con métodos de protección y bloqueo configurables según el dispositivo.
- Mensajería SOS y Centro DR con Radar/Agenda.
- Recuperación cifrada de conversaciones y datos mediante NPBK2.

## 📦 Información del APK
| Campo | Valor |
|---|---|
| Versión | **1.3.9** |
| Código de versión | **54** |
| Paquete Android | `org.nodaviva.mesh` |
| Android mínimo | **8.0 (API 26)** |
| Android objetivo | API **37** |
| Archivo para GitHub | `nodopin.apk` |
| Tamaño | **14,846,997 bytes** (aprox. 14.16 MiB) |
| SHA-256 | `32bcf1f9ce906aa114697aca38f851cefa84e84368811937404ed7b0f9da323a` |
| Firma SHA-256 del certificado | `8E:6F:7A:BC:CB:3D:51:53:3E:C3:6C:CC:72:CB:19:E3:30:8B:79:2F:73:A2:F4:98:56:F9:6E:3D:06:C0:1B:86` |

## 📲 Cómo actualizar
1. Descarga **`nodopin.apk`** desde los archivos adjuntos de esta publicación en **GitHub Releases**.
2. Instálalo **encima de tu NodoPin actual**, sin desinstalar ni borrar datos; debe conservar el mismo certificado de firma.
3. Abre NodoPin y revisa **Ajustes → Respaldo y almacenamiento** para definir tu clave y carpeta de copia cifrada.
4. Conserva tu clave en un lugar seguro y comprueba que existe una copia NPBK2 recuperable; si elegiste Drive, comprueba también que se haya sincronizado.

**Recomendación:** realiza una copia cifrada antes de actualizar. Si pierdes tanto la clave como las copias, NodoPin no puede reconstruir su contenido cifrado.

**Alcance de la validación:** el APK fue inspeccionado (versión, paquete, firma y cadenas nuevas). Se han realizado pruebas funcionales del usuario en restauración E2EE, grupos y comunicación offline, y se confirmó HTTP 200 del backend. Estas comprobaciones no constituyen una auditoría de seguridad independiente ni pruebas universales en todos los modelos Android.

---

❤️ **NodoPin — Comunicación privada cuando más importa.** 🔐📡