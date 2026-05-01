**🚀 .NET CLI Quick Reference**

**📁 Setup & Info**

  dotnet new gitignore
  ➡️ Adds a .gitignore file

  dotnet -h
  ➡️ Shows all available .NET CLI commands
  
  dotnet new --list
  ➡️ Lists all project templates (Console, WPF, WCF, etc.)

**🧱 Solution & Project Creation**

  dotnet new sln
  ➡️ Creates a solution file
  
  dotnet new console -o DemoApp
  ➡️ Creates a console app named DemoApp
  
  dotnet new classlib -o DemoLib
  ➡️ Creates a class library named DemoLib
  
  dotnet sln add DemoApp
  ➡️ Adds DemoApp to the solution

**🔗 References & Packages**

  dotnet add DemoApp reference ./DemoLib/DemoLib.csproj
  ➡️ Adds reference of DemoLib to DemoApp
  
  dotnet add DemoApp package Dapper
  ➡️ Adds Dapper NuGet package
  ⚠️ Always add packages to a specific project, not the solution

**📦 Dependency Management**

  dotnet restore
  ➡️ Restores all packages

**🛠️ Build & Run**

  dotnet build
  ➡️ Builds the solution
  
  dotnet clean
  ➡️ Cleans temporary files
  
  dotnet run
  ➡️ Runs the application

📦 **Publish (Single Executable)**

  dotnet publish -p:PublishSingleFile=true -r win-x64 --self-contained true
  🔍 Explanation:
  PublishSingleFile=true
  ➡️ Bundles everything into one executable
  -r win-x64
  ➡️ Targets Windows 64-bit runtime
  --self-contained true
  ➡️ Includes the .NET runtime (runs on any machine)
