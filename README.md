# 100 Must-Know .Net Core Interview Questions

<div>
<p align="center">
<a href="https://devinterview.io/questions/web-and-mobile-development/">
<img src="https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/github-blog-img%2Fweb-and-mobile-development-github-img.jpg?alt=media&token=1b5eeecc-c9fb-49f5-9e03-50cf2e309555" alt="web-and-mobile-development" width="100%">
</a>
</p>

#### You can also find all 100 answers here 👉 [Devinterview.io - .Net Core](https://devinterview.io/questions/web-and-mobile-development/net-core-interview-questions)

<br>

## 1. What is _.NET Core_ and how does it differ from the _.NET Framework_?

**.NET Core** and **.NET Framework** are both ecosystem variations developed by Microsoft. They share similar libraries, syntax and core components, yet have distinctive characteristics and purposes.

### Key Distinctions

#### Dependency on Operating System

   **.NET Core** is built to fluctuate across operating systems, providing reliability from Windows, macOS, and Linux.

   **.NET Framework's** exclusive residence is on Windows.

#### Deployment Mechanisms

   For **.NET Framework**, components are distributed through a Global Assembly Cache (GAC).

   In contrast, **.NET Core** utilizes its open-source library format. All essential dependencies are gathered during the runtime of the hosting system.

#### Stack Structures

   **.NET Core** is modular in design, permitting you to streamline the allocation of resources. This means that resources from .NET Core can be combined with resources from other packages or your code, and any unused resources will be left out of the final deployment.

   **.NET Framework** resources are all-inclusive. Every application constructed within the .NET Framework will use the complete stack of associated resources.

#### API Accessibility

   **.NET Core** highlights a subset of libraries accessible across all operating systems. This ensures consistent performance among various platforms.

   On the contrary, **.NET Framework** provides in-depth access to exclusive Windows APIs, which might not resonate well with non-Windows platforms.


### Targets and Use-Case Scenarios

#### .NET Core-Based Projects

- Cloud-First Deployments: Given its lightweight factor, numerous platforms host applications from **.NET Core**.
- Applications involving containers: **.NET Core** is particularly suitable, bearing its minimalistic resource usage.
- Web-based applications: **.NET Core** is a strong contender due to its inbuilt support for client-server architectures and cloud-based applications.

#### .NET Framework-Based Projects

- Long-Running Applications: Applications with consistent and prolonged operational times will significantly benefit from using **.NET Framework**.
- Established Windows-centric applications: **.NET Framework** still reigns as the preferred choice, especially for applications deeply embedded within Windows ecosystems or those leveraging platforms such as Silverlight or WPF.
- Specific APIs: If your application necessitates specialized Windows APIs that aren't accommodated by **.NET Core**, **.NET Framework** remains the ultimate choice.
<br>

## 2. Describe the cross-platform capabilities of _.NET Core_.

**.NET Core** is a framework for developing cross-platform applications.

### Key Cross-Platform Features

- **Libraries**: Provides a consistent set of libraries across operating systems. Developers can use these libraries seamlessly, ensuring that functions work consistently across environments.

- **Runtime Environment**: .NET Core applications are run using a runtime environment that adapts to the underlying system. The runtime handles critical tasks like memory management and garbage collection.

- **Cross-Platform Support**: Code written using .NET Core runs on various operating systems without modifications. This allows developers to target a broad range of devices and environments.

- **Platform-Dependent Code Paths**: In some cases, developers may need to differentiate between OS variants. .NET Core offers mechanisms for handling platform-specific code, enabling conditional execution.

- **NuGet Packages and Package Management**: .NET Core supports NuGet packages, simplifying the inclusion of third-party libraries. It helps ensure that dependencies are resolved consistently, regardless of the target system.

- **Code Execution**: .NET Core supports multiple development idioms, including Just-In-Time (JIT) compilation and ahead-of-time (AOT) compilation. These features enable code execution tailored to the system, optimizing performance.
<br>

## 3. What are the main components of the _.NET Core architecture_?

The architecture of the .NET Core platform revolves around modularity, flexibility, and platform independence.

### Key Components of .NET Core

#### Core Features

- **Framework and BCL**: The BCL (Base Class Library) provides fundamental classes and types, while the Core Framework encompasses core libraries and runtime services.
  
- **Garbage Collector**: The GC in .NET Core ensures automatic memory management by alleviating developers from manual memory cleanup, thus minimizing memory leaks and memory management issues.

