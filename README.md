dotnet new gitignore                  										                    // adds gitignore file
dotnet -h                             										                    // shows us all dotnet commands 
dotnet new --list                     										                    // shows list of projects we can create.(Console, WPF, WCF)
dotnet new sln                        										                    // creates solution file
dotnet new console -o DemoApp         										                    // creates console app with name DemoApp
dotnet sln add DemoApp                                                        // adds DemoApp to solution file
dotnet new classlib -o DemoLib                                                // creates class lib with name DemoLib
dotnet add package Dapper                                                     // adds Dapper nuget package in project file 
                                                                                 (always add package in specific project not in solution)
dotnet add reference . ./DemoLib/DemoLib. csproj                              // adds reference of DemoLib to DemoApp
dotnet restore                                                                // restores packages
dotnet build                                                                  // builds solution
dotnet clean                                                                  // cleans temp files
dotnet run                                                                    // runs solution
dotnet publish -p: PublishSingleFile=true -r win-x64 --self-contained true    // publishes the app where 
   -p: PublishSingleFile=true means to publish all files in one executable file
   -r win-x64 this is runtime identifier which is use to run this on specific runtime env only 
   --self-contained true means it is self contained with the .NET runtime in it so we can run it on any machine




