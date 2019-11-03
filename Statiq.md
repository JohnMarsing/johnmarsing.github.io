# My Notes on Statiq (FKA WYAM)


- [Twitter](https://twitter.com/statiqdev)
- [Github](https://github.com/statiqdev/Statiq.Framework)
- [framework.statiq.dev](https://framework.statiq.dev/)
- https://wyam.io/

https://www.nuget.org/packages/Statiq.App
This package has a SemVer 2.0.0 package version.
This package will only be available to download with SemVer 2.0.0 compatible NuGet clients, such as Visual Studio 2017 (version 15.3) and above or NuGet client 4.3.0 and above
  -https://semver.org/spec/v2.0.0.html

- uses [LicenseZero](https://licensezero.com/) a new way to support open software developers.
-  Parity and Prosperity, that make their work free for not-for-profit or open-source users, then sell private licenses to other devs who want to use for profit or in closed source.

## The Bootstrapper -  getting started with Statiq Framework
The easiest way to get started with Statiq Framework is to use the Bootstrapper from the **Statiq.App** package. 
This class helps create an engine and has fluent methods to configure it, add modules and pipelines, and process command-line arguments.

In general, a Statiq Framework application looks something like the following:
 ```csharp
 public class Program
{
  private static async Task<int> Main(string[] args) =>
    await Bootstrapper
      .CreateDefault(args)
      .BuildPipeline(
        "Pages",
        builder => builder
          .WithInputReadFiles("**/*.md")
          .WithProcessModules(new RenderMarkdown())
          .WithOutputWriteFiles(".html"))
      .RunAsync();
}
 ``` 


 I think I may stream the creation of a new podcast website for 
@dotnetbytes
 using 
@statiqdev
, and 
@azure
 storage - for the mp3s, but also the static site :)