# Asp-Net-Api

## Asp.Net commands

  **Command:**
> dotnet new ``ProjectName`` -o DirectoryName --no-https -f net7.0

1. dotnet </br>
  R: Command for work with .Net
2. dotnet **new ProjectName** </br>
  R: Create a new project in .Net
3. dotnet new ``ProjectName`` **-o DirectoryName** </br>
  R: Create a new directory for the project
4. dotnet new ``ProjectName`` -o DirectoryName **--no-https** </br>
  R: Alert to don't enable HTTPS
5. dotnet new ``ProjectName`` -o DirectoryName --no-https **-f net7.0** </br>
  R: The -f <version> indicates that you're creating a project with a specific version

## Which file were created?
 1. Program.cs : Contains the app startup code and middleware configuration.
 2. Pages : Contains some example web pages for the application.
 3. MyWebApp.csproj : Defines some project settings, such as, .NET SDK version to target.
 4. Properties/launchSettings.json : Defines different profile settings for the local development environment. A port number ranging between 5000-5300 is automatically assigned at project creation and saved on this file.
