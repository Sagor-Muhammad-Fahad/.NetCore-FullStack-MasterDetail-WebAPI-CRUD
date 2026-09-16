# Employee Management System (.NET Core Web API + MVC)

A full-stack web application built using **ASP.NET Core Web API** as the backend and **ASP.NET Core MVC** as the client application. This project demonstrates a complete **Master-Detail CRUD operation** for employee profiles, along with work experience management and image upload capability.

---

## 🚀 Features

- **Full-Stack Architecture:** Clean separation of concerns with Server (API), Client (MVC), and Shared Library.
- **Master-Detail CRUD:** Manage employees alongside multiple dynamically added work experiences.
- **Image Upload & Storage:** Profile picture upload handling, preview, and server-side file deletion on update/delete.
- **Dynamic Frontend Forms:** Client-side JavaScript-driven dynamic row additions/removals for work experience titles and durations.
- **RESTful Web API:** Endpoints supporting `GET`, `POST`, `PUT`, and `DELETE` with proper HTTP status code responses (`200 OK`, `400 Bad Request`, `404 Not Found`, `204 No Content`).
- **Data Transfer Objects (DTOs):** DTOs used for form binding and JSON payload handling.
- **Circular Reference Protection:** Handled Entity Framework Core relationship loops using `NewtonsoftJson` settings.

---

## 🛠️ Tech Stack & Libraries

- **Backend:** ASP.NET Core Web API (.NET)
- **Frontend:** ASP.NET Core MVC, Bootstrap, HTML5, JavaScript (ES6), jQuery
- **Database:** SQL Server
- **ORM:** Entity Framework Core (Code-First)
- **HTTP Client:** Typed `HttpClient` (`AddHttpClient<EmployeeService>`)
- **Format / Protocol:** JSON / Multipart Form Data via HTTP

---

## 📁 Project Structure

```text
├── Server/             # ASP.NET Core Web API (Endpoints, EF Core DbContext, Controllers)
├── WebClient/          # ASP.NET Core MVC Application (Views, Controllers, EmployeeService)
└── SharedLibrary/      # Shared Models and DTOs used across Server and Client
