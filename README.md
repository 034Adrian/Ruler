# Ruler
 AdministradorWeb
 * usando **asp.NET core 7.0**
 [dependencias](README.md#dependencias)

# Dependencias
 * `dotnet tool install dotnet-aspnet-codegenerator --version 6.0.2 --global` **ok**
 * `dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design --version 6.0.2`
 * `dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore --version 6.0.3`
 * `dotnet add package Microsoft.AspNetCore.Identity.UI --version 6.0.3`
 * `dotnet add package Microsoft.EntityFrameworkCore.Design --version 6.0.3`
 * `dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version 6.0.3`

  * `dotnet tool install dotnet-ef --version 6.0.3 --global`

 * `dotnet ef migrations add CreateIdentitySchema`
 * `dotnet ef database update`

 # Procedimiento
  * `cd RazorPagesFolder`
  * [instalar](README.md#dependencias)
  * `dotnet aspnet-codegenerator identity --useDefaultUI --dbContext RazorPagesRulerAuth`