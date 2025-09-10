# Drop It!

Welcome to the official GitHub organization for **Drop It!**, a suite of repositories dedicated to building a robust, multi-tenant dropshipping integration platform.

This organization is home to the core application and all of its shared, foundational components.

### Core Repositories

-   **[dropit](https://github.com/dropitnl/dropit)**: The heart of the operation. This repository houses the main Laravel application that acts as a **smart pipe** between e-commerce stores, suppliers, and fulfillment providers.
-   **[.github](https://github.com/dropitnl/.github)**: This repository serves as the central hub for our organization's community health files, including this profile, and all shared GitHub Actions workflows. It ensures consistency and quality across all of our projects.

### Architectural Philosophy

The Drop It! platform is built on a foundation of clean code and modern design patterns to handle the complexities of dropshipping at scale. Our architecture is designed to be **decoupled**, **resilient**, and **idempotent**, with a focus on:

-   **"Smart Pipe" Logic**: We only store data when flows fail, allowing for high-performance, real-time data orchestration.
-   **Automated Quality Control**: Every pull request is automatically verified with our shared CI workflows, which run **Laravel Pint** for code styling, **PHPStan** for static analysis, and **PHPUnit** for testing.

---

### Get Started

To learn more about the project and contribute, please visit the **[dropit](https://github.com/dropitnl/dropit)** repository.
