# Invoice Generator 

## Overview

This web application allows users to easily generate customized invoices for their customers. Built with **Laravel** as the backend and **Filament** for the frontend, this application provides a seamless, user-friendly interface for creating and managing invoices.

### Features:
- **User Authentication**: Secure login and registration for users.
- **Invoice Creation**: Generate invoices with custom details such as customer information, products/services, pricing, and discounts.
- **Customizable Templates**: Create invoices using predefined templates, with options to customize colors, logos, and styles.
- **Invoice Management**: View, edit, and delete previously created invoices.
- **PDF Generation**: Download invoices in PDF format for easy sharing and printing.
- **Responsive Design**: Fully responsive and optimized for both desktop and mobile devices.

## Prerequisites

Before you start, ensure you have the following installed:
- PHP >= 8.0
- Composer
- Laravel 8 or higher
- MySQL (or any supported database)
- Node.js (for frontend assets)
- Filament Admin Panel

## Installation

### 1. Clone the repository:

```bash
git clone https://github.com/Ms-Ngari/invoice-generator.git
```

### 2. Navigate into the project directory:

```bash
cd invoice-generator
```

### 3. Install dependencies:

Install PHP dependencies using Composer:

```bash
composer install
```

Install Node.js dependencies for frontend assets:

```bash
npm install
```

### 4. Configure environment variables:

Rename `.env.example` to `.env`:

```bash
cp .env.example .env
```

Set up your database and other application configuration in the `.env` file. Make sure to define the correct database connection, APP_KEY, and any other relevant values.

### 5. Generate application key:

```bash
php artisan key:generate
```

### 6. Run database migrations:

```bash
php artisan migrate
```

### 7. Build assets:

```bash
npm run dev
```

This will compile the frontend assets.

### 8. Serve the application:

```bash
php artisan serve
```

The application should now be running at `http://127.0.0.1:8000`.

## Usage

### 1. Authentication:

- You can register a new account or log in with an existing one.

### 2. Invoice Creation:

- After logging in, navigate to the "Invoices" section from the Filament admin dashboard.
- Click on the "Create New Invoice" button.
- Fill in customer details, products/services, and any other necessary information.
- Customize the invoice appearance as needed.
- Click "Generate Invoice" to create the invoice.

### 3. Download or Print:

Once an invoice is generated, you can download it as a **PDF** or print it directly from the application.

### 4. Invoice Management:

- View a list of your previously generated invoices.
- Edit or delete invoices as needed.

## File Structure

```
.
├── app/
│   ├── Models/
│   ├── Http/
│   ├── ...
├── resources/
│   ├── views/
│   ├── js/
│   └── ...
├── routes/
│   ├── web.php
│   └── api.php
├── storage/
│   └── ...
├── database/
│   ├── migrations/
│   └── seeders/
├── public/
│   ├── css/
│   └── js/
└── ...
```

## Dependencies

- **Laravel**: Web application framework used for backend logic and routing.
- **Filament**: Admin panel and interface for managing invoices, built using Filament.
- **Tailwind CSS**: For styling the frontend.

## Contributing

1. Fork the repository.
2. Create a new branch (`git checkout -b feature-branch`).
3. Make your changes and commit them (`git commit -am 'Add new feature'`).
4. Push to your branch (`git push origin feature-branch`).
5. Create a new pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.