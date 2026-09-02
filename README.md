# Jokes Web App

A small ASP.NET Core MVC application for managing a list of jokes (question/answer format), built while following a .NET Core course to learn the framework.

## Features

- CRUD operations for jokes (create, read, update, delete)
- Search jokes by question text
- User authentication via ASP.NET Core Identity — reading jokes is public, creating/editing/deleting requires login
- Data persistence with Entity Framework Core + SQL Server LocalDB

## Tech Stack

- ASP.NET Core MVC (.NET 10)
- Entity Framework Core
- ASP.NET Core Identity
- SQL Server LocalDB
- Bootstrap

## Getting Started

### Prerequisites

- .NET 10 SDK
- SQL Server LocalDB (included with Visual Studio)

### Setup

```bash
git clone https://github.com/33Cerberus/jokes-web-app.git
cd jokes-web-app
dotnet restore
dotnet ef database update
dotnet run
```

The app will be available at the URL shown in the console (e.g. `https://localhost:7002`).

## Project Structure

```
Controllers/   MVC controllers
Models/        Data models
Views/         Razor views
Data/          EF Core DbContext and migrations
Areas/Identity/ Authentication pages
```
