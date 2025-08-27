# Appointment Scheduling System

A web-based appointment scheduling application built with ASP.NET Core (.NET 5) and Entity Framework Core. It provides secure user authentication, role management, and appointment booking features for admins, doctors, and patients.

## Features

- User registration and login (with roles: Admin, Doctor, Patient)
- Admin dashboard for managing users and roles
- Appointment booking and management
- Email notifications (configurable)
- Session management
- SQL Server database integration

## Technologies Used

- ASP.NET Core MVC (.NET 5, C# 9.0)
- Entity Framework Core
- ASP.NET Identity
- SQL Server
- Razor Views

## Getting Started

### Prerequisites

- .NET 5 SDK
- SQL Server (local or remote)
- Visual Studio 2022

### Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/aman2601/Appointment_Scheduler.git
   cd Appointment_Scheduler
   ```

2. **Configure the database:**
   - Update the connection string in `appsettings.json` under `ConnectionStrings:DefaultConnection` to match your SQL Server setup.

3. **Apply migrations and seed roles/users:**
   - The application will automatically apply migrations and seed initial roles and an admin user (`admin@gmail.com` / `Aman@3323`) on first run.

4. **Run the application:**
   - Open the solution in Visual Studio 2022.
   - Build and run (F5).

### Default Admin Credentials

- **Email:** admin@gmail.com
- **Password:** Aman@3323

## Project Structure

- `Models/` - Entity and ViewModel classes
- `Controllers/` - MVC controllers for user and appointment management
- `Views/` - Razor views for UI
- `DbInitializer/` - Database seeding logic
- `Utility/` - Helper classes and utilities

## Configuration

- **Database:** Update `appsettings.json` with your SQL Server connection string.
- **Email:** Configure SMTP settings in the email sender service if email notifications are required.

## Usage

- Register as a patient or doctor, or log in as admin using the default credentials.
- Admins can manage users and assign roles.
- Doctors and patients can book and manage appointments.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the MIT License.

---

**Note:** For email notifications, configure your SMTP settings in the appropriate service class.