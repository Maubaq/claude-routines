# claude-routines

`registro_notiflyer.csv` es el registro acumulativo de la rutina de correo.
Cada ejecución lee el archivo, agrega al final las filas nuevas (sin duplicar
links ya registrados) y hace commit en la rama `claude/awesome-cerf-3jis0z`.

Columnas: fecha_ejecucion, fecha_recepcion, categoria, remitente_nombre,
remitente_email, asunto, accion_sugerida, razon_urgencia, link