- **Just-in-Time (JIT) Compiler**: .NET Core translates Intermediate Language (IL) code into machine code, enabling cross-platform execution.
  
- **Multi-level Compilation**: .NET Core employs both on-demand **JIT** compilation and **Ahead-of-Time (AOT)** compilation for specific scenarios.

- **Portable PDB Format**: This component simplifies debugging across different environments.

- **Exception Handling and Stack Trace Mechanism**: These built-in mechanisms aid in robust error handling and debugging.

- **Native Interoperability (P/Invoke)**: .NET Core interacts with native code such as DLLs using the P/Invoke mechanism.

- **Build and Packaging Tools**: .NET Core's build and packaging mechanisms streamline deployment to various platforms.

#### Tools and Interfaces

- **CLI**: The Command-Line Interface offers a powerful, text-based toolset for building, managing, and deploying .NET Core applications.

- **Global Tooling Management**: This system facilitates the installation and lifecycle management of global .NET Core tools.

#### Execution Environments

- **.NET Core Application Host**: This component hosts and manages the execution of .NET Core applications.

- **Operating System Abstraction**: .NET Core provides a unified set of APIs for interacting with the underlying operating system, ensuring consistency across platforms.

- **Cross-Platform Compatibility Layer**: This layer simplifies multi-platform development by streamlining interactions between the application and various operating systems.

#### Libraries and Dependencies

- **NuGet Package Manager**: The default package manager for .NET Core simplifies the acquisition and management of third-party libraries.

- **.NET Core-specific NuGet Packages**: These packages are tailored for the .NET Core ecosystem.

- **.NET Standard Libraries**: These are a consistent set of APIs shared across .NET platforms.

- **Project References and NuGet Dependency Management**: These tools streamline library dependencies within .NET projects.

#### Compiler and Build Toolset

- **.NET Compiler Platform (Roslyn)**: Roslyn serves as the C# and Visual Basic compiler system, providing dynamic code analysis and transformation capabilities.

- **MSBuild**: This build engine offers comprehensive control over the build process and is notable for its project-file-based build configuration.

- **NuGet Package Restoration**: The .NET tooling automatically restores **NuGet** packages for a project as part of the build process.

#### Containers and Microservices

- **Docker Support**: .NET Core applications can be containerized using Docker for portability and consistency across diverse environments.

#### Network Integration

- **HTTP Components**: .NET Core has a range of HTTP-related tools, including an embedded web server, support for SSL, and client-side HTTP capabilities.

- **WebSocket Support**: The platform supports WebSockets for efficient, bi-directional communication.

#### Data Persistence and Management

- **Entity Framework Core**: As the object-relational mapper (ORM) of choice for .NET Core, this component simplifies database interactions.

- **Data Provider Abstraction**: .NET Core abstracts database providers, allowing applications to work with different databases without extensive modifications.

- **Data Access and Querying Tools**: It offers various methods for robust data access and querying, such as LINQ and ADO.NET.

- **In-memory Data Storage**: For transient data storage requirements, .NET Core provides in-memory data storage capabilities.

- **File I/O and Storage Integration**: The platform includes robust file-handling utilities.

#### Security and Cryptography

- **Authentication and Authorization Frameworks**: .NET Core offers features for secure user and service authentication and authorization.

- **Cryptography Services**: It provides a suite of cryptographic tools for secure data handling.

- **Code Access Security (CAS)**: This component defends against potential security vulnerabilities by controlling code execution.

#### Text and Localization

- **Text Manipulation Utilities**: .NET Core includes a plethora of text-related tools, like string manipulation methods and string encoding controls.

- **Globalization and Localization Components**: These components aid in the management of region-specific and multilingual applications.

#### UI and Presentation

- **Presentation Frameworks**: .NET Core provides frameworks for constructing diverse graphical user interfaces.

- **ASP.NET Core for Web Applications**: This web framework is tailored for building modern web applications and services.

- **Blazor for Web Applications**: This innovative web development framework allows for client-side applications with C#.

- **WPF, WinForms, and Universal Windows Platform (UWP)**: These established frameworks enable desktop and Windows-specific application development.

- **Gtk# for Cross-Platform Desktop Applications**: This component provides a set of .NET bindings for the GTK+ toolkit.

- **Mobile-Specific Frameworks**: For mobile application development, .NET Core integrates with Xamarin.
<br>

