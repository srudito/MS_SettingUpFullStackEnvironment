# MS_SettingUpFullStackEnvironment

## Overview

This project demonstrates a basic **Full-Stack .NET application setup** consisting of:

* **Frontend:** Blazor WebAssembly
* **Backend:** ASP.NET Core Minimal API
* **Communication:** REST API endpoints
* **Documentation:** Swagger/OpenAPI support

The project serves as a starter template for learning how to configure and run a full-stack .NET environment with separate frontend and backend applications.

---

## Project Structure

```text
MS_SettingUpFullStackEnvironment/
│
├── backend/                 # ASP.NET Core Web API
│   ├── Program.cs
│   ├── appsettings.json
│   └── Properties/
│
├── frontend/                # Blazor WebAssembly Client
│   ├── Pages/
│   ├── Layout/
│   ├── wwwroot/
│   ├── Program.cs
│   └── App.razor
│
└── Projects.sln             # Solution file
```

---

## Features

### Backend

* ASP.NET Core Minimal API
* CORS configuration enabled
* Swagger/OpenAPI integration
* Sample API endpoints:

  * `/products`
  * `/weatherforecast`

### Frontend

* Blazor WebAssembly application
* Routing and navigation support
* Counter page example
* Weather page example
* Bootstrap styling

---

## Prerequisites

Before running the project, ensure you have:

* .NET SDK 8.0 or later
* Visual Studio 2022 (recommended)

  * ASP.NET and Web Development workload
  * WebAssembly build tools

Verify installation:

```bash
dotnet --version
```

---

## Getting Started

### Clone Repository

```bash
git clone <repository-url>
cd MS_SettingUpFullStackEnvironment
```

### Open Solution

Open:

```text
Projects.sln
```

using Visual Studio 2022.

---

## Running the Backend

Navigate to the backend folder:

```bash
cd backend
```

Run:

```bash
dotnet run
```

Default endpoints:

```text
https://localhost:<port>/swagger
https://localhost:<port>/products
https://localhost:<port>/weatherforecast
```

### Sample Products Response

```json
[
  {
    "id": 1,
    "name": "Laptop"
  },
  {
    "id": 2,
    "name": "Phone"
  }
]
```

---

## Running the Frontend

Navigate to the frontend folder:

```bash
cd frontend
```

Run:

```bash
dotnet run
```

The Blazor application will launch in your browser.

Available pages:

* Home
* Counter
* Fetch Data
* Weather

---

## API Endpoints

| Method | Endpoint           | Description                          |
| ------ | ------------------ | ------------------------------------ |
| GET    | `/products`        | Returns sample product data          |
| GET    | `/weatherforecast` | Returns sample weather forecast data |

---

## Technologies Used

### Frontend

* Blazor WebAssembly
* Razor Components
* Bootstrap

### Backend

* ASP.NET Core Minimal API
* Swagger/OpenAPI
* CORS Middleware

### Development Tools

* .NET SDK
* Visual Studio 2022
* Git

---

## Learning Objectives

This project demonstrates:

* Setting up a full-stack .NET solution
* Creating Minimal APIs
* Configuring CORS
* Using Swagger for API documentation
* Building a Blazor WebAssembly frontend
* Organizing frontend and backend projects within a single solution

---

## Future Enhancements

Potential improvements include:

* Database integration (SQL Server or PostgreSQL)
* Entity Framework Core
* Authentication and Authorization
* CRUD operations for products
* API consumption from Blazor frontend
* Deployment to Azure

---

## Author

Created as part of a Full-Stack .NET environment setup and learning exercise.

---

## License

This project is intended for educational purposes.
