# Base de datos

Script: Script_BD_AerolineaVIP.sql (crea las dos bases).

## AerolineaVIP (dominio)
30 tablas, 5 vistas, 5 triggers y el procedimiento usp_GenerarVuelos.
Conectada al proyecto mediante Models/AerolineaVIPModel.edmx (cadena AerolineaVIPEntities).

## AerolineaVIP_Identity (identidad)
Tablas estÃ¡ndar de ASP.NET Identity (AspNetUsers, AspNetRoles, AspNetUserRoles, entre otras), creadas por el script.
Conectada mediante la cadena DefaultConnection (ApplicationDbContext).
En IdentityModels.cs se desactiva el inicializador de EF (Database.SetInitializer<ApplicationDbContext>(null))
porque las tablas las crea el script, no Entity Framework.

## Cadenas de conexiÃ³n (Web.config)
Ambas usan autenticaciÃ³n integrada de Windows (Integrated Security=True). No se guardan usuarios ni contraseÃ±as de SQL Server.

## Sprint 1
Solo se usa la base de identidad (registro, login, roles). La base de dominio se usa desde el Sprint 2 (vuelos y flota).