## 4. Explain the _.NET Core CLI_ and its primary functions.

Let's look at the **.NET Core CLI** and its primary operations: **new**, **build**, **publish**, **run**, **test**.

### New

The **new** command initializes a new .NET project using a specific template. You can choose from project types like console applications, web applications, class libraries, and more.

### Build

With the **build** command, you can compile your source code into an executable format or a library. It also resolves project dependencies and creates an assembly.

### Publish

The **publish** command gathers necessary components for an application, like the .NET Core runtime, and **prepares it for deployment**. This ensures the target machine has the relevant runtime and runtime components.

### Run

The **run** command simplifies the process of executing your application. It does this by **combining building and execution tasks** into a single, more straightforward step.

### Test

Use the **test** command to execute tests in the project. The .NET Core Test Explorer, VS Code, or Continuous Integration (CI) systems like Azure Pipelines or Jenkins can also run these tests.

### Simplified Workflow

These CLI commands simplify the development process. You can transition from creating a new project to building, testing, and running it, all from the command line. These commands save time and make development more efficient.
<br>

## 5. How do you create a new _.NET Core project_ using the _CLI_?

To create a new **.NET Core** project using the command line:

### Step 1: Install the .NET Core SDK

If you haven't already, install the **.NET Core SDK**. This provides the necessary **tools** and **libraries** for developing in .NET.

### Step 2: Run the `dotnet new` Command

Use the `dotnet new` command to **create** a new .NET Core project. This command offers various **project templates**, such as for web APIs, console applications, and more.

Here is the syntax:

```bash
dotnet new <TEMPLATE_NAME> [-n <PROJECT_NAME>] [-o <OUTPUT_DIRECTORY>]
```

- Substitute **`<TEMPLATE_NAME>`** with the desired project template like `console`, `webapi`, `mvc`, etc.
- Optionally, set a **`<PROJECT_NAME>`** and an **`<OUTPUT_DIRECTORY>`**.

### Example: Running `dotnet new` to Create a Console App

Use the following command:

```bash
dotnet new console -n MyConsoleApp -o MyConsoleAppDir
```

- **TEMPLATE_NAME**: `console`
- **PROJECT_NAME**: `MyConsoleApp`
- **OUTPUT_DIRECTORY**: `MyConsoleAppDir`

This will create a new **console application project** with the name `MyConsoleApp` and place it in the `MyConsoleAppDir` folder.
<br>

## 6. Discuss the purpose and use of a `csproj` file in a _.NET Core project_.

The **C# project file** (`*.csproj`) serves as a **configuration manifest** for .NET Core projects, providing a wealth of options for customizing your build process, declaring project dependencies, and adjusting compiler settings.

The `csproj` file is based on the more general `msbuild` format and has had several iterations as new features are introduced.

### Key Elements

#### Directives for .NET Targeting

- **Target Framework**: Defines the version and profile of the .NET runtime you're targeting. For multi-platform projects like Xamarin, it can differentiate between platforms.

- **Type of Output File**: It is usually a .dll or .exe file.

#### Building and Debugging Configuration

- **Output Type**: Selects the kind of .NET assembly produced.
- **Debug Symbols Generation**: Decide whether to create debug symbols for better debuggability.

#### Sources Organization

- **Source Files**: Provides a list of source files to be included in the project.

- **Resources**: Offers a way to incorporate non-code files like images or text files.

#### Compiling Directives

- **Conditional Compiles**: Conditional symbols can be set to determine which part of the code gets compiled.

- **Option to Treat Warnings as Errors**: Warnings can be forced to be treated as errors.

- **Optimizations**: You can control whether the compiler optimizes your code for a fast build or a smaller assembly.

#### Dependencies Management

- **Core Assemblies Membership**: The project lists the essential .NET Core assemblies it depends on.

- **NuGet and Direct Dependencies**: The file signals dependencies through multiple methods, helping the framework to acquire necessary packages.

- **Framework Assemblies**: It can include or exclude assemblies that are part of the .NET Core library.

- **Private Library Folder**: It lets you specify a location to search for libraries not on NuGet.

#### Customization Through Directives

-  **Custom Tasks**: This feature allows you to run custom tasks as part of the build process.

- **Event-Based Integration**: In some cases, you might want to execute custom actions during specific build events (like "BeforeBuild" or "AfterRebuild").

#### Project Settings

