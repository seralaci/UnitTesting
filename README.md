# Unit Testing (.NET Playground)

## Code Coverage

```bash
coverlet ./bin/Debug/net7.0/Users.Api.Tests.Unit.dll --target "dotnet" --targetargs "test --no-build" --exclude "[*]Users.Api.Repositories*"'
```

```bash
dotnet test --collect:"XPlat Code Coverage"
```

```bash
reportgenerator -reports:"./TestResults/8ff703a5-41ac-44ec-b967-32ca3ce8f3f6/coverage.cobertura.xml" -targetdir:"codecoverage" -reporttypes:Html
```