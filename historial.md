# historial
## create a soluction project base.
  Id CommandLine                                                                                                                    
  -- -----------                                                                                                                    
   1. `dotnet new sln --name EccommerceSolucion`
   2. `md src`
   3. `dotnet new classlib -o src/core/Ecommerce.Domain`
   5. `dotnet new classlib -o src/core/Ecommerce.Application`
   6. `dotnet new classlib -o src/Infrastructure --name Ecommerce.Infrastructure`
   7. `dotnet new webapi -o src/Api --name Ecommerce.Api`
   9. `dotnet sln add .\src\Infrastructure\Ecommerce.Infrastructure.csproj`
  10. `dotnet sln add .\src\core\Ecommerce.Domain\Ecommerce.Domain.csproj`
  11. `dotnet sln add .\src\core\Ecommerce.Application\Ecommerce.Application.csproj`
  12. `dotnet sln add .\src\Api\Ecommerce.Api.csproj`
  13. `dotnet add .\src\Infrastructure\Ecommerce.Infrastructure.csproj reference .\src\core\Ecommerce.Application\Ecommerce.Applica...`
  14. `dotnet add .\src\Api\Ecommerce.Api.csproj refence .\src\core\Ecommerce.Application\Ecommerce.Application.csproj`
  15. `dotnet add .\src\Api\Ecommerce.Api.csproj reference .\src\core\Ecommerce.Application\Ecommerce.Application.csproj`
  16. `dotnet add .\src\Api\Ecommerce.Api.csproj reference .\src\Infrastructure\Ecommerce.Infrastructure.csproj`