- **Project Type**: It distinguishes between different types of projects like web applications or class libraries.

- **Default Namespace**: You can set a default namespace for classes created in the project.

#### Code Analysis and Best Practices

- **Code Style Rules**: By setting various style rules, you can enforce a consistent coding style in all the projects throughout your solution.

- **Docs and Localization**: It supports inclusion of documentation and localization files.

#### Cross-Platform Considerations

- **Mono and .NET Compact Framework**: It enables developers to target platforms based on Mono or the .NET Compact Framework.

- **Cross-Platform Execution**: For different platform targets or compatibility modes, the setting ensures the correct execution of the project.

### .NET Core SDK Versioning and Evolution

The `.csproj` underwent significant simplifications in conjunction with the release of .NET Core 3.0, aiming to streamline project file definitions and make them more standardized and modular across project types.

Through continuous updates and community feedback, the project file remains central to the management and orchestration of .NET Core projects.
<br>

## 7. What is the _runtime_ and _SDK_ in _.NET Core_?

The **.NET Core** framework is a versatile, modular platform for developing cross-platform applications. It delivers its core libraries, tools, and runtime as an integrated package.

### Two Essential Components

1. **.NET Core Runtime**: This environment is necessary for executing .NET Core applications. It's typically distributed as a single deployable unit, ensuring that applications are self-contained and alleviating the need for separately installed .NET runtimes.

2. **.NET Core SDK**: Integrating essential tools like the compiler, NuGet package manager, and MSBuild, the SDK empowers developers to build, test, and publish applications. Its comprehensive suite of libraries and APIs supports development across a range of applications and industries.

### Compatibility Considerations

The version of the .NET Core runtime specifies the advertised **API compatibility level** and **previously introduced feature sets**.

Developers outline any framework version dependencies in their applications through the use of the `<TargetFramework>` element in the project file.

### Code Example: Project File with Target Framework

```xml
<Project Sdk="Microsoft.NET.Sdk">
  <PropertyGroup>
    <OutputType>Exe</OutputType>
    <TargetFramework>netcoreapp3.1</TargetFramework>
    <TreatWarningsAsErrors>true</TreatWarningsAsErrors>
  </PropertyGroup>
</Project>
```

### Managing Multiple .NET Core Versions

The .NET Core SDK provides a command-line tool, `dotnet`, which enables you to monitor various installed versions and switch between them seamlessly. Use the `global.json` file in your project to fix the specific SDK version for your project or a range of projects.

### Code Example: Global.json

```json
{
  "sdk": {
    "version": "3.1.402"
  }
}
```
<br>

## 8. How would you manage different versions of the _.NET Core SDK_ on the same machine?

You can use **`global.json`** files and specify the version of the .NET SDK you wish to target within a project. When you run `.net build` or `.net run` in a directory that contains a global.json file, the SDK version specified in that file takes precedence over any other installed versions.

Here is a code snippet showing how to write a `global.json` file:

```json
{
  "sdk": {
    "version": "2.1.402"
  }
}
```
<br>

## 9. What is the purpose of the `global.json` file?

The `global.json` file in a .NET Core project defines the version of the SDK used and allows for **multi-project management**.

It also assists with:

- **Managing SDK Versions**: By setting the `sdk` field to a specific version, you ensure consistent behavior across development environments and CI/CD pipelines. Additionally, the `allowPrerelease` flag gives you control over using preview versions.

- **Setting Default Paths for Global Packages and Tools**: The `packageManagement` and `tools` fields can be helpful in specifying directory paths for global tools and packages. This can simplify configuration on new machines or during deployment. For instance, you can use it to set up the same configuration across machines of your team.

- **Coordinating Multi-Project Solutions**: A `global.json` file helps manage **consistent SDK versions and ensures that inter-related projects within a solution are either using the same version or compatible ones. This coordination is essential for projects that *depend* on each other, especially in a CI/CD environment.

### Global SDK vs. Local SDK

The SDK version specified in the `global.json` usually supersedes the locally installed SDK version unless the local version is explicitly pinned, or there's a higher priority, such as in a project-specific `global.json` file.

**When shared**, the `global.json` settings apply to all projects within its directory and those in subdirectories unless they have their own `global.json` files, which would then take precedence.

**If you're pushing software to production**, always account for SDK versions and set up your CI/CD pipelines accordingly. For consistency and to guard against unintended version updates, you should generally specify the SDK versions in your build configurations, rather than relying solely on the local environment of the build agent or developer machines.
<br>

