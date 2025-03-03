# Laravel Job Management System

This project allows users to manage job listings, perform CRUD operations, and filter jobs based on specific criteria. The project also includes authentication functionality for secure access.

## Features

- **Authentication:** User registration, login, and password management.
- **Job CRUD Operations:** Create, Read, Update, and Delete job listings.
- **Job Filtering:** Filter job listings based on various criteria such as job title, location, and job type.
- **User Roles:** Different user roles for managing jobs and viewing listings.

## Prerequisites

Before running this project, make sure you have the following installed:

- **PHP** (version 8.0 or higher)
- **Laravel** (version 9.x or higher)
- **Composer** (for managing PHP dependencies)
- **MySQL** or another compatible database server

### Database Setup
This app uses MySQL. To use something different, open up config/Database.php and change the default driver.

To use MySQL, make sure you install it, setup a database and then add your db credentials(database, username and password) to the .env.example file and rename it to .env

### Migrations
To create all the nessesary tables and columns, run the following
```
php artisan migrate
```

### Seeding The Database
To add the dummy listings with a single user, run the following
```
php artisan db:seed
```

### File Uploading
When uploading listing files, they go to "storage/app/public". Create a symlink with the following command to make them publicly accessible.
```
php artisan storage:link
```

### Running The App
Upload the files to your document root, Valet folder or run 
```
php artisan serve
```

## License

The LaraGigs app is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).
