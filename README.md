# Laravel Backend Service

This is a Laravel-based backend service using **SQLite** as the database and **Laravel Sanctum** for API authentication.

## 📦 Requirements

Before running the project, make sure you have the following installed:

- PHP >= 8.1
- Composer
- SQLite (comes pre-installed with most PHP installations)
- Git (optional but recommended)

## 🚀 Getting Started

Follow these steps to set up and run the backend service:

---

### 1. Clone the repository

```bash
git clone https://github.com/EdCanzana12/Location-Back-End.git
cd geo-login-api

composer install

Create a copy of the .env file from the example:
cp .env.example .env

Then open the .env file and update the following lines to use SQLite:
DB_CONNECTION=sqlite
Create the file if it doesn't exist:
touch database/database.sqlite