## 10. Can you explain the _Directory Structure_ of a typical _.NET Core project_?

The directory structure of a typical .NET Core project is designed to keep code organized and manageable.

### Key Directories

- **src**: Contains the core application and all of its modules.

- **tests**: Houses unit, integration, or end-to-end test projects.

- **docs**: For documentation files.

- **artifacts**: Not always present, but used for build outputs (e.g., binaries).

- **build**: For build-related scripts or files.

- **.github**: GitHub-specific files like workflows or issue templates.

- **.vscode**: Configurations specific to Visual Studio Code.

### Core Files

- **global.json**: Might specify the version of the .NET SDK to use.
  
- **.gitignore**: Lists files and folders to exclude from version control.
  
- **.editorconfig**: Gives project-wide text editor settings.
  
- **.wslconfig**: This is an optional file which you can create to configure the Windows Subsystem for Linux

- **Dockerfile**: If the project uses Docker, this defines the container.

- **Makefile**: Optional file used to automate tasks on Unix-based systems.

### Build-Related Files

- **.editorconfig**: Provides consistent coding styles for multiple developers working across various editors and IDEs.

- **global.json**: Helps specify the SDK version used for the project.

- **MyApp.sln**: Solution file associated with Visual Studio, listing project dependencies and configurations.

- **nuget.config**: Configures NuGet package sources.

- **local-mira-tool.manifest**: Specifies the version targeted by Mira, a cross-platform CLI.

### Dynamic/Generated Files

- **appsettings.json**: JSON configuration file translated to `Configuration` objects.

- **appsettings.Development.json**: App-specific data for the Development environment.

- **appsettings.Production.json**: Environment-specific data for the Production environment.

- **MyApp.deps.json**: Dependency details.

- **MyApp.runtimeconfig.json**: Runtime-related information like shared frameworks and native libraries.

### Version Control

- **.git**: Git repository.

- **.gitattributes**: Used to customize how versions of files should be handled.

- **.gitignore**: Lists files and folders to be excluded from version control.
<br>

## 11. How do you add and manage _NuGet packages_ in a _.NET Core project_?

Working with **NuGet** in a **.NET Core** project is seamless, thanks to Visual Studio and the dotnet CLI. Whether you're a fan of the GUI or prefer command-line superiority, you can manage NuGet packages without breaking a sweat.

### Using NuGet Package Manager UI

1. **Locate NuGet Package Manager**:
   - In Visual Studio, access it via `Project > Manage NuGet Packages...`.

2. **Browse for Packages**:
   - Look for packages in the NuGet.org online repository under the "Browse" tab.

3. **Install Packages**:
   - Click "Install" for the desired package.

4. **Verify Installations**:
   - Check the "Installed" tab to see the installed packages.

#### Useful Tips

- **Version Management**: Click on the installed package to see other available versions.
  
- **Updating Packages**: Navigate to the "Updates" tab to see which packages have newer versions.

- **Uninstalling**: Use the "Installed" tab to remove packages.

### Managing Packages via .NET CLI

Use the `dotnet add package` and `dotnet remove package` commands.

#### Syntax

- **Add Package**:
  ```bash
  dotnet add package PackageName
  ```
- **Remove Package**:
  ```bash
  dotnet remove package PackageName
  ```

- **Update Package**:
  ```bash
  dotnet add package PackageName --version 1.2.3
  ```


#### Using Private Feeds

- **Configuring**: In `nuget.config`, define the source, or use `-s`/`--source` in the CLI. E.g.:
  ```bash
  dotnet add package CompanyPackage --source https://NuGetServer.com/nuget/MyPrivateFeed/
  ```

  **Authentication**: For authenticated feeds, use `.config` files or `-k`/`--api-key` along with the command.


### Using NuGet.Config

- **Creating**: Use the `new` command to create a config file in your solution folder:
  ```bash
  dotnet new nugetconfig
  ```

- **Configuring Sources**: With the `add source`  command:
  ```bash
  dotnet nuget add source https://AnotherFeed.com/v3/index.json --name AnotherFeed
  ```

  And to remove a source:
  ```bash
  dotnet nuget remove source AnotherFeed
  ```

- **Setting Default Push Source**: Utilize the `push` command:
  ```bash
  dotnet nuget push -t API_KEY MyPackage.1.0.0.nupkg
  ```
  Use the `-s`/`--source` switch to specify the desired push source.

