# MVC101 - ASP.NET Core MVC Playground

This is a template project built with ASP.NET Core MVC to explore and learn the fundamentals of Model-View-Controller architecture in .NET.

## Project Overview

- **Framework**: ASP.NET Core 9.0
- **Project Type**: Web Application (MVC)
- **Language**: C#
- **Development Environment**: Visual Studio 2022

## Features

- Standard MVC project structure
- Built-in authentication and authorization
- HTTPS configuration
- Static file serving
- Pre-configured routing
- Development/Production environment settings

## Project Structure

```
├── Controllers/         # Contains MVC controllers
│   └── HomeController.cs
├── Models/             # Data models and view models
│   └── ErrorViewModel.cs
├── Views/              # Razor views and layouts
│   ├── Home/
│   │   ├── Index.cshtml
│   │   └── Privacy.cshtml
│   └── Shared/
│       └── _Layout.cshtml
└── wwwroot/           # Static files (CSS, JS, images)
    ├── css/
    ├── js/
    └── lib/
```

## Getting Started

### Prerequisites

- .NET 9.0 SDK or later
- Visual Studio 2022 or your preferred IDE

### Running the Project

1. Clone the repository
2. Open the solution in Visual Studio
3. Press F5 or click "Run" to start the application

The application will start on:
- HTTPS: https://localhost:7021
- HTTP: http://localhost:5192

## Configuration

- `appsettings.json` - Main configuration file
- `appsettings.Development.json` - Development-specific settings
- `Properties/launchSettings.json` - Launch profiles and environment settings

## Available Routes

By default, the application uses a conventional routing pattern:
```
{controller=Home}/{action=Index}/{id?}
```

## Development Features

### Hot Reload
Hot Reload automatically applies code changes to your running application without requiring a manual restart. In ASP.NET Core MVC:
- Views (.cshtml files) support runtime compilation and updates
- C# code changes are applied while debugging
- Works in both Visual Studio and `dotnet watch`
- Limitations: Some changes like method signature updates require restart

Other Features:
- Development exception page with detailed error information
- HTTPS redirection
- Static file middleware
- MVC view compilation

## Contributing

This is a playground project meant for learning and experimentation. Feel free to:
- Fork the repository
- Create your feature branch
- Experiment with different MVC features
- Share your learnings

## License

This project is open-source and available for learning purposes.

## Additional Resources

- [ASP.NET Core Documentation](https://docs.microsoft.com/en-us/aspnet/core/)
- [MVC Pattern](https://docs.microsoft.com/en-us/aspnet/core/mvc/overview)
- [Razor Syntax](https://docs.microsoft.com/en-us/aspnet/core/mvc/views/razor)