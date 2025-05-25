# BlogPost Project

A modern blog platform built with **Laravel 11**, **Jetstream**, **Livewire**, **Vite**, and **Tailwind CSS**. This application supports user authentication, role-based dashboards (user/admin), and a simple post management system.

---

## Features

-   **User Authentication** (Laravel Jetstream, Sanctum)
-   **Role-based Dashboards**: Separate views for users and admins
-   **Admin Panel**:
    -   Add new blog posts (with image upload)
    -   View all posts
-   **User Panel**:
    -   View homepage and posts
-   **Responsive UI**: Built with Tailwind CSS and Blade templates
-   **API Ready**: Basic API route for authenticated user info

---

## Project Structure

-   `app/Http/Controllers/` – Main controllers (`HomeController`, `AdminController`)
-   `app/Models/` – Eloquent models (`Post`, `User`)
-   `resources/views/` – Blade templates for user and admin interfaces
-   `routes/web.php` – Web routes (homepage, dashboard, post management)
-   `routes/api.php` – API routes (user info)
-   `public/` – Public assets and uploaded images
-   `database/` – Migrations, factories, and seeders

---

## Getting Started

### Prerequisites

-   PHP >= 8.2
-   Composer
-   Node.js & npm

### Installation

1. **Clone the repository:**

    ```bash
    git clone <your-repo-url>
    cd blogpost
    ```

2. **Install PHP dependencies:**

    ```bash
    composer install
    ```

3. **Install Node dependencies:**

    ```bash
    npm install
    ```

4. **Copy and configure environment:**

    ```bash
    cp .env.example .env
    php artisan key:generate
    ```

5. **Run migrations:**

    ```bash
    php artisan migrate
    ```

6. **Build frontend assets:**

    ```bash
    npm run build
    ```

    For development, use:

    ```bash
    npm run dev
    ```

7. **Start the development server:**
    ```bash
    php artisan serve
    ```

---

## Usage

-   Visit `/` for the homepage.
-   Register/login to access user or admin dashboards.
-   Admins can add/view posts via `/post_page` and `/show_posts`.
-   Users see the homepage and available posts.

---

## Testing

-   Run tests with:
    ```bash
    php artisan test
    ```

---

## Tech Stack

-   **Backend:** Laravel 11, Jetstream, Livewire, Sanctum
-   **Frontend:** Blade, Tailwind CSS, Vite
-   **Database:** Eloquent ORM (default: SQLite/MySQL)
-   **Build Tools:** Vite, PostCSS

---

## License

This project is open-sourced under the [MIT license](https://opensource.org/licenses/MIT).

---

## Credits

-   Laravel (https://laravel.com)
-   Tailwind CSS (https://tailwindcss.com)
-   Vite (https://vitejs.dev)

