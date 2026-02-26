<div align="center">

  <img src="https://laravel.com/img/logomark.min.svg" alt="Logo" width="100" height="100">

  <h1 align="center">Laravel Starter Template</h1>

  <p align="center">
    <strong>A professional-grade boilerplate to jumpstart your Laravel projects with modern best practices.</strong>
    <br />
    <a href="https://github.com/maskintelligence-gif/Laravel-starter-template"><strong>Explore the docs »</strong></a>
    <br />
    <br />
   <a
    ·
    <a href="https://github.com/maskintelligence-gif/Laravel-starter-template/issues">Report Bug</a>
    ·
    <a href="https://github.com/maskintelligence-gif/Laravel-starter-template/issues">Request Feature</a>
  </p>

  <p align="center">
    <img src="https://img.shields.io/github/license/maskintelligence-gif/Laravel-starter-template?style=for-the-badge" alt="License">
    <img src="https://img.shields.io/github/issues/maskintelligence-gif/Laravel-starter-template?style=for-the-badge" alt="Issues">
    <img src="https://img.shields.io/github/issues-pr/maskintelligence-gif/Laravel-starter-template?style=for-the-badge" alt="Pull Requests">
    <img src="https://img.shields.io/github/last-commit/maskintelligence-gif/Laravel-starter-template?style=for-the-badge" alt="Last Commit">
    <img src="https://img.shields.io/badge/PHP-8.2%2B-777BB4?style=for-the-badge&logo=php" alt="PHP Version">
    <img src="https://img.shields.io/badge/Laravel-11.x-FF2D20?style=for-the-badge&logo=laravel" alt="Laravel Version">
  </p>
</div>

---

## 📖 About The Project

Building a modern web application from scratch often involves hours of repetitive configuration—setting up authentication, configuring asset bundlers, establishing a testing environment, and defining a scalable architecture. 

The **Laravel Starter Template** is a highly curated boilerplate designed by architects to eliminate "boilerplate fatigue." It provides a robust, production-ready foundation that follows Laravel's latest standards and industry-best practices. Whether you are building a SaaS, a corporate dashboard, or a complex API, this template ensures your project starts with a clean, maintainable, and scalable codebase.

### Why use this template?
*   **Speed to Market**: Skip the first 10 hours of project setup.
*   **Consistency**: Enforces a clean directory structure and coding standards across teams.
*   **Performance**: Pre-optimized Vite and Tailwind CSS configuration for lightning-fast frontend delivery.
*   **Reliability**: Includes a pre-configured CI/CD pipeline via GitHub Actions to ensure code quality.

### Built With

*   ![PHP](https://img.shields.io/badge/php-%23777BB4.svg?style=flat-square&logo=php&logoColor=white) **PHP 8.2+**
*   ![Laravel](https://img.shields.io/badge/laravel-%23FF2D20.svg?style=flat-square&logo=laravel&logoColor=white) **Laravel 11.x**
*   ![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=flat-square&logo=vite&logoColor=white) **Vite**
*   ![TailwindCSS](https://img.shields.io/badge/tailwindcss-%2338B2AC.svg?style=flat-square&logo=tailwind-css&logoColor=white) **Tailwind CSS**
*   ![MySQL](https://img.shields.io/badge/mysql-%2300f.svg?style=flat-square&logo=mysql&logoColor=white) **MySQL**
*   ![GitHub Actions](https://img.shields.io/badge/github%20actions-%232671E5.svg?style=flat-square&logo=githubactions&logoColor=white) **GitHub Actions**

---

## ✨ Key Features

### 🔐 Authentication Ready
Comes with a secure authentication scaffolding. Includes Login, Registration, Password Reset, and Email Verification out of the box, utilizing Laravel's native features for maximum security.

### 🎨 Modern Frontend Stack
Integrated with **Vite** for ultra-fast Hot Module Replacement (HMR) and **Tailwind CSS** for rapid UI development. The template includes a basic layout structure with responsive design patterns.

### 🏗️ Clean Architecture
Follows the "Fat Models, Skinny Controllers" philosophy while providing placeholders for Service Layers and Action classes to keep your business logic decoupled and testable.

### 🧪 Comprehensive Testing Suite
Pre-configured with **Pest** (or PHPUnit) to encourage Test-Driven Development (TDD). Includes example Unit and Feature tests to serve as a reference for your own test cases.

### 🤖 CI/CD Integration
A pre-defined `.github/workflows/main.yml` file is included. Every push or pull request automatically triggers:
*   Linting and Code Style checks.
*   Static Analysis.
*   Automated Test Execution.

### 🗄️ Optimized Database Config
Standardized migrations and factory patterns. Pre-configured for MySQL but easily adaptable to PostgreSQL or SQLite for local development.

---

## 📂 Project Structure

A high-level overview of the organized directory structure:

```text
laravel-starter-template/
├── app/
│   ├── Actions/            # Logic classes for single-responsibility tasks
│   ├── Http/
│   │   ├── Controllers/    # Slim controllers
│   │   └── Middleware/     # Custom request filters
│   ├── Models/             # Eloquent models with strict typing
│   └── Providers/          # Service providers for package integration
├── bootstrap/              # App initialization scripts
├── config/                 # Centralized configuration files
├── database/
│   ├── factories/          # Model factories for testing
│   ├── migrations/         # Database schema definitions
│   └── seeders/            # Initial data population
├── public/                 # Entry point for the web server
├── resources/
│   ├── css/                # Tailwind & custom styles
│   ├── js/                 # JavaScript/Vue/React components
│   └── views/              # Blade templates
├── routes/                 # Web, API, and Console route definitions
├── tests/
│   ├── Feature/            # Integration & HTTP tests
│   └── Unit/               # Isolated logic tests
├── .github/                # GitHub Actions workflows
├── vite.config.js          # Vite asset bundling configuration
└── tailwind.config.js      # Tailwind CSS theme customization
```

---

## 🚀 Getting Started

Follow these steps to get your local development environment up and running.

### Prerequisites

*   **PHP**: `^8.2`
*   **Composer**: `^2.0`
*   **Node.js**: `^18.x` & **NPM**
*   **Database**: MySQL, PostgreSQL, or SQLite

### Installation

1.  **Clone the repository**
    ```bash
    git clone https://github.com/maskintelligence-gif/Laravel-starter-template.git
    cd Laravel-starter-template
    ```

2.  **Install PHP dependencies**
    ```bash
    composer install
    ```

3.  **Install Frontend dependencies**
    ```bash
    npm install
    ```

4.  **Environment Setup**
    Copy the example environment file and configure your database.
    ```bash
    cp .env.example .env
    ```

5.  **Generate Application Key**
    ```bash
    php artisan key:generate
    ```

6.  **Run Migrations & Seeders**
    ```bash
    php artisan migrate --seed
    ```

7.  **Compile Assets**
    ```bash
    npm run dev
    ```

8.  **Start the Server**
    ```bash
    php artisan serve
    ```

### Environment Variables

| Variable | Description | Default |
| :--- | :--- | :--- |
| `APP_ENV` | Application environment | `local` |
| `APP_DEBUG` | Enable/Disable debug mode | `true` |
| `DB_CONNECTION` | Database driver | `mysql` |
| `DB_DATABASE` | Name of the database | `laravel` |
| `VITE_APP_NAME` | App name for frontend | `${APP_NAME}` |

---

## 🛠️ Usage Examples

### Creating a New Action
Instead of bloating controllers, use Actions:
```php
namespace App\Actions;

use App\Models\User;

class CreateUserAction {
    public function execute(array $data): User {
        // Logic for user creation...
        return User::create($data);
    }
}
```

### Running Tests
Ensure everything is working correctly:
```bash
# Run tests using Pest
php artisan test

# Run tests with coverage (requires Xdebug)
php artisan test --coverage
```

### Compiling for Production
When you are ready to deploy:
```bash
npm run build
```

---

## 🗺️ Roadmap

- [ ] **Docker Integration**: Add `docker-compose.yml` with Laravel Sail support.
- [ ] **API Scaffolding**: Add Sanctum/Passport pre-configuration for mobile app support.
- [ ] **Admin Dashboard**: Optional integration with Filament or Nova.
- [ ] **Socialite Integration**: Pre-configure OAuth for Google and GitHub.
- [ ] **Multilingual Support**: Setup i18n for Blade and JS.

---

## 🤝 Contributing

Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📄 License

Distributed under the MIT License. See `LICENSE` for more information.

---

## 📞 Contact

**Mask Intelligence**  
Email: maskintell1@gmail.com  
Tel: +256 791715573  

Project Link: [https://github.com/maskintelligence-gif/Laravel-starter-template](https://github.com/maskintelligence-gif/Laravel-starter-template)

---

## 💖 Acknowledgments

*   [Laravel Documentation](https://laravel.com/docs)
*   [Tailwind CSS Components](https://tailwindcss.com/components)
*   [Laravel News](https://laravel-news.com)
*   [Spatie's Open Source Packages](https://spatie.be/open-source)

---
<p align="center">Made with ❤️ for the Laravel Community</p>
