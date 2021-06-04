# dotnet-mongo

Exemplo de aplicação .net core com mongodb.

Para teste:

https://localhost:5001/infectado

http://localhost:57142

```json
{
	"dataNascimento": "1990-03-01",
	"sexo": "M",
	"latitude": -23.5630994,
	"longitude": -46.6565712
}
```
OBS: é preciso ter configurar o acesso ao banco no appsettings.

Links Uteis:

USER: API T3ZgmYNOJ3RFqLQb
1234@Abcd$

Replace <password> with the password for the API user. Replace <myFirstDatabase> with the name of the database that connections will use by default. Ensure any option params are URL encoded.


mongodb://API:<94kuYrwycNpmZLXb>@cluster0-shard-00-00.vo44a.mongodb.net:27017,cluster0-shard-00-01.vo44a.mongodb.net:27017,cluster0-shard-00-02.vo44a.mongodb.net:27017/myFirstDatabase?ssl=true&replicaSet=atlas-71q7oe-shard-0&authSource=admin&retryWrites=true&w=majority


var client = new MongoClient("mongodb://API:<94kuYrwycNpmZLXb>@cluster0-shard-00-00.vo44a.mongodb.net:27017,cluster0-shard-00-01.vo44a.mongodb.net:27017,cluster0-shard-00-02.vo44a.mongodb.net:27017/MongoAPI?ssl=true&replicaSet=atlas-71q7oe-shard-0&authSource=admin&retryWrites=true&w=majority");
var database = client.GetDatabase("test");


var client = new MongoClient("mongodb://API:<94kuYrwycNpmZLXb>@cluster0-shard-00-00.vo44a.mongodb.net:27017,cluster0-shard-00-01.vo44a.mongodb.net:27017,cluster0-shard-00-02.vo44a.mongodb.net:27017/myFirstDatabase?ssl=true&replicaSet=atlas-71q7oe-shard-0&authSource=admin&retryWrites=true&w=majority");
var database = client.GetDatabase("test");

*appsettings.json criar o connection string*

- .net core - https://dotnet.microsoft.com/download

- visual code - https://code.visualstudio.com/download

- postman - https://www.postman.com/downloads/

- mongo atlas - https://www.mongodb.com/cloud/atlas/register

-----------------------------------------------

Referências:

https://docs.mongodb.com/

https://docs.mongodb.com/manual/

https://docs.mongodb.com/ecosystem/drivers/csharp/

https://docs.atlas.mongodb.com/






C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>dotnet run
It was not possible to find any compatible framework version
The framework 'Microsoft.AspNetCore.App', version '3.1.0' was not found.
  - The following frameworks were found:
      5.0.6 at [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]

You can resolve the problem by installing the specified framework and/or SDK.

The specified framework can be found at:
  - https://aka.ms/dotnet-core-applaunch?framework=Microsoft.AspNetCore.App&framework_version=3.1.0&arch=x64&rid=win10-x64

C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>dir
 O volume na unidade C é Camilla2013
 O Número de Série do Volume é 565D-3A05

 Pasta de C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api

03/06/2021  16:19    <DIR>          .
03/06/2021  16:19    <DIR>          ..
03/06/2021  01:16    <DIR>          .vscode
02/04/2020  01:54               239 Api.csproj
02/04/2020  01:54               159 appsettings.Development.json
02/04/2020  01:54               238 appsettings.json
03/06/2021  16:19    <DIR>          bin
02/04/2020  01:54    <DIR>          Controllers
02/04/2020  01:54    <DIR>          Data
02/04/2020  01:54    <DIR>          Models
03/06/2021  16:19    <DIR>          obj
03/06/2021  01:22               506 Program.cs
02/04/2020  01:54    <DIR>          Properties
03/06/2021  01:22               830 Startup.cs
               5 arquivo(s)          1.972 bytes
               9 pasta(s)      248.340.480 bytes disponíveis

C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>dotnet run
It was not possible to find any compatible framework version
The framework 'Microsoft.AspNetCore.App', version '3.1.0' was not found.
  - The following frameworks were found:
      5.0.6 at [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]

You can resolve the problem by installing the specified framework and/or SDK.

The specified framework can be found at:
  - https://aka.ms/dotnet-core-applaunch?framework=Microsoft.AspNetCore.App&framework_version=3.1.0&arch=x64&rid=win10-x64

