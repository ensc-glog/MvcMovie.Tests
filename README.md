# MvcMovie.Tests

.NET console app demonstrating integration testing for ASP.NET Core MVC.

Adapted from the [official documentation](https://docs.microsoft.com/en-us/aspnet/core/test/integration-tests?view=aspnetcore-5.0).

## Development notes

### Installing dependencies

```bash
dotnet add package Microsoft.AspNetCore.Mvc.Testing -v 5.0.12
```

### Creating a reference to the tested project

This command must be run in the (common) parent folder of SUT ("System Under Test") and tests projects.

```bash
dotnet add ./MvcMovie.Tests/MvcMovie.Tests.csproj reference ./MvcMovie/MvcMovie.csproj
```

### Running the tests

```bash
dotnet test
```