### Docker and NuGet

To use a cache layer when adding packages in a Docker container, first retrieve and add the `.csproj` file to the container before executing the `dotnet restore` command. This approach speeds up the build process.

#### Dockerfile Example

```Dockerfile
# Copy .csproj and nuget.config and restore as distinct layers
COPY nuget.config ./
COPY Orcha.csproj ./
RUN dotnet restore
```
<br>

## 12. Explain the role of the _NuGet package manager_.

The **NuGet Package Manager** simplifies the process of integrating external libraries and components into your project. It's a core element in the Microsoft toolchain and is closely integrated with .NET Core, Visual Studio, and Visual Studio Code.

### Key NuGet Package Manager Capabilities

1. **Package Management**: NuGet serves as a centralized repository for .NET packages, where developers can easily search, discover, and install packages.

2. **Dependency Management**: NuGet tracks and resolves dependencies between packages, ensuring that all required components are downloaded and installed.

3. **Version Control**: Different versions of the same package are maintained, giving developers flexibility in choosing the most suitable one for their project.

4. **Project Scopes**: NuGet allows you to define packages at various levels such as the global package store, the project-local store, or as a package reference within a project file.

5. **Commands via CLI**: Besides GUI integration, NuGet supports a powerful command-line interface for streamlined package management.

6. **Publishing Packages**: It facilitates package creators in distributing their libraries to the global NuGet repository for wider consumption.

7. **Extensibility**: NuGet allows for easy management of third-party tools and integrations, beyond just code libraries.

### NuGet in Action: A Simple Example

Here is what you should do:

- In Visual Studio, open a .NET Core project.
- Right-click on the project in the Solution Explorer and choose "Manage NuGet Packages".
- Click on "Browse" and search for "Newtonsoft.Json", a commonly used JSON parsing library.
- Click "Install" to add the package to your project.

This will modify your project file, adding a `<PackageReference>` to `Newtonsoft.Json` and any of its dependencies.
<br>

## 13. Describe the process of _publishing a .NET Core application_.

When publishing a **.NET Core application**, you compile it and its dependencies for deployment. .NET Core supports various publishing methods and configurations to cater to your specific requirements.

### Various Publishing Methods

1. **Framework-Dependent**: Publishes the app without the .NET Core runtime. It indicates which version to use on the target system. The app will only run on systems with matching or newer .NET Core runtimes.

2. **Self-Contained**: Packages the app with the .NET Core runtime, allowing it to run on systems without an existing .NET Core installation.

3. **Portable**: Typically suitable for use-cases like USB flash or external drives.

4. **Ready-To-Run**: Optimizes the app startup time by pre-compiling specific libraries to native code. RTR has the added benefit of being useful for promoting cross-gen and unification common. Thus, **RTR Is the default for these modes vs traditional JIT**.

### Publishing Commands

The Dotnet Command Line produces build artifacts onto the file system. 

- **dotnet build** compiles the app.
- **dotnet publish** copies necessary files to a target path, to make it ready for deployment.

### Project Files for Publishing

The following configuration settings can be specified in your project file to influence the publish process:

- **PublishWithAspNetCoreTargetManifest**: For web apps, this setting specifies whether the app should be published with or without an AspNetCore target manifest.

- **PublishTrimmed**: When set to 'true', minimizes the number of assemblies included in the published output based on necessary. This improves performance & size.



An example DOTNET CLI command for publishing a self-contained app would look like this:

```sh
dotnet publish -c Release --self-contained --runtime linux-x64
```

And for ready-to-run (RTR), it would be:

```sh
dotnet publish -c Release --runtime linux-x64 --self-contained false --output rtr/path
```

When the **Ready-To-Run** is specified, the `--self-contained` and `--output` are disabled.

For deploying to Linux or Windows in **framework-dependent** mode:



```sh
dotnet publish -c Release --runtime linux-x64
```

```sh
dotnet publish -c Release --runtime win-x64
```

### Repositories, NuGet & Web



-  **Repository**: Useful for sharing the project's source code publicly. Code hosting platforms such as GitHub, GitLab or Bitbucket support repository management.
  
- **NuGet Package**: Ideal for publishing libraries as it simplifies their consumption. Once you've published a library to NuGet, others can include it as a dependency in their projects.
  
