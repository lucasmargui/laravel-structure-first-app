<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">🚀 Development of a first structure for future references</p>

## Resources Used
Laravel


# Database and Environment variables

In Laravel, environment variables are usually stored in a file called .env, located in the root of the project. To access these variables within the Laravel application, you can use the env() function.

![image](https://github.com/user-attachments/assets/668f75ec-7cf7-4f56-bc4d-e8cb55a40732)



## Connection to Database in Laravel

Database configuration is done in the config/database.php file. This file uses environment variables to define connection details.

![image](https://github.com/user-attachments/assets/e64e1137-b23d-46b6-8b39-1a1b096e5baa)



## Accessing the Database
Laravel uses Eloquent ORM and Query Builder to interact with the database.

![image](https://github.com/user-attachments/assets/0b96df75-9abc-4cac-991c-dcd21943f8c5)


## Migrations

Migrations allow you to define the structure of the database through migration files.


### Creating a migration:

```
php artisan make:migration create_users_table
```

### Running migrations:

```
php artisan migrate
```

## Seeds
Seeders allow you to populate the database with initial data.

### Creating a seeder:

```
php artisan make:seeder UsersTableSeeder
```

### Running seeders:

```
php artisan db:seed --class=UsersTableSeeder
```


# Directory structure  

![image](https://github.com/user-attachments/assets/441d0651-cd8b-4195-89aa-5b45c201088c)


### The Root Directory: 
Main directory of the project. 

### The App Directory: 
Contains the application's core code. 

### The Bootstrap Directory: 
Contains the app.php file that initializes the framework and a cache directory for performance optimization. 

### The Config Directory: 
Contains the application configuration files. 

### The Database Directory: 
Contains the migrations, model factories, and database seeds, and can store an SQLite database. 

### The Public Directory: 
Contains the index.php file, entry point for all requests, and assets such as images, JavaScript and CSS. 

### The Resources Directory: 
Contains views and uncompiled assets, such as CSS and JavaScript. 

### The Routes Directory: 
Contains the application's route definitions, including the web.php and console.php files by default. 

### The Storage Directory: 
Contains logs, compiled Blade templates, file-based sessions, caches and other files generated by the framework, segregated into app, framework and logs directories. 

### The Storage/App/Public Directory: 
Stores user-generated files, such as profile avatars, which must be publicly accessible; a symbolic link in public/storage should point to this directory, created with the php crafts storage command 

### The Tests Directory: 
Contains automated tests, including unit and functionality tests with Pest or PHPUnit; Tests can be run using the /vendor/bin/pest, /vendor/bin/phpunit or php crafts test commands. 

### The Vendor Directory: 
Contains the dependencies managed by Composer.

# The App Directory 

The app directory houses the majority of the application and is autoloaded by Composer using the PSR-4 standard.

### Http, Models, and Providers:
Contains the Http, Models, and Providers directories by default, and other directories are generated as Artisan commands are used.

### Console and Http:
The Console and Http directories provide APIs for the application, being interfaces to interact via the HTTP and CLI protocol, respectively.

### Artisan Commands:
Many classes can be generated via Artisan commands; use php artisan list make to review available commands.

### Broadcasting Directory:
Contains broadcast channel classes, created using the make:channel command.

### Console Directory:
It houses custom Artisan commands, generated by the make:command command.

### Event Directory:
Contains event classes, created by the event:generate and make:event commands.

### Exceptions Directory:
Contains custom exceptions, generated by the make:exception command.

### Http Directory:
Contains controllers, middleware and form requests, dealing with request logic.

### Job Directory:
It houses queuable jobs, created by the make:job command.

### Listeners Directory:
Contains classes that handle events, generated by the event:generate and make:listener commands.

### Mail Directory:
Contains email classes, created by the make:mail command.

### Model Directory:
Contains Eloquent model classes for interacting with the database.

### Notifications Directory:
Contains transactional notifications, created by the make:notification command.

### Policies Directory:
Contains authorization policy classes, created by the make:policy command.

### Providers Directory:
Contains service providers that initialize the application.

### Rules Directory:
Contains custom validation rule objects created by the make:rule command.
