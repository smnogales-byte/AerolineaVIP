# Evidencias de pruebas - Sprint 1

Los casos CP-001 a CP-004 provienen de la matriz de casos de prueba del enunciado (apartado 13.7).
La matriz completa y ejecutada se arma al finalizar todos los Sprints; aquÃ­ se registran los casos ejecutados en el Sprint 1.

Las capturas se guardan en la carpeta evidencias/ de este mismo directorio con el nombre indicado.

| Caso | RF | DescripciÃ³n | Resultado obtenido | Estado | Captura |
|------|----|-------------|--------------------|--------|---------|
| CP-001 | RF-001 | Registro vÃ¡lido | Usuario "prueba1" se registrÃ³, entrÃ³ a sesiÃ³n y aparece con rol Cliente en /Roles | Aprobado | evidencias/CP-001_registro.png |
| CP-002 | RF-002 | Inicio de sesiÃ³n vÃ¡lido | administrador@aerolineavip.com entra y ve el menÃº Roles | Aprobado | evidencias/CP-002_login_valido.png |
| CP-003 | RF-002, RF-005 | Credenciales incorrectas | Permanece en Login con "Intento de inicio de sesiÃ³n no vÃ¡lido." | Aprobado | evidencias/CP-003_login_invalido.png |
| CP-004 | RF-005 | Acceso indebido con sesiÃ³n de cliente | cliente@aerolineavip.com abre /Roles y es redirigido a /Account/Login?ReturnUrl=%2FRoles | Aprobado | evidencias/CP-004_acceso_indebido.png |

## Pruebas adicionales (no son casos CP del enunciado)

| Prueba | Resultado | Captura |
|--------|-----------|---------|
| Cierre de sesiÃ³n | Vuelven "Registrarse" e "Iniciar sesiÃ³n" en el menÃº, sin saludo | evidencias/extra_logout.png |
| Listado de usuarios y roles en /Roles como administrador | Muestra todos los usuarios con sus roles | evidencias/extra_roles_listado.png |
| Editar roles de un usuario | Un usuario sin roles pasÃ³ a Administrador | evidencias/extra_roles_editar.png |
| Administrador intenta quitarse su propio rol | Mensaje "No puedes quitarte a ti mismo el rol Administrador." y el rol se mantiene | evidencias/extra_bloqueo_autoquitar.png |