# Arquitectura

Decisiones vigentes (RNF-001, RNF-002 del enunciado):
- AplicaciÃ³n web monolÃ­tica en ASP.NET MVC 5, .NET Framework 4.8, namespace Progra_03.
- Acceso a datos del dominio con Entity Framework 6 (modelo EDMX, Models/AerolineaVIPModel.edmx).
- AutenticaciÃ³n y roles con ASP.NET Identity (IdentityModels.cs, ApplicationDbContext).
- Dos bases en SQL Server: AerolineaVIP (dominio) y AerolineaVIP_Identity (usuarios y roles).
- Conexiones con autenticaciÃ³n integrada de Windows; sin credenciales en el repositorio.

Pendiente: diagrama de arquitectura y de componentes para la entrega correspondiente.