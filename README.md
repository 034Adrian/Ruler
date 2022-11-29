# Ruler
 AdministradorWeb
 * usando **asp.NET core 7.0**
 [dependencias](README.md#dependencias)

# Dependencias
 * `dotnet tool install dotnet-aspnet-codegenerator --version 6.0.2 --global` **ok**
 * `dotnet add package Microsoft.VisualStudio.Web.CodeGeneration.Design --version 6.0.2` **ok**
 * `dotnet add package Microsoft.AspNetCore.Identity.EntityFrameworkCore --version 6.0.3` **ok**
 * `dotnet add package Microsoft.AspNetCore.Identity.UI --version 6.0.3` **ok**
 * `dotnet add package Microsoft.EntityFrameworkCore.Design --version 6.0.3` **ok**
 * `dotnet add package Microsoft.EntityFrameworkCore.SqlServer --version 6.0.3` **ok**

 * `dotnet tool install dotnet-ef --version 6.0.3 --global` **ok**

# Procedimiento
 * `cd RazorPagesFolder`

 * [instalar](README.md#dependencias)

 * `dotnet aspnet-codegenerator identity --useDefaultUI --dbContext RazorPagesRulerAuth`

 * `dotnet ef migrations add CreateIdentitySchema`
 * `dotnet ef database update`

 * agregar `<partial name="_LoginPartial" />` en Pages/Shared/__Layout.cshtml

 creacion y personalizacion de la interfas de registro de usuario
 * `dotnet aspnet-codegenerator identity --dbContext RazorPagesRulerAuth --files "Account.Manage.EnableAuthenticator;Account.Manage.Index;Account.Register;Account.ConfirmEmail" --userClass RazorPagesRulerUser --force`

 el siguiente comando desde la raíz del proyecto para ver los valores válidos de la opción --files:
 * `dotnet aspnet-codegenerator identity --listFiles`

 