# Laravel 12 Starter Kit

This repository serves as a lightweight starting point for professional Laravel projects. It combines best practices without bloating the core – enabling you to become productive quickly without needing to strip things out later.

## Included Packages

**Backend**

- [Laravel 12](https://laravel.com) – latest framework version with PHP 8.2
- [Laravel Sanctum](https://laravel.com/docs/sanctum) – token authentication for SPAs and APIs
- [Livewire 3](https://livewire.laravel.com/) – modern components with minimal JavaScript
- [Spatie Media Library](https://spatie.be/docs/laravel-medialibrary) – file-based media management
- [Spatie Permission](https://spatie.be/docs/laravel-permission) – roles and permissions
- [Laravel Telescope](https://laravel.com/docs/telescope) – debugging dashboard
- [Laravel Tinker](https://laravel.com/docs/tinker) – interactive shell

**Developer Tools**

- [Laravel Sail](https://laravel.com/docs/sail) – Docker-based local development environment
- [Laravel Pint](https://laravel.com/docs/pint) – code formatting
- [Laravel Pail](https://github.com/laravel/pail) & [Debugbar](https://github.com/barryvdh/laravel-debugbar) – logging & debugging
- [Pest](https://pestphp.com) – testing framework

**Frontend**

- [Vite](https://vitejs.dev) & [Laravel Vite Plugin](https://laravel.com/docs/vite)
- [Tailwind CSS 4](https://tailwindcss.com)
- [Axios](https://axios-http.com) for HTTP requests

## Requirements

- PHP >= 8.2
- Composer
- Node.js & npm
- Database (MySQL by default; tests use in-memory SQLite)

## Installation & Setup

1. Clone the repository
   ```bash
   git clone https://github.com/dnz1801/laravel-12-starter-kit
   cd laravel-12-starter-kit
   ```

2. Create environment file
   ```bash
   cp .env.example .env
   # Adjust database and other values
   ```

3. Install dependencies
   ```bash
   composer install
   npm install
   ```

4. Generate app key & run migrations
   ```bash
   php artisan key:generate
   php artisan migrate
   ```

5. Start development server – runs PHP server, queue listener, and Vite
   ```bash
   composer dev
   ```

   Alternatively, start each service separately:
   ```bash
   php artisan serve
   php artisan queue:listen
   npm run dev
   ```

## Running Tests

```bash
composer test
```

## Production Build

Compile assets for production:

```bash
npm run build
```
## Contributing

To contribute, please ensure code style consistency and verify tests pass:

```bash
./vendor/bin/pint
composer test
```

## License

The Starter Kit is released under the MIT License.
