# Sprint 1 - Fundamentos y requerimientos (semanas 1-2)

Rama de trabajo: feature/sprint-1-base-identidad

## Objetivo
Dejar la base de identidad funcionando (registro, inicio y cierre de sesiÃ³n, roles), el repositorio organizado
y los requerimientos y roles preliminares documentados.

## Entregables segÃºn el enunciado
- Requerimientos aprobados -> 01_requerimientos/requerimientos_sprint1.md (aprobaciÃ³n del docente pendiente)
- Roles preliminares -> 01_requerimientos/roles_preliminares.md
- Criterios de calidad -> este documento
- Repositorio documental organizado -> carpeta docs/ y repositorio Git

## Estado de las historias

| HU | Resultado | Evidencia |
|----|-----------|-----------|
| HU-001 Registro con rol Cliente | Hecha y probada | CP-001 |
| HU-002 Inicio y cierre de sesiÃ³n | Hecha y probada | CP-002, CP-003 |
| HU-003 GestiÃ³n de roles | Hecha y probada | CP-004 y pruebas de /Roles |
| HU-027 Casos de prueba | Parcial: casos del Sprint 1 ejecutados; la matriz completa se arma al final de todos los Sprints | evidencias_sprint1.md |
| HU-028 DocumentaciÃ³n y versiones | Hecha: repositorio Git y Web.config sin credenciales; documentaciÃ³n en docs/ | commit del Sprint 1 |

## Criterios de aceptaciÃ³n del Sprint
1. Un visitante puede registrarse y queda con rol Cliente.
2. Un usuario con credenciales vÃ¡lidas inicia sesiÃ³n; con credenciales invÃ¡lidas se rechaza sin revelar informaciÃ³n sensible.
3. Cerrar sesiÃ³n retira el acceso a funciones privadas.
4. Solo el Administrador puede ver y editar roles; un cliente que intenta abrir /Roles es redirigido al inicio de sesiÃ³n.
5. El administrador no puede quitarse a sÃ­ mismo el rol Administrador.
6. El repositorio no contiene contraseÃ±as de SQL Server.

## Criterios de calidad
- AutorizaciÃ³n validada en el servidor, no solo ocultando enlaces en la interfaz (RNF-005, RNF-007).
- Formularios protegidos con ValidateAntiForgeryToken.
- Cada cambio de cÃ³digo documentado con comentarios que indican la historia y el requerimiento de origen.
- Cadenas de conexiÃ³n sin credenciales (autenticaciÃ³n integrada de Windows).
- Cada caso de prueba se considera aprobado solo si existe evidencia (captura) de su ejecuciÃ³n.

## Pendientes conocidos
- AuditorÃ­a de cambios de roles (parte del criterio de RF-044) para un Sprint posterior.
- Confirmar con el docente el alcance esperado de la entrega del Sprint 1.