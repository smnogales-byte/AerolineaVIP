# Requerimientos del Sprint 1

Fuente: ENUNCIADO_PROYECTO (apartados de requerimientos funcionales y no funcionales).
Sprint 1 "Fundamentos y requerimientos" (semanas 1-2). Historias: HU-001, HU-002, HU-003, HU-027, HU-028.

## Requerimientos funcionales que cubre el Sprint 1

| ID | Requerimiento | Criterio de aceptaciÃ³n | Historia |
|----|---------------|------------------------|----------|
| RF-001 | El sistema permitirÃ¡ registrar cuentas de cliente. | Una cuenta solo se crea cuando los datos obligatorios son vÃ¡lidos y se cumplen las reglas de unicidad aprobadas. | HU-001 |
| RF-002 | El sistema permitirÃ¡ iniciar sesiÃ³n. | Un usuario con credenciales vÃ¡lidas accede segÃºn sus permisos; uno no autenticado no accede a las funciones protegidas. | HU-002 |
| RF-003 | El sistema permitirÃ¡ cerrar sesiÃ³n. | La sesiÃ³n deja de autorizar el acceso a funciones privadas. | HU-002 |
| RF-005 | El sistema administrarÃ¡ roles y permisos. | Cada operaciÃ³n protegida se autoriza de acuerdo con el rol y los permisos efectivos. | HU-003 |
| RF-044 | El sistema permitirÃ¡ gestionar usuarios y roles autorizados. | Las modificaciones de privilegios quedan restringidas y registradas. | HU-003 |

Nota sobre RF-044: en el Sprint 1 las modificaciones de privilegios quedan restringidas al rol Administrador. El registro (auditorÃ­a) de esos cambios no estÃ¡ implementado todavÃ­a.

## Requerimientos no funcionales relevantes

| ID | CategorÃ­a | Requerimiento | CÃ³mo se cumple en el Sprint 1 |
|----|-----------|---------------|-------------------------------|
| RNF-005 | Seguridad | Las funciones protegidas requerirÃ¡n autenticaciÃ³n y autorizaciÃ³n. | Atributo [Authorize] en RolesController; prueba CP-004. |
| RNF-006 | Confidencialidad | Los datos personales solo serÃ¡n visibles para usuarios autorizados. | /Roles solo es accesible al rol Administrador. |
| RNF-007 | ValidaciÃ³n | Las reglas crÃ­ticas se comprobarÃ¡n en el servidor. | La regla "el administrador no puede quitarse su propio rol" se valida en el servidor (RolesController). |
| RNF-020 | Versionamiento | Los cambios estarÃ¡n sujetos a control de versiones. | Repositorio Git, rama feature/sprint-1-base-identidad (HU-028). |

## Historias de usuario del Sprint 1

| HU | Historia | Prioridad | Puntos |
|----|----------|-----------|--------|
| HU-001 | Como cliente, quiero registrarme para gestionar mis operaciones. | P1 | 3 |
| HU-002 | Como usuario, quiero iniciar y cerrar sesiÃ³n de forma segura. | P1 | 3 |
| HU-003 | Como administrador, quiero gestionar los roles para controlar el acceso. | P1 | 5 |
| HU-027 | Como responsable de QA, quiero verificar los requisitos mediante casos de prueba. | P1 | 5 |
| HU-028 | Como responsable tÃ©cnico, quiero documentar y controlar las versiones del proyecto. | P1 | 3 |

Estado de aprobaciÃ³n de los requerimientos: pendiente de confirmaciÃ³n del docente.