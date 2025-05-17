# 🎬 eTickets – Movie Ticket E-Commerce App

An ASP.NET Core MVC web application for online movie ticket booking with full e-commerce features, user authentication, role-based access control, and admin management.

---

## 🚀 Features

### 🎟️ 1. Movie Ticket E-Commerce Functionality

- **Movies**: Browse, filter, and view detailed information.
- **Cinemas**: Manage cinema details.
- **Producers & Actors**: Create and manage producers/actors with bios and images.
- **Shopping Cart**:
  - Add/remove movies from the cart
  - View cart summary and calculate totals
- **Orders**:
  - Place orders and view past order history
- **User Management**:
  - Admins can view and manage all users

---

### 🔐 2. Authentication & Authorization

- **Authentication**:
  - Built with ASP.NET Core Identity
  - Secure user registration, login, and logout
  - Passwords hashed and stored securely

- **Authorization**:
  - Role-based (Admin, User) using Identity roles
  - Admin-only access for movie/cinema/actor/producer management
  - Access control via `[Authorize]` and `[AllowAnonymous]` attributes
  - Custom access denied view for unauthorized actions

---

### 👤 3. User & Role Seeding

On application startup, the database is seeded with:

- **Default Roles**: Admin, User  
- **Default Users**:
  - `admin@etickets.com` / `Coding@1234?`
  - `user@etickets.com` / `Coding@1234?`

---

### 🛢️ 4. Database & ORM

- **Entity Framework Core (EF Core)** used with Code-First approach
- Migrations for schema updates
- **Models**: Movie, Cinema, Actor, Producer, Order, OrderItem, ShoppingCartItem, Identity User
- **Database**: SQL Server (connection string in `appsettings.json`)

---

### 🧱 5. Design Patterns & Architecture

- **Repository Pattern**:
  - Generic base repository for CRUD operations
- **Service Layer**:
  - Encapsulates business logic (e.g., `ActorsService`, `MoviesService`)
- **Dependency Injection**:
  - ASP.NET Core DI container for services and repositories

---

### 🎨 6. UI & Frontend

- **Razor Views**: Strongly-typed using Razor syntax
- **Bootstrap**: Responsive layout with custom dark theme
- **Partial Views & Components**: For shared UI like nav bar, cart summary, user identity
- **Validation**: Client-side and server-side validation on forms

---

### ⚙️ 7. Other Features

- **Database Seeding**: Initial data for movies, cinemas, actors, and producers
- **Session Management**: Shopping cart uses session storage
- **Error Handling**:
  - Developer exception page (dev only)
  - Custom user-friendly error pages

---

## 🧠 Built with AI Assistance

This project was developed with the help of AI tools:

- [GitHub Copilot](https://github.com/features/copilot) – for code suggestions and faster implementation.
- [ChatGPT (by OpenAI)](https://chat.openai.com) – for code guidance, explanations, and architectural decisions.

AI played a key role in helping accelerate development, debug issues, and follow best practices in .NET, EF Core, and clean architecture.

---

## 🛠️ Technologies Used

- ASP.NET Core MVC
- Entity Framework Core
- SQL Server
- Bootstrap 5
- Razor Views
- Identity (Authentication & Authorization)

---

## 📦 Getting Started

1. Clone the repository
2. Update the `appsettings.json` with your SQL Server connection string
3. Run `Update-Database` via Package Manager Console to apply migrations
4. Run the app!

---

## 📬 Contact

For questions or suggestions, feel free to reach out!

---

> Developed with ❤️ using .NET Core and a little help from AI
