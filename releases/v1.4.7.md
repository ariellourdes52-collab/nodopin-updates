# 🚀 NodoPin v1.4.7 (63) — Copia Integral desde el inicio

NodoPin para Android da un paso más hacia la gestión de copias cifradas. Esta versión **1.4.7**, posterior a la 1.4.6, concentra el cambio en la **configuración inicial**, sin rediseñar ni alterar las demás funciones de la aplicación.

## 🆕 Novedad principal

- 🗂️ **Copia Integral en la configuración inicial:** se sustituye el acceso secundario «Copia antigua» por **«Copia Integral»** y se abre el panel existente de Copia Integral **NPINTEGRAL2**.
- 🔐 **Identidad cifrada protegida:** el nuevo acceso no reemplaza las claves criptográficas de una identidad existente. Para recuperar historial en otra instalación es necesario conservar o recuperar primero la identidad original correspondiente al PIN.
- 🛡️ **Cambios quirúrgicos:** se conservan la recuperación heredada cuando resulta necesaria para la identidad, Google Drive, las sesiones NLDR1, los chats, los grupos y las demás funciones existentes.

## 🪪 Tarjeta de cuenta verificada

NodoPin Android dispone de consulta de estado de verificación al compartir una tarjeta nueva. Si una cuenta obtiene después una insignia oficial y un cargo como «Negocio Verificado», la **siguiente tarjeta PNG compartida** puede reflejar la insignia y el título confirmados por el servidor. **Esta función ya existía y se revisó en el código; no es una modificación nueva de v1.4.7.** Los PNG compartidos previamente no se actualizan por sí solos. La consulta depende de que el servidor responda correctamente.

## ✨ Funciones que se mantienen de v1.4.6

- 📌 Hasta **5 chats fijados** en la parte superior.
- 📱 Invitaciones QR más rápidas entre dispositivos Android.
- 💬 Sincronización de mensajes optimizada entre Android y Web, con **PINes diferentes**.
- 🎙️ Notas de voz, archivos y funciones existentes de mensajería cifrada.
- 🆘 SOS, grupos, QR/NFC, conexiones locales compatibles y Centro DR.

## ⚠️ Alcance de la Copia Integral

El acceso a NPINTEGRAL2 **no significa que la restauración integral Android ↔ Web, con todos los archivos e identidad, esté certificada en dispositivos reales**. Tampoco activa el PIN compartido multidispositivo V4 ni convierte por sí solo archivos antiguos NPBK2 a NPINTEGRAL2. Antes de reinstalar, conserva una copia cifrada y sus frases de recuperación.

## 📦 Identificación del APK verificado

| Campo | Valor |
| --- | --- |
| Versión | `1.4.7` |
| versionCode | `63` |
| Identificador | `org.nodaviva.mesh` |
| Archivo a adjuntar | `nodopin.apk` |
| Tamaño | `14,896,185 bytes` |
| SHA-256 del APK | `43cf1f846ba37e6a159bd05a1f75ba2526ce02ce71ec44305683c5046406979f` |
| SHA-256 del certificado | `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86` |
| Android mínimo | Android 8.0 (API 26) |

**Comprobaciones:** manifiesto 1.4.7 (63), integridad del ZIP y presencia de bloque de firma APK. La huella del certificado coincide con la edición 1.4.6 publicada en este repositorio. Esto no sustituye las pruebas funcionales completas en dispositivos Android reales.

## ⬇️ Actualización

1. En **Assets**, descarga el archivo `nodopin.apk`.
2. Conserva tu copia de seguridad cifrada y las frases de recuperación.
3. Instala esta versión **encima de NodoPin**, sin desinstalar ni borrar los datos.
4. Comprueba la opción de Copia Integral en la configuración inicial cuando corresponda y verifica que tus chats y respaldos siguen funcionando.

🌐 **Web oficial:** https://nodopin.web.app/

**NodoPin — Tu PIN. Tu identidad. Tu conexión.**
