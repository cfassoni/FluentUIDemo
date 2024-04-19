# Fluent UI in Blazor ASP.NET

This project intends to demonstrated capabilities of Blazor Web Application using Microsoft Fluent UI components.
As it uses the DotNet CLI in (in case of windows, the Powershell terminal), it's not tied to Visual Studio so you can use any IDE to edit files.

## Getting Started

The easiest way to get started is by using our template.

```powershell

dotnet new install Microsoft.FluentUI.AspNetCore.Templates

```

## Create a Demo project

The commands below in PowerShell will create a solution folder  followed by Blazor Fluent UI project. The folders names were intentionally declared diferently to show they are independent.

```
mkdir FluentUIDemo

cd .\FluentUIDemo\

dotnet new sln -n FluentUIDemo

dotnet new fluentblazor -n BlazorFluentUI

dotnet sln add .\BlazorFluentUI\
```

__Optional:__ Add 'gitignore' to Project:

```
dotnet new gitignore
```

## Running with Hot Reloading

```
cd .\BlazorFluentUI\

dotnet build

dotnet watch
```

__optional:__ before running, in case you want to test the application using HTTPS, edit the properties file *'launchSettings.json'* located in *Properties* folder and move the https declaration before the http. Alternatively you can run the https informing the launch profile using option -lp (or --launch-profile):

```
dotnet watch -lp https
```
Use 'CTRL-C' to gracefully exit the server.

## References

1. https://www.fluentui-blazor.net/
2. https://github.com/microsoft/fluentui-blazor
3. https://dotnet.microsoft.com/en-us/apps/aspnet/web-apps/blazor
4. https://learn.microsoft.com/en-us/aspnet/core/