-  **Web Host**: For web applications and services, hosting them with a web server is essential.  When you deploy to a web server, ensure your web.config file is correctly configured for its needs. Additionally, when using Kestrel, ensure it's accessible through a proxy server.
<br>

## 14. What is a _.NET Standard_ and how does it relate to _.NET Core_?

**.NET Standard** serves as a formalized set of APIs, ensuring cross-compatibility among different .NET implementations. Essentially, it is a standardized interface that abstracts from the underlying platform.

### Motivation for .NET Standard

Before .NET Standard, developers had to detect and account for the specific platform they were targeting, such as UWP or different versions of .NET Framework. This diversity resulted in interoperability challenges.

By establishing a standardized target across .NET implementations, **.NET Standard** simplifies multi-platform development, making it more cohesive and intuitive.

### Evolution of Development Platforms

While '.NET Core' and '.NET Framework' cater to specific use cases, **.NET Standard** essentially aims for cross-compatibility. As of 2020, Microsoft advocated for using '.NET Core' for newer projects.

Here is the overview:

- **.NET Framework**: It's a mature, all-in-one development platform for Windows-based applications.
- **.NET Core**: A streamlined, open-source platform shattering Windows allegiance, targeting both Windows and non-Windows systems.
- **.NET 5**: A unification of ".NET Core" and ".NET Framework".
- **.NET 6 **: The next leap, evolving further from ".NET 5".

Given this diverse landscape, **.NET Standard** acts as an umbrella platform with defined capabilities and APIs, ensuring consistent behavior across different .NET implementations.
<br>

## 15. How do you create a _class library_ in _.NET Core_?

To create a **Class Library** in .NET Core, you can use either Visual Studio or the `dotnet` command-line interface.

### Using Visual Studio

- Open Visual Studio.
- Select "Create a new project".
- Choose the "Class Library" template under the "C#" or appropriate language heading.
- Specify the project name and location.
- Click "Create".

### Using the .NET CLI

1. **Create the Project**: Open a terminal and navigate to the desired directory. Run the following command:

   ```bash
   dotnet new classlib -n MyLibrary
   ```

   Replace `MyLibrary` with your preferred project name.

The above command will generate a `.csproj` file, which is the project file for the class library.

2. **Configure the Project Reference**:

   You can either manually add the reference or use the `dotnet add reference` command. Manually, you would do this editing the `.csproj` file:

   ```xml
   <ItemGroup>
       <ProjectReference Include="..\Path\To\AnotherProject.csproj" />
   </ItemGroup>
   ```

   Using the command line:

   ```bash
   dotnet add reference ..\Path\To\AnotherProject.csproj
   ```

   This connects your class library to your other projects or external libraries.

### Visual Studio Code

You can create a class library in Visual Studio Code using the .NET CLI. Here is how:

1. **Initialize the Project Folder**:

   Open the terminal in the desired directory and run:

   ```bash
   dotnet new sln -n MySolution
   ```

   Replace `MySolution` with your preferred name.

2. **Create the Library Project**:

   Run the following commands in the terminal:

   ```bash
   dotnet new classlib -n MyLibrary -o MyLibrary
   ```

   This creates a new directory named `MyLibrary` and initializes it as a class library.

3. **Add the Library to the Solution**:

   To include the library in the solution, run:

   ```bash
   dotnet sln add MyLibrary/MyLibrary.csproj
   ```

4. **Link to Other Projects or Libraries**:

   You can **add a project reference**:

   ```bash
   dotnet add reference ..\Path\To\AnotherProject.csproj
   ```

   Or **add a package reference**:

   ```bash
   dotnet add package MyPackage
   ```

5. **Build the Solution**:

   To ensure everything is linked up correctly, build the solution with:

   ```bash
    dotnet build
   ```

   The class library and any linked projects should build without errors.
<br>



#### Explore all 100 answers here 👉 [Devinterview.io - .Net Core](https://devinterview.io/questions/web-and-mobile-development/net-core-interview-questions)

<br>

<a href="https://devinterview.io/questions/web-and-mobile-development/">
<img src="https://firebasestorage.googleapis.com/v0/b/dev-stack-app.appspot.com/o/github-blog-img%2Fweb-and-mobile-development-github-img.jpg?alt=media&token=1b5eeecc-c9fb-49f5-9e03-50cf2e309555" alt="web-and-mobile-development" width="100%">
</a>
</p>

