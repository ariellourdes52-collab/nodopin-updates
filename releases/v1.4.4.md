# 🚨 NodoPin v1.4.4 (60) — SOS por SMS directo y experiencia premium

Nueva vía de emergencia para solicitar ayuda **sin Internet y sin conexión local útil**, siempre que el teléfono disponga de una SIM y servicio de SMS. Esta edición es la **variante GitHub**.

## Novedades
- **SOS celular directo, sin Twilio ni servicios intermediarios:** como último recurso, NodoPin permite enviar el aviso desde la SIM del usuario a los números opcionales de sus Favoritos SOS.
- **Activación restringida:** el respaldo SMS solo se ofrece cuando no hay Internet funcional ni enlace BLE/mesh o Wi-Fi Direct utilizable. Exige confirmación expresa antes de enviar.
- **Mensaje de auxilio breve:** «SOS NODOPIN: NECESITO AYUDA», con enlace de Google Maps que incluye las coordenadas GPS disponibles. Si no se obtiene ubicación, se debe poder pedir ayuda igualmente.
- **Favoritos SOS mejorados:** configuración voluntaria de un teléfono de emergencia y presentación más clara y elegante en modo claro y oscuro.
- **Interfaz SOS pulida:** mejores tarjetas informativas, indicadores y controles de edición de números.
- **Actualizador GitHub conservado:** esta APK mantiene la comprobación interna de nuevas versiones. La variante Store se compila por separado, sin respaldo SMS ni actualizador.
- **Sin cambios intencionales en los motores de mensajería y cifrado:** chats, Double Ratchet, grupos, BLE, Wi-Fi Direct y Centro DR conservan su funcionamiento.

## Importante sobre el SOS por SMS
- **Necesita señal celular y servicio SMS activo**; puede generar cargos de la operadora por destinatario y por segmento.
- **No es un mensaje prioritario garantizado** por la red móvil ni puede forzar alarmas en el teléfono receptor.
- **Los SMS no tienen el cifrado de extremo a extremo de los chats NodoPin**: su contenido puede ser procesado por las operadoras.
- El enlace del mapa usa la última ubicación disponible; obtener GPS y abrir el mapa dependen del equipo y de las condiciones del lugar.
- No reemplaza llamar a los servicios de emergencia. La confirmación del envío no garantiza recepción o lectura.

## Identificación de esta APK
- **Versión:** 1.4.4
- **versionCode:** 60
- **Paquete:** `org.nodaviva.mesh`
- **Archivo que debes adjuntar:** `nodopin.apk`
- **Tamaño exacto:** 14,896,185 bytes
- **SHA-256 del APK:** `b84d1f95412ada09d7a6587834767229dae96f036972b5b505d84100bbfc0537`
- **Certificado de firma SHA-256:** `8e6f7abccb3d51533ec36ccc72cb19e3308b792f73a2f49856f96e3d06c01b86`

## Verificaciones y alcance
Se comprobó que la APK suministrada tiene manifiesto Android 1.4.4 (60), paquete correcto, los permisos `SEND_SMS` y `REQUEST_INSTALL_PACKAGES`, estructura ZIP íntegra y certificado de firma coincidente con la release previa. Esta inspección **no equivale a una auditoría completa de seguridad ni a una prueba integral de la firma APK**. El desarrollador probó en un teléfono real el envío SOS con ubicación precisa; faltan pruebas exhaustivas en otras operadoras y configuraciones de conectividad.

## Actualización
1. Descarga **`nodopin.apk`** del apartado *Assets* de esta release.
2. Conserva una copia de seguridad cifrada NPBK2 antes de actualizar.
3. Instala sobre la versión existente **sin desinstalar ni borrar datos**.
4. Comprueba que los contactos SOS tengan números correctos; prueba chats, confirmaciones D/R, recepción de notificaciones y enlaces locales.

**Web oficial:** https://nodopin.web.app/

**NodoPin — Tu PIN. Tu identidad. Tu conexión.**
