# ASP.NET CORE 2.1 ADMIN PANEL TEMPLATE

There is a distinct lack of a good admin panel template with authentication for ASP.NET, so this is my take on a template that implemented authentication using ASP.NET Identity and can be used as a building block for your own admin panel portal. 

# Databases

The project is setup with Entity Framework Core and has configuration strings and libraries loaded for MS SQL, MySql or the default of SQLite. SQLite is the default so you can quickly evaluate the project, an empty SQLite database is even provided to get you going quicker.

Want to use another database? Just add the relevant Entity Framework Core libraries to the project with NuGet and edit Startup.cs.

# Getting Started

There's a couple of things you will need to do to get started with the project. 

The first thing you'll need is a [SendGrid](http://www.sendgrid.com/) API Key for receiving the email confirmation message. You can add this key to the appsettings.json file.

If you want to use a database other than the default SQLite you'll need to setup your connection string in appsettings.json, and then make a couple of changes in Startup.cs, which are documented in the file.

At this point you're pretty much set to go, just register a user, confirm your email address by clicking the link in the email you receive and then login.