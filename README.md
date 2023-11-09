Login Page UI: https://github.com/junxian428/HackerLoginPage_UI

php artisan make:controller AuthController


php artisan make:model User

CREATE TABLE users (
    id INT PRIMARY KEY,
    username VARCHAR(255) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL
);

INSERT INTO users (username, password) VALUES ('admin', 'admin');

$username = $request->input('username');
$password = $request->input('password');

$user = User::where('username', '=', $username)->first();

In this code, the values of $username and $password are not directly injected into the SQL query. Instead, they are treated as parameters and will be automatically escaped and sanitized by Laravel.

By using Eloquent's query builder methods, you are already safeguarding against SQL injection. Laravel handles the parameter binding for you, making it secure by default.

However, if you ever need to execute raw SQL queries in Laravel, you should use parameter binding provided by the query builder or use bindings:


php artisan make:controller DashboardController

https://freefrontend.com/css-dashboards/#google_vignette


https://codepen.io/TheMOZZARELLA/pen/BawVrYr

https://codepen.io/adnanov/pen/QKjMgb


 To run:

 php artisan serve

 go to http://localhost:8000

Client: http://localhost:8000

Admin : http://localhost:8000/superuser


php artisan make:controller ClientDashboardController


For pagination :

php artisan vendor:publish --tag=laravel-pagination


php artisan make:controller PLCController

php artisan make:controller HMIController

php artisan make:controller IPCController

php artisan make:controller ECController

PS C:\Users\USer\Desktop1\MMU\V2> php artisan make:controller HydraulicController

PS C:\Users\USer\Desktop1\MMU\V2> php artisan make:controller PneumaticsController