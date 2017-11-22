# MvcMusicStore

Copied from the old project of the same name previously hosted on [Codeplex](http://mvcmusicstore.codeplex.com/).

I use this for MTA demoing and testing purposes.

## Getting Started

### Databases

There are two databases for this app:

* [ASP.NET membership DB](MvcMusicStoreAuthDB)
* [Application DB](MvcMusicStoreDB)

The connection strings are currently configured to expect the databases to be attached to SQL Server LocalDB but they can be attached to any SQL Server instance. The connection strings are also configured to use Windows Integration Authentication, in order to test enable showing how Windows Authentication works in containers with gMSAs and CredentialSpecs. 

#### Windows Authentication
Some instructions on how to configure Windows Authentication in Docker containers can be found [here](https://stackoverflow.com/questions/47337969/integrating-windows-authentication-in-docker-container-asp-net-app/47360216#47360216).

### Users

Regular application users can register through the application.

The default admin user info is:

**username:** administrator  
**password:** password123!

Additional administrative users can be added by using the ASP.NET Website Web Configuration Tool. This tool was "hidden" (i.e., no longer available directly from Visual Studio) beginning with VS 2013. However, it is still accessible through a command prompt. Instructions on how to do so can be found [here](https://blogs.msdn.microsoft.com/webdev/2013/08/19/accessing-the-asp-net-web-configuration-tool-in-visual-studio-2013/).

In the above set of instructions, the applicationUrl you will want to use is `/MvcMusicStore` as that is the name of the application in the database.
