# Sección para reemplazar "REGISTRO EN GOOGLE DRIVE" en el prompt de la rutina

# REGISTRO EN GITHUB

Al finalizar el informe, agrega los correos clasificados al archivo acumulativo
`registro_notiflyer.csv` del repositorio `maubaq/claude-routines`, rama
`claude/awesome-cerf-3jis0z`. NO uses Google Drive.

**Columnas (mismo orden):**
fecha_ejecucion, fecha_recepcion, categoria, remitente_nombre, remitente_email, asunto, accion_sugerida, razon_urgencia, link

**Reglas:**
- Lee el archivo actual (ya existe con headers), agrega las filas nuevas al final y haz commit/push a esa rama. No crees archivos nuevos.
- No dupliques: omite correos cuyo `link` ya esté en el archivo.
- Solo categorías 🔴 🟡 🟢 (`urgente`, `importante`, `informativo`); los ⚪ no se registran.
- Fechas en formato `YYYY-MM-DD HH:MM`; `razon_urgencia` solo para `urgente`.
- Entrecomilla con "..." los campos que tengan comas.
- `link`: https://mail.google.com/mail/u/0/#search/rfc822msgid:MESSAGE_ID con el ID real.
- Si el push falla, repórtalo en el informe y notifica.
