## Inventory Management CRUD Platform

A full-stack inventory management web application developed as part of WGU’s Software Engineering program.  
This application is designed to simulate a real-world store management system using a classic MVC architecture.

> 🔒 **Note:** This repository contains a project overview only.  
> The full source code is kept private in compliance with WGU’s Academic Authenticity Policy.  

---

### Project Summary

This system allows store managers to:

- View, create, update, and delete **products** and **parts**
- Navigate through a clean, user-friendly web UI
- Use a **"Buy Now"** button to simulate product purchase
- Enforce **inventory validation** using minimum and maximum stock boundaries
- Auto-load **sample inventory** (5 products + 5 parts) on first run
- Display store information through a dedicated **About** page
- Run **unit tests** to verify inventory constraint logic

The application was built based on a UML diagram and starter template. All controller logic, validation, and UI customization were implemented from scratch.

---

### Tech Stack

| Layer      | Technology                           |
|------------|---------------------------------------|
| Frontend   | HTML, CSS, Thymeleaf, Bootstrap 5     |
| Backend    | Java 17, Spring Boot 2, Spring MVC    |
| Database   | MySQL 8                               |
| Build Tool | Maven                                 |
| IDE        | IntelliJ IDEA Ultimate (Student License) |
| Testing    | JUnit 5                               |

---

### Project Structure

<pre>
inventory-app/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/inventory/
│   │   │       ├── controller/           ← Web controllers
│   │   │       ├── model/                ← Domain models (Part, Product)
│   │   │       ├── service/              ← Business logic layer
│   │   │       └── InventoryApp.java     ← Application entry point
│   │   └── resources/
│   │       ├── templates/                ← Thymeleaf HTML views
│   │       │   ├── index.html
│   │       │   ├── partForm.html
│   │       │   └── about.html
│   │       └── application.properties    ← DB config, server port, etc.
│
├── test/
│   └── java/com/example/inventory/
│       └── PartTest.java                ← JUnit tests for inventory logic
│
└── pom.xml                              ← Project dependencies & build config
</pre>

