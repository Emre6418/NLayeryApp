# NLayer Udemy App

This project is built on a multi-layered architecture (NLayer Architecture) using .NET Core. The project primarily provides a product management system and handles database operations with Entity Framework Core.

## Project Structure

- **Layers**:
  - **NLayer.Core**: Contains the core business logic of the project. Models and service interfaces are defined here.
  - **NLayer.Repository**: The layer that manages database operations. Database operations are performed using Entity Framework Core.
  - **NLayer.Service**: The layer where services reside. It connects database operations to the interfaces in the Core layer.
  - **NLayer.Web**: The layer that presents the project as a web-based application using ASP.NET Core MVC.

## Technologies Used

- .NET Core
- Entity Framework Core
- ASP.NET Core MVC
- SQL Server

## Installation

### Requirements

- .NET SDK (6.0 or later)
- SQL Server

### Installation Steps

1. Clone this project to your local machine:
    ```bash
    git clone https://github.com/Emre6418/NLayerUdemyApp.git
    ```
2. Navigate to the project directory:
    ```bash
    cd NLayerUdemyApp
    ```
3. Install the necessary dependencies:
    ```bash
    dotnet restore
    ```
4. Create the database:
    ```bash
    dotnet ef database update --project NLayer.Repository
    ```
5. Run the application:
    ```bash
    dotnet run --project NLayer.Web
    ```

## Usage

After starting the application, you can use it by visiting the following address in your browser:
