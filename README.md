# PHP Admin Dashboard

A simple PHP-based admin dashboard for managing products, orders, and users.

## Requirements

- PHP 7.4 or higher
- MySQL 5.7 or higher
- Apache web server
- PDO PHP Extension
- PDO MySQL PHP Extension

## Installation

1. Clone or download this repository to your web server's document root (e.g., `C:\xampp\htdocs\themeforest`).

2. Create the database and tables:
   - Open your web browser and go to http://localhost/phpmyadmin
   - Click on the "SQL" tab
   - Copy and paste the contents of the `config/schema.sql` file
   - Click "Go" to execute the SQL

3. Configure the database connection:
   - Open `config/database.php`
   - Update the database credentials if needed (default: username: "root", password: "")

4. Access the application:
   - Open your web browser and go to http://localhost/themeforest
   - Login with the default credentials:
     - Email: admin@example.com
     - Password: password

## Project Structure

```
themeforest/
├── config/                  # Configuration files
│   ├── database.php         # Database connection
│   └── schema.sql           # Database schema
├── public/                  # Public files (web root)
│   ├── admin/               # Admin pages
│   │   ├── index.php        # Admin dashboard
│   │   ├── products.php     # Products management
│   │   ├── orders.php       # Orders management
│   │   ├── users.php        # Users management
│   │   ├── profile.php      # User profile
│   │   └── settings.php     # Site settings
│   ├── assets/              # CSS, JS, and images
│   │   ├── css/             # CSS files
│   │   └── js/              # JavaScript files
│   ├── index.php            # Entry point
│   ├── login.php            # Login page
│   ├── dashboard.php        # User dashboard
│   ├── logout.php           # Logout script
│   ├── error.php            # Error page
│   └── bootstrap.php        # Application bootstrap
├── src/                     # Application source code
│   ├── controllers/         # Controllers
│   ├── models/              # Models
│   └── views/               # Views
└── README.md                # This file
```

# Project Update SOON

## Troubleshooting

If you encounter any issues:

1. Make sure your web server (Apache) and MySQL server are running.
2. Check that the PDO and PDO MySQL extensions are enabled in your PHP configuration.
3. Verify that the database credentials in `config/database.php` are correct.
4. Check the PHP error logs for any error messages.

## License

This project is licensed under the MIT License - see the LICENSE file for details. 