C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>dotnet add package Microsoft.EntityFrameworkCore.Design
  Determinando os projetos a serem restaurados...
  Writing C:\Users\Compaq\AppData\Local\Temp\tmpF84C.tmp
info : Adicionando PackageReference do pacote 'Microsoft.EntityFrameworkCore.Design' ao projeto 'C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\Api.csproj'.
info :   GET https://api.nuget.org/v3/registration5-gz-semver2/microsoft.entityframeworkcore.design/index.json
info :   OK https://api.nuget.org/v3/registration5-gz-semver2/microsoft.entityframeworkcore.design/index.json 605ms
info : Restaurando pacotes para C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\Api.csproj...
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.design/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.design/index.json 574ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.design/5.0.6/microsoft.entityframeworkcore.design.5.0.6.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.design/5.0.6/microsoft.entityframeworkcore.design.5.0.6.nupkg 37ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.relational/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/humanizer.core/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.csharp/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.relational/index.json 569ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.csharp/index.json 371ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.relational/5.0.6/microsoft.entityframeworkcore.relational.5.0.6.nupkg
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.csharp/4.7.0/microsoft.csharp.4.7.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.relational/5.0.6/microsoft.entityframeworkcore.relational.5.0.6.nupkg 41ms
info :   OK https://api.nuget.org/v3-flatcontainer/humanizer.core/index.json 770ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.csharp/4.7.0/microsoft.csharp.4.7.0.nupkg 128ms
info :   GET https://api.nuget.org/v3-flatcontainer/humanizer.core/2.8.26/humanizer.core.2.8.26.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/humanizer.core/2.8.26/humanizer.core.2.8.26.nupkg 151ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.configuration.abstractions/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore/index.json 165ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore/5.0.6/microsoft.entityframeworkcore.5.0.6.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.configuration.abstractions/index.json 166ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.configuration.abstractions/5.0.0/microsoft.extensions.configuration.abstractions.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore/5.0.6/microsoft.entityframeworkcore.5.0.6.nupkg 98ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.configuration.abstractions/5.0.0/microsoft.extensions.configuration.abstractions.5.0.0.nupkg 39ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.abstractions/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.primitives/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.analyzers/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.memory/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.abstractions/index.json 170ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.primitives/index.json 161ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.analyzers/index.json 165ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.abstractions/5.0.6/microsoft.entityframeworkcore.abstractions.5.0.6.nupkg
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection/index.json 156ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.primitives/5.0.0/microsoft.extensions.primitives.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.abstractions/5.0.6/microsoft.entityframeworkcore.abstractions.5.0.6.nupkg 35ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.memory/index.json 558ms
info :   GET https://api.nuget.org/v3-flatcontainer/system.collections.immutable/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging/index.json 170ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.analyzers/5.0.6/microsoft.entityframeworkcore.analyzers.5.0.6.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.primitives/5.0.0/microsoft.extensions.primitives.5.0.0.nupkg 117ms
info :   GET https://api.nuget.org/v3-flatcontainer/system.componentmodel.annotations/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection/5.0.1/microsoft.extensions.dependencyinjection.5.0.1.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.entityframeworkcore.analyzers/5.0.6/microsoft.entityframeworkcore.analyzers.5.0.6.nupkg 35ms
info :   OK https://api.nuget.org/v3-flatcontainer/system.collections.immutable/index.json 167ms
info :   GET https://api.nuget.org/v3-flatcontainer/system.diagnostics.diagnosticsource/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.memory/5.0.0/microsoft.extensions.caching.memory.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection/5.0.1/microsoft.extensions.dependencyinjection.5.0.1.nupkg 30ms
info :   OK https://api.nuget.org/v3-flatcontainer/system.componentmodel.annotations/index.json 164ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging/5.0.0/microsoft.extensions.logging.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.memory/5.0.0/microsoft.extensions.caching.memory.5.0.0.nupkg 44ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection.abstractions/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/system.diagnostics.diagnosticsource/index.json 436ms
info :   GET https://api.nuget.org/v3-flatcontainer/system.collections.immutable/5.0.0/system.collections.immutable.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging/5.0.0/microsoft.extensions.logging.5.0.0.nupkg 35ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.abstractions/index.json
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection.abstractions/index.json 161ms
info :   GET https://api.nuget.org/v3-flatcontainer/system.componentmodel.annotations/5.0.0/system.componentmodel.annotations.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/system.collections.immutable/5.0.0/system.collections.immutable.5.0.0.nupkg 46ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging.abstractions/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/system.diagnostics.diagnosticsource/5.0.1/system.diagnostics.diagnosticsource.5.0.1.nupkg
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.options/index.json
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection.abstractions/5.0.0/microsoft.extensions.dependencyinjection.abstractions.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/system.componentmodel.annotations/5.0.0/system.componentmodel.annotations.5.0.0.nupkg 56ms
info :   OK https://api.nuget.org/v3-flatcontainer/system.diagnostics.diagnosticsource/5.0.1/system.diagnostics.diagnosticsource.5.0.1.nupkg 53ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging.abstractions/index.json 178ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.dependencyinjection.abstractions/5.0.0/microsoft.extensions.dependencyinjection.abstractions.5.0.0.nupkg 302ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.abstractions/index.json 567ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging.abstractions/5.0.0/microsoft.extensions.logging.abstractions.5.0.0.nupkg
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.abstractions/5.0.0/microsoft.extensions.caching.abstractions.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.logging.abstractions/5.0.0/microsoft.extensions.logging.abstractions.5.0.0.nupkg 59ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.caching.abstractions/5.0.0/microsoft.extensions.caching.abstractions.5.0.0.nupkg 42ms
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.options/index.json 894ms
info :   GET https://api.nuget.org/v3-flatcontainer/microsoft.extensions.options/5.0.0/microsoft.extensions.options.5.0.0.nupkg
info :   OK https://api.nuget.org/v3-flatcontainer/microsoft.extensions.options/5.0.0/microsoft.extensions.options.5.0.0.nupkg 33ms
info : Microsoft.EntityFrameworkCore.Relational 5.0.6 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo zzmO/cAcvsFeU3Ey6643GiLl4hCgGpWdcCW8LHsHP35zmfTirnjm2PrB+wf1wYQlPNyGT9+uypbVSoOopg58Mg==.
info : Microsoft.Extensions.Logging.Abstractions 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo NxP6ahFcBnnSfwNBi2KH2Oz8Xl5Sm2krjId/jRR3I7teFphwiUoUeZPwTNA21EX+5PtjqmyAvKaOeBXcJjcH/w==.
info : Microsoft.Extensions.Options 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo CBvR92TCJ5uBIdd9/HzDSrxYak+0W/3+yxrNg8Qm6Bmrkh5L+nu6m3WeazQehcZ5q1/6dDA7J5YdQjim0165zg==.
info : Microsoft.Extensions.DependencyInjection.Abstractions 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo ORj7Zh81gC69TyvmcUm9tSzytcy8AVousi+IVRAI8nLieQjOFryRusSFh7+aLk16FN9pQNqJAiMd7BTKINK0kA==.
info : Microsoft.Extensions.Caching.Abstractions 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo bu8As90/SBAouMZ6fJ+qRNo1X+KgHGrVueFhhYi+E5WqEhcnp2HoWRFnMzXQ6g4RdZbvPowFerSbKNH4Dtg5yg==.
info : Microsoft.Extensions.Logging 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo MgOwK6tPzB6YNH21wssJcw/2MKwee8b2gI7SllYfn6rvTpIrVvVS5HAjSU2vqSku1fwqRvWP0MdIi14qjd93Aw==.
info : Microsoft.Extensions.Caching.Memory 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo /1qPCleFOkJe0O+xmFqCNLFYQZTJz965sVw8CUB/BQgsApBwzAUsL2BUkDvQW+geRUVTXUS9zLa0pBjC2VJ1gA==.
info : Microsoft.Extensions.DependencyInjection 5.0.1 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo //mDNrYeiJ0eh/awFhDFJQzkRVra/njU5Y4fyK7X29g5HScrzbUkKOKlyTtygthcGFt4zNC8G5CFCjb/oizomA==.
info : System.Diagnostics.DiagnosticSource 5.0.1 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo uXQEYqav2V3zP6OwkOKtLv+qIi6z3m1hsGyKwXX7ZA7htT4shoVccGxnJ9kVRFPNAsi1ArZTq2oh7WOto6GbkQ==.
info : Microsoft.EntityFrameworkCore.Design 5.0.6 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo 2hjMovtUx3zvMMJDNjFFtYbiYRg7SNAyRe3JQzCYy7kXfADcyr7tuf9meq0lxGZBf8qvilYcDaBj5M+iq90krQ==.
info : Microsoft.EntityFrameworkCore.Abstractions 5.0.6 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo mZCwrwaiE3dSfJZZLihPueGJ2L5/vPU8VPpz21lErYIMmtZmxfSqocXe65bLlwMQ6EO/OcW7P+tvHWPsrAzMTg==.
info : Microsoft.EntityFrameworkCore.Analyzers 5.0.6 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo PhcaRr/5NgTVjm43ITSPSYQGYCUkyuBV1gEDipLnDZI+VsYwyr2HH8pHXDUaY1E6dkZoiWNRt+XNMAsK3qDIKQ==.
info : Microsoft.Extensions.Configuration.Abstractions 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo ETjSBHMp3OAZ4HxGQYpwyGsD8Sw5FegQXphi0rpoGMT74S4+I2mm7XJEswwn59XAaKOzC15oDSOWEE8SzDCd6Q==.
info : System.ComponentModel.Annotations 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo dMkqfy2el8A8/I76n2Hi1oBFEbG1SfxD2l5nhwXV3XjlnOmwxJlQbYpJH4W51odnU9sARCSAgv7S3CyAFMkpYg==.
info : Microsoft.Extensions.Primitives 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo cI/VWn9G1fghXrNDagX9nYaaB/nokkZn0HYAawGaELQrl8InSezfe9OnfPZLcJq3esXxygh3hkq2c3qoV3SDyQ==.
info : System.Collections.Immutable 5.0.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo FXkLXiK0sVVewcso0imKQoOxjoPAj42R8HtjjbSjVPAzwDfzoyoznWxgA3c38LDbN9SJux1xXoXYAhz98j7r2g==.
info : Microsoft.CSharp 4.7.0 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo pTj+D3uJWyN3My70i2Hqo+OXixq3Os2D1nJ2x92FFo6sk8fYS1m1WLNTs0Dc1uPaViH0YvEEwvzddQ7y4rhXmA==.
info : Microsoft.EntityFrameworkCore 5.0.6 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo uEqAprroH469aPCZm4iPA1oD8/YDqEQT9QjINkq4HWFA2kRh7Dm2lXX4uZ4MAzpcxoWCqKni2KbLqG8I0KnGqw==.
info : Humanizer.Core 2.8.26 instalado de https://api.nuget.org/v3/index.json com o hash de conteúdo OiKusGL20vby4uDEswj2IgkdchC1yQ6rwbIkZDVBPIR6al2b7n3pC91elBul9q33KaBgRKhbZH3+2Ur4fnWx2A==.
info : O pacote 'Microsoft.EntityFrameworkCore.Design' é compatível com todas as estruturas especificadas no projeto 'C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\Api.csproj'.
info : PackageReference do pacote 'Microsoft.EntityFrameworkCore.Design' versão '5.0.6' adicionada ao arquivo 'C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\Api.csproj'.
info : Confirmando restauração...
info : Gerando arquivo do MSBuild C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\obj\Api.csproj.nuget.g.props.
info : Gravando o arquivo de ativos no disco. Caminho: C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\obj\project.assets.json
log  : C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api\Api.csproj restaurado (em 26,23 sec).

