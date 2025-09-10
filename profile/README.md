# Drop It!

### A Smart Pipe for Dropshipping Operations

Drop It! is a Laravel 12 multi-tenant SaaS application designed to act as a **smart pipe** between e-commerce stores, suppliers, and fulfillment providers. The core philosophy is to orchestrate complex data flows with **minimal data storage** and **comprehensive logging on failure**.

---

### Key Architectural Principles

-   **Decoupled Architecture**: Each part of the system is independent, allowing for easy scaling and maintenance.
-   **Idempotent Flows**: Every flow is unique and can be safely re-run without causing data duplication, ensuring data integrity.
-   **Automated Quality Control**: Our CI/CD pipeline runs automated checks for code styling (Laravel Pint), static analysis (PHPStan), and feature tests (PHPUnit) on every commit.

---

### Core Components

The application's logic is powered by a set of core components built with modern Laravel design patterns:

-   **Connectors**: Manages external service integrations (Shopify, AliExpress, etc.).
-   **Transformers**: Converts payloads from external services into a clean, canonical data model.
-   **Pipelines**: Executes business logic using the **Strategy Pattern** for clean, flexible data processing.
-   **Decorators**: Enhances API clients with stackable behaviors like logging, rate limiting, and retry mechanisms.

---

### Getting Started

To get the application up and running, follow these steps:

1.  Clone this repository:
    ```bash
    git clone [https://github.com/dropitnl/dropit.git](https://github.com/dropitnl/dropit.git)
    ```
2.  Install Composer dependencies:
    ```bash
    composer install
    ```
3.  Set up your environment file:
    ```bash
    cp .env.example .env
    php artisan key:generate
    ```
4.  Run database migrations:
    ```bash
    php artisan migrate
    ```
5.  Launch the development server:
    ```bash
    php artisan serve
    ```
    The application will now be running at `http://localhost:8000`.

---

### Contributions

We welcome contributions from the community. Before submitting a pull request, please ensure your code adheres to our quality standards by running the following commands:

-   Run PHPUnit tests: `php artisan test`
-   Apply code styling fixes: `vendor/bin/pint`
-   Run static analysis: `vendor/bin/phpstan`

For more detailed information on our development process, please refer to our contributing guidelines.
