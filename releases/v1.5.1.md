# 🚀 NodoPin v1.5.1 (67) — Grupos, multimedia y seguridad reforzada

**Más control en las conversaciones grupales, imágenes de mejor calidad y una comunicación privada protegida.** Esta publicación reúne el trabajo de Android realizado después de **v1.4.9** y conserva las mejoras de recuperación incorporadas en **v1.5.0**.

## 👥 Grupos y conversaciones

- 🔐 **Invitaciones y administración cifradas:** mejoras en el intercambio de invitaciones, el ingreso y la salida de integrantes y el seguimiento del estado de membresía. El protocolo de grupos conserva la identidad y el cifrado de las conversaciones.
- 🖼️ **Foto de grupo HD:** mejoras en selección, codificación, sincronización y presentación de avatares grupales. Se corrigió un caso de deduplicación que impedía mostrar correctamente una foto recibida; la foto grupal HD fue comprobada en Android.
- 💬 **Mensajes y estados grupales:** mejoras de compatibilidad para mensajes grupales, visualización de contenido y confirmaciones **S (enviado), D (entregado) y R (leído)**. La aparición de D/R depende de las confirmaciones reales de los destinatarios.
- 📷 **Multimedia de grupos:** soporte del flujo de fotos, notas de voz y videos cifrados, con estructuras y metadatos propios de grupo (NPG1/NPG2). La disponibilidad de cada envío depende del tipo de archivo, los dispositivos y la conexión.
- 🔔 **NOD! en grupos:** se conserva la recepción y reproducción de avisos NOD! compatibles. No se anuncia como validado el envío completo de NOD! entre todos los equipos.

## 🛡️ Protección del contenido y de los participantes

- 🔗 **Multimedia vinculada a su mensaje:** integración Android de los identificadores de archivo **mediaId** usados para comprobar la asociación de adjuntos con su mensaje en el backend (P2). Se verificó el registro de multimedia Android → Web.
- 👥 **Autorizaciones de grupos (P1):** componentes de compatibilidad con las constancias y pruebas de pertenencia para multimedia de grupo, sujetos a las reglas activas del servidor. La aplicación no cambia por sí sola la configuración de Cloudflare.
- 🔐 **App Check conservado:** se mantiene la integración de integridad de la aplicación incluida desde v1.4.9, junto con el cifrado E2EE de los chats.

## 🔑 Recuperación de cuenta y continuidad

- ☁️ **Recuperación Google mejorada (incorporada en v1.5.0):** reautenticación únicamente cuando una operación sensible de recuperación la exige, con comprobaciones de cuenta y PIN y reintento controlado. **No requiere iniciar sesión periódicamente cada 15 minutos.**
- 🗂️ **Copias cifradas preservadas:** se mantienen Google Drive, el acceso a **Copia Integral NPINTEGRAL2** y los mecanismos locales de adjuntos cifrados. La restauración integral de todos los adjuntos grupales entre Android y Web sigue requiriendo validación de extremo a extremo.
- 🔄 **Mensajería entre Android y Web:** se conservan mensajes privados, notas de voz, sincronización por Internet e identidades con **PIN diferentes**. No se activa la modalidad V4 de PIN compartido.

## ✨ Funciones que se mantienen

- 📌 Hasta **5 conversaciones fijadas**.
- 📱 Intercambio de contactos mediante **QR y NFC**, con invitaciones Android optimizadas.
- 🪪 Tarjetas de perfil, insignias y cargos verificados cuando el servidor confirma ese estado.
- 🆘 **SOS**, ubicaciones, conexiones locales BLE/Wi-Fi Direct y **Centro DR**.
- 📲 Actualizador premium con comprobación SHA-256 y protección contra instalación de un APK distinto del anunciado.

## 📦 Identificación del APK oficial

| Campo | Valor |
| --- | --- |
| Versión | **1.5.1** |
| versionCode | **67** |
| Paquete Android | `org.nodaviva.mesh` |
| Android mínimo | **8.0 (API 26)** |
| Archivo que se debe adjuntar | **`nodopin.apk`** |
| Tamaño exacto | **14,928,953 bytes** |
| SHA-256 del APK | `61db01286d4a3918a8bbd0f9dc34d717a1c39671721f9804887ea26829fb7b53` |
| SHA-256 del certificado | `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86` |

**Comprobaciones realizadas:** integridad ZIP correcta, manifiesto `1.5.1 (67)`, paquete Android esperado y certificado de firma coincidente con la edición oficial v1.5.0. El APK contiene el bloque de firma Android v2. Esta inspección no sustituye una prueba funcional completa de todos los casos de grupo, multimedia y restauración en teléfonos reales.

## ⬇️ Instalación y actualización

1. Descarga el único archivo **`nodopin.apk`** en los archivos adjuntos (**Assets**) de esta publicación.
2. Instala sobre NodoPin existente **sin desinstalar ni borrar sus datos**, usando la misma firma oficial.
3. Conserva una copia cifrada y la clave de recuperación antes de actualizar.
4. Comprueba mensajes privados y grupales, multimedia y sincronización.

**Publicación segura:** el actualizador oficial solo debe anunciar `v1.5.1` después de que el APK esté adjunto, la publicación sea pública y su SHA-256 coincida exactamente con el valor indicado.

🌐 Web oficial: https://nodopin.web.app/

**NodoPin — Tu PIN. Tu identidad. Tu conexión.**
