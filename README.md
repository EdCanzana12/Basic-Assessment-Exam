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
APP_URL=http://localhost:8000
DB_CONNECTION=sqlite
Create the file if it doesn't exist:
touch database/database.sqlite

Generate application key:
php artisan key:generate

Install Sanctum (if not already installed):
composer require laravel/sanctum
Then publish the Sanctum config:
php artisan vendor:publish --provider="Laravel\Sanctum\SanctumServiceProvider"

Create and run a seeder:
php artisan make:seeder UserSeeder
```
### Start Local Server
```bash
# Run migrations
php artisan migrate

# Seed the database
php artisan db:seed

# Clear caches
php artisan config:clear
php artisan cache:clear
php artisan route:clear

php artisan serve
```
This will start the backend at http://localhost:8000

