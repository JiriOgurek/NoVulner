<img src="https://github.com/JiriOgurek/NoVulner/blob/main/logo.png" width="500">

NoVulner! is a high-performance, easy-to-use vulnerability scanner for Microsoft .NET environment, supporting all .NET versions and all .NET languages on Windows, Linux and macOS platforms.

### Usage
Usage is quite simple, run the app with only one parameter pointing to the root of your project.

`NoVulner!.exe C:\PathToYourProject`

### Database
Application has got its own embedded database of vulnerabilities, you will be notified when it’s loaded.

`Vulnerability database from 10/05/2023 is ready.`

### Scanning
NoVulner! searches provided path recursively for all .NET assemblies (*.exe and *.dll files). You get notice, when the search finishes.

`618 assemblies found.`

Scanner analyses all found assemblies for known vulnerabilities and displays final message with
overview table like this:

`150 vulnerabilities found.`

![](https://github.com/JiriOgurek/NoVulner/blob/main/overviewTable.png)

At the end, detailed report (with all vulnerability details) is saved to an Excel file (see Support)*.

`Excel file saved.`

### Remarks
- All reported issues have to reviewed and confirmed by security expert as all the reported issues are vulnerability suspects only.
- All assemblies in ‘packages’ directory are ignored as this is the folder containing all, even unused, packages of the .NET solution. This prevents false alarm of unused vulnerable assemblies.
- When scanning your own solution ensure all projects are fully built with all the dependencies.

### Prerequisite
The only one prerequisite is .NET 7 runtime environment for your platform, download it [here...](https://dotnet.microsoft.com/en-us/download/dotnet/7.0)

### Platforms
NoVulner! supports Windows, Linux and macOS platforms.

### *Support
The basic NoVulner! is provided as-it-is by free MIT license without any support. If you are interested in getting support, up-to-date vulnerability database and full-feature edition including detail Excel reporting, ask for the commercial NoVulner! edition to support the development of this product.

