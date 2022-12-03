# Asp-Net-Api

Sources (https://dotnet.microsoft.com/en-us/learn/aspnet/hello-world-tutorial/create)

## Asp.Net commands

  **Command:**
> dotnet new webapp -o DirectoryName --no-https -f net7.0

1. dotnet </br>
  R: Command for work with .Net
2. dotnet **new webapp** </br>
  R: Create a new web project in .Net (Replace webapi for any other type of project that you want)
3. dotnet new webapp **-o DirectoryName** </br>
  R: Create a new directory for the project
4. dotnet new webapp -o DirectoryName **--no-https** </br>
  R: Alert to don't enable HTTPS
5. dotnet new webapp -o DirectoryName --no-https **-f net7.0** </br>
  R: The -f <version> indicates that you're creating a project with a specific version

## Which file were created?
 1. Program.cs : Contains the app startup code and middleware configuration.
 2. Pages : Contains some example web pages for the application.
 3. MyWebApp.csproj : Defines some project settings, such as, .NET SDK version to target.
 4. Properties/launchSettings.json : Defines different profile settings for the local development environment. A port number ranging between 5000-5300 is automatically assigned at project creation and saved on this file.



## **What's a controller?**
Controller is bridge between model and views, and can the most important side in an API, because it save all the requests and set the endpoints

Example: WeatherForecastController, all requests about weatherforecast go inside this controller

### Controller can be created as class, if you're doing a webapp, you need call the Controller 
ExampleController : Controller </br>
But, you're building a webapi, you call ControllerBase
ExampleControllerApi : ControllerBase

### **Webapi controller sintax:**
``Class UserController``
### Enable resources that help to build an API
>[ApiController]
### It will handle your route, at example below the route will remove the "controller", so, UserController will turn in just User at route
> Route("[controller]");
### class calling the ControllerBase
>public class UserController : ControllerBase {
### route for the action
>[HttpGet("ReturnUsers")]
### the above line will return the below function at User/ReturnUsers
>public IAction ReturnUsers(){
>}
### 
