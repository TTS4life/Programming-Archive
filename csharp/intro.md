# C#

## Installation

On Ubuntu, make sure the following packages are installed:

```
apt-transport-https dotnet-sdk-5.0

```

and isntall this `deb` package:

```
wget https://packages.microsoft.com/config/ubuntu/20.04/packages-microsoft-prod.deb -O packages-microsoft-prod.deb
```

using `sudo dpkg -i` command


## Creating a new project

To create a simple console application, create a folder for the project and execute the following: 

``` dotnet new console ```

Note: The project will take the name of the folder by default. 

Ouptut from the program will be held in the `DEBUG CONSOLE` tab on VSCode.


## Imports

Imports are done with the `using` syntax

```csharp
using System;
```

## Printing 

Printing to console is done by calling `Console.WriteLine(message)`


## Sources
[Microsoft's "Hello world" tutorial](https://docs.microsoft.com/en-us/dotnet/csharp/tour-of-csharp/tutorials/)