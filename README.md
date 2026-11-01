# inventory-tracking-system

Inventory tracking and sales application (ITSP), my final project for **BilgeAdam Academy**. A Windows desktop app built with C# WinForms on an N-tier architecture.

**Status:** Archived · **Stack:** C#, .NET Framework 4.8, WinForms, SQL Server

## Features

- Login and sign-up, with an admin panel for user management
- Product management: add, edit, delete, list stock
- Company (supplier) management
- Customer management
- Sales entry and sales list

## Architecture

```
EntityLayer/        Entities: Product, Company, Customer, Sale, User
DataAccessLayer/    Dal* classes: SQL Server queries, Connection.cs
LogicLayer/         Logic* classes: validation and business rules
IFAP_FINAL/         Presentation layer (WinForms): Login_SignUp, Admin, UC_* screens
```

The project grew out of my earlier IFAP stock-tracking app; the solution is still named `IFAP_FINAL.sln`.

## Getting started

1. Open `IFAP_FINAL.sln` in Visual Studio 2019 or later.
2. Restore NuGet packages.
3. Point the connection string in `DataAccessLayer/Connection.cs` at your SQL Server instance (default: local `.` instance) and create the tables.
4. Run the `IFAP_FINAL` (PresentationLayer) project.

## Related

- [library-management-system](https://github.com/EmreKaram/library-management-system): another BilgeAdam project