C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>




### Erro 

*dotnet --version*

C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>dotnet --version
5.0.203


C:\Workspace\bootcamps\009_API.NET-integrada-ao-MongoDB\Api>dotnet run
It was not possible to find any compatible framework version
The framework 'Microsoft.AspNetCore.App', version '3.1.0' was not found.
  - The following frameworks were found:
      5.0.6 at [C:\Program Files\dotnet\shared\Microsoft.AspNetCore.App]


Instalar a versao antiga

https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-aspnetcore-3.1.15-windows-x64-installer


** Erro 500 **

fail: Microsoft.AspNetCore.Server.Kestrel[13]
      Connection id "0HM96SVAHB9PI", Request id "0HM96SVAHB9PI:00000001": An unhandled exception was thrown by the application.

**MONGODB.cs** Replace <password> with the password for the API user. Replace <myFirstDatabase> with the name of the database that connections will use by default. Ensure any option params are URL encoded.


 ** Unable to authenticate using sasl protocol mechanism SCRAM-SHA-1. **

reinstalei o mongodb driver
**dotnet add package MongoDB.Driver --version 2.12.3**


https://docs.microsoft.com/pt-br/aspnet/core/tutorials/first-mongo-app?view=aspnetcore-5.0&tabs=visual-studio-code


https://docs.microsoft.com/pt-br/aspnet/core/tutorials/first-mongo-app?view=aspnetcore-5.0&tabs=visual-studio-code#test-the-web-api



http://localhost:5001/api/books
