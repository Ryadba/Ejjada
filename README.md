# Ejjada
A business website and content-management prototype for Ejjada Building Cleaning Company, built with ASP.NET MVC and C#.
by Ryad Abdelgalil


Features
Dynamic company website
Services, benefits, and “Why Us” sections
Company information and service descriptions loaded from a database
Bootstrap-based responsive layout
Image galleries, testimonials, sliders, and contact content
Custom administration controllers for editing website content
Entity Framework database models and migrations
ASP.NET account and authentication views
Separate public and administrative areas
Technology
C#
ASP.NET MVC 4
ASP.NET Web API
Razor views
Entity Framework 5
.NET Framework 4.5
Visual Studio 2013
SQL Server-compatible Entity Framework context
Bootstrap 3
jQuery
Knockout.js
LESS
SMTP email support
Project Structure
Text
Ejjada/
├── App_Data/        Local application data
├── App_Start/       Routing, bundles, filters, and Web API configuration
├── Controllers/     Public pages and content-management controllers
├── Migrations/      Entity Framework migration configuration
├── Models/          Database entities and view models
├── Services/        Mail service abstractions
├── Views/           Razor pages and CRUD forms
├── Content/         CSS, LESS, themes, galleries, and website assets
└── Scripts/         JavaScript and third-party libraries
Database and Content Models
The application uses EjjadaDb1, an Entity Framework DbContext, with database sets for:

Services
Benefits
“Why Us” points
Service descriptions
About-us descriptions
The public pages combine these records into a view model and render them dynamically.

Administration
The project contains CRUD functionality for:

Services
Benefits
“Why Us” content
Service descriptions
About-us descriptions
Each CRUD area provides create, edit, details, and delete views.

The README also refers to /SuperAdmin as a hidden/custom CMS entry point.

Running the Project
Open Ejjada.sln in Visual Studio.
Restore or verify the included NuGet packages.
Configure DefaultConnection1 in Web.config.
Ensure SQL Server is available and compatible with Entity Framework 5.
Apply or enable the Entity Framework migrations if needed.
Build and run the project using IIS Express.
The project targets .NET Framework 4.5, so it requires a compatible Windows and Visual Studio environment.

Configuration Notes
Before deployment:

Configure the database connection in Web.config.
Seed or migrate initial website content.
Configure SMTP settings if the contact form is enabled.
Restrict /SuperAdmin and every CRUD controller with authentication and authorization.
Review uploaded or committed image assets.
Add HTTPS and security headers.
