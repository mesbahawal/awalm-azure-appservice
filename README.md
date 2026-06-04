# Welcome to awalM-webapp Azure App Service
- Working with WebApp type resource group using MS Azure cloud

# To Create a new web app in Azure Web App Service:
## Basics
- set web app name
- set resourse group
- subscription plan
- windwos plan
- cloud zone
- server runtime stack(.NET/Php/Java etc.)

## Deployment
- connect Github to use it as the deployment center
- choose organisation, repository and branch
- create slot to swap between staging and production version

## Networking
- private/public access
- virtual network integration

## Monitor-Secure
- application insights for expert monitoring
- enable/disable automatic app monitoring

## Tags
- for metadata

## Review and Deploy
- review above items
- check costs and subscription plan
- deploy app service

# To develop a Blazor Web App
## Absolute minimum extensions for VS Code
- C# Dev Kit
- C#
- .NET install tool

## sdks
- install .NET 10

## Get blazorserver template
- To search for the templates on NuGet.org, run:   `dotnet new search blazorserver`
- To use template run: `dotnet new install [<package>...]`.An available example package name that we used here - `Microsoft.Fast.Templates.FluentUI`, the shortname is - `fluentuiblazorserver`
- Therefore, the complete command to run: `dotnet new install Microsoft.Fast.Templates.FluentUI`

## Create a new blazorserver template
- to check if blazorserver templates are installed, run: `dotnet new list blazorserver`
- to create new blazorserver template, run: `dotnet new fluentuiblazorserver -n BlazorNetApp`. The name of the Project is going to be - *BlazorNetApp*
- since we use .NET 10, check target framework version at - `<TargetFramework>net10.0</TargetFramework>` inside the `BlazorNetApp.csproj` file
- to restore any changes done, run: `dotnet restore`

## Build and Run the app
- to build the app, run: `dotnet build`
- to publish locally the output, run: `dotnet publish -c Release -o ./publish`
- to run the BlazorNetApp run: `dotnet run`

## Pages
- Application homepage is [here](BlazorAppDemo/BlazorNetApp/Pages/Index.razor)

## Publish/Deploy code into Azure from VS Code
- we need Azure App Service extension in VS Code
- Sign in to Azure, also sign in accounts & tenants
- right-click on the App services name (in this case, awalM-webapp) and select option "Deploy to Web App.."
- browse and select BlazorNetApp, this will publish/deploy the files into Azure App service
