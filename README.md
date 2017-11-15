# MvcMusicStore


Copied from the old project of the same name previously hosted on [Codeplex](http://mvcmusicstore.codeplex.com/).

## Getting Started

### Database

The database files are located under the project's [App_Data](MvcMusicStore/App_Data) directory. The web.config is currently configured to expect the databases to be attached to SQL Server LocalDB but they can be attached to any SQL Server instance and the web.config updated appropriately.

### Users

Regular users can register through the application.

The default admin user info is:

username: administrator  
password: password123!

Additional administrative users can be added by using the ASP.NET Website Web Configuration Tool. This tool was "hidden" (i.e., no longer available directly from Visual Studio) beginning with VS 2013. However, it is still accessible through a command prompt. Instructions on how to do so can be found [here](https://blogs.msdn.microsoft.com/webdev/2013/08/19/accessing-the-asp-net-web-configuration-tool-in-visual-studio-2013/).

In the above set of instructions, the applicationUrl you will want to use is `/MvcMusicStore` as that is the name of the application in the database.