# Roles preliminares del sistema

Fuente: matriz de roles (apartado 16.1 del enunciado) y apartados 9.2 y 9.8.
ImplementaciÃ³n: Global.asax.cs (CrearRoles) con ASP.NET Identity, base AerolineaVIP_Identity.

| Rol | Origen | DÃ³nde se solicita en el enunciado | ObservaciÃ³n |
|-----|--------|-----------------------------------|-------------|
| Cliente | ExplÃ­cito | 4.1, 9.2 (INT-02), 9.8, 16.1, RF-001, HU-001, CP-004 | Se asigna automÃ¡ticamente al registrarse (HU-001). |
| Pasajero | ExplÃ­cito | 9.2 (INT-03), 9.8, RF-035/036, HU-016 | Permisos se detallan en sprints posteriores. |
| Counter | ExplÃ­cito | 9.2 (INT-04), 9.8 (empleado de counter), RF-038/039, HU-018, CP-023 | Funciones pendientes de la decisiÃ³n DP-13. |
| Administrador | Propuesta | 9.2 (INT-05), 9.8, RF-005, RF-044, HU-003, CP-024 | Ãšnico rol que gestiona roles (/Roles). |
| Operaciones | Propuesta | 9.2 (INT-06), 9.8 (responsable de operaciones), RF-041/047, HU-007/024 | Permisos se detallan en sprints posteriores. |
| Comercial | Propuesta | 9.2 (INT-07), 9.8 (responsable comercial), DP-04 a DP-08 | Depende de decisiones pendientes. |

## Usuarios de prueba (solo desarrollo)

Se crean al iniciar la aplicaciÃ³n (Global.asax.cs): un usuario por rol mÃ¡s un superadministrador con rol Administrador.
Las contraseÃ±as de prueba estÃ¡n en Global.asax.cs y deben cambiarse o retirarse antes de cualquier uso fuera del entorno acadÃ©mico.

## Reglas del Sprint 1

- Un registro nuevo recibe el rol Cliente (HU-001).
- Solo el rol Administrador accede a /Roles (RF-005, RF-044, RNP-09 mÃ­nimo privilegio).
- El administrador no puede quitarse a sÃ­ mismo el rol Administrador.