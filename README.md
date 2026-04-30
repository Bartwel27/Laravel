<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework. You can also check out [Laravel Learn](https://laravel.com/learn), where you will be guided through building a modern Laravel application.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Redberry](https://redberry.international/laravel-development)**
- **[Active Logic](https://activelogic.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).




# Laravel Project Structure Explained

This project was built using **Laravel**, a modern PHP framework that follows the MVC (Model-View-Controller) architecture.

Laravel provides a clean and organized folder structure to help developers build scalable and maintainable applications.

---

## 📁 Root Directory Structure

```text
my-project/
├── app/
├── bootstrap/
├── config/
├── database/
├── public/
├── resources/
├── routes/
├── storage/
├── tests/
├── vendor/
├── .env
├── .env.example
├── .gitignore
├── artisan
├── composer.json
├── composer.lock
├── package.json
├── phpunit.xml
├── vite.config.js
└── README.md
```

---

## 📁 Main Folders

### app/

Contains the main application logic.

| Folder     | Description                       |
| ---------- | --------------------------------- |
| Console    | Custom Artisan commands           |
| Exceptions | Error handling                    |
| Http       | Controllers, Middleware, Requests |
| Models     | Eloquent models                   |
| Providers  | Service providers                 |

---

### bootstrap/

Used during application startup.

| File/Folder | Description                |
| ----------- | -------------------------- |
| app.php     | Bootstraps the application |
| cache/      | Optimized cache files      |

---

### config/

Contains all configuration files.

Examples:

* `app.php` → App name, timezone
* `database.php` → Database settings
* `mail.php` → Email configuration
* `services.php` → Third-party API keys

---

### database/

Handles database structure and sample data.

| Folder     | Description           |
| ---------- | --------------------- |
| migrations | Database tables       |
| seeders    | Sample/default data   |
| factories  | Fake data for testing |

---

### public/

Publicly accessible files.

| File        | Description         |
| ----------- | ------------------- |
| index.php   | Entry point of app  |
| favicon.ico | Website icon        |
| robots.txt  | Search engine rules |

---

### resources/

Frontend resources.

| Folder | Description      |
| ------ | ---------------- |
| views  | Blade templates  |
| css    | Stylesheets      |
| js     | JavaScript files |

---

### routes/

Application routes.

| File         | Description           |
| ------------ | --------------------- |
| web.php      | Website routes        |
| api.php      | API routes            |
| console.php  | Console commands      |
| channels.php | Broadcasting channels |

---

### storage/

Generated runtime files.

| Folder    | Description          |
| --------- | -------------------- |
| app       | Uploaded files       |
| framework | Sessions/cache/views |
| logs      | Application logs     |

---

### tests/

Used for automated testing.

| Folder  | Description        |
| ------- | ------------------ |
| Feature | Full feature tests |
| Unit    | Unit tests         |

---

### vendor/

Contains Composer dependencies.

> Auto-generated. Do not edit manually.

---

## 📄 Important Root Files

### .env

Stores environment variables.

```env
APP_NAME=Laravel
APP_ENV=local
DB_DATABASE=mydb
DB_USERNAME=root
```

---

### .env.example

Template file for `.env`

---

### artisan

Laravel command-line tool.

```bash
php artisan serve
php artisan migrate
php artisan make:controller UserController
```

---

### composer.json

PHP dependencies and project metadata.

---

### composer.lock

Locks installed package versions.

---

### package.json

Frontend dependencies for Node.js.

---

### phpunit.xml

Testing configuration.

---

### vite.config.js

Vite frontend build configuration.

---

### .gitignore

Files ignored by Git.

```text
/vendor
/node_modules
.env
```

---

## 📌 Laravel MVC Structure

Laravel follows MVC:

* **Model** → Handles data
* **View** → Handles UI
* **Controller** → Handles logic

---

## 📚 Summary

| Folder/File | Purpose             |
| ----------- | ------------------- |
| app         | Core backend logic  |
| routes      | URL routes          |
| resources   | Views and assets    |
| public      | Public files        |
| config      | App settings        |
| database    | Tables and seeders  |
| storage     | Logs/cache/uploads  |
| tests       | Automated tests     |
| vendor      | Dependencies        |
| .env        | Local configuration |

---

## 🚀 Best Practice

Keep your project organized:

* Business logic → `app/`
* Routes → `routes/web.php`
* Views → `resources/views`
* Database → `database/`
* Settings → `config/`

---

