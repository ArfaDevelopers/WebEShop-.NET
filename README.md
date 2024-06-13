# WebEShop
The WebEShop is a E Commerce website. WebEShop is much simpler in regards to its current functionality and focuses on traditional Web Application Development with a single deployment.

# VERSION
ASP.NET Core 8.0.

# Running the sample locally
Most of the site's functionality works with just the web application running. However, the site's Admin page relies on Blazor WebAssembly running in the browser, and it must communicate with the server using the site's PublicApi web application. You'll need to also run this project. You can configure Visual Studio to start multiple projects, or just go to the PublicApi folder in a terminal window and run dotnet run from there. After that from the Web folder you should run dotnet run --launch-profile Web. Now you should be able to browse to https://localhost:5001/. The admin part in Blazor is accessible to https://localhost:5001/admin

# Note
If you use this approach, you'll need to stop the application manually in order to build the solution (otherwise you'll get file locking errors).

After cloning or downloading the sample you must setup your database. To use the sample with a persistent database, you will need to run its Entity Framework Core migrations before you will be able to run the app.
