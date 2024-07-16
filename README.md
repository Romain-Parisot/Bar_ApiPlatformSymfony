# Bar_ApiPlatformSymfony

This is a student project to learn about api using symfony. <br>
The Subject of this exercice is available here: https://docs.yoanncoualan.com/api-platform/evaluations/iim-A3-1

## Authors

This project was made by: 

- SIMON Adam
- PARISOT Romain

## Prerequisites

- PHP >= 8.1
- Composer 2.5
- Symfony CLI
- MySQL database

## Installation

1. Run this command to clone the repository:
   git clone https://github.com/Romain-Parisot/Bar_ApiPlatformSymfony.git

2. Run this command to navigate to the project directory:
   cd Bar_ApiPlatformSymfony

3. Run this command to install dependencies:
   composer install

4. Set up the environment variables in by creating an `.env.local` file, copy this command line into this file and edit it with your personal data:
```
   DATABASE_URL="mysql://UserOfYourLocalConfigForDatabaseConnection:PasswordOfYourLocalConfigForDatabaseConnectionIf YouHaveOne@127.0.0.1:3306/NameOfTheDatabase?serverVersion=8.0.32&charset=utf8mb4"
```
You will also need to add this into this file: 
```
APP_SECRET=6b35c4f44a1afa7454161ac3490f817b

###> lexik/jwt-authentication-bundle ###
JWT_SECRET_KEY=%kernel.project_dir%/config/jwt/private.pem
JWT_PUBLIC_KEY=%kernel.project_dir%/config/jwt/public.pem
JWT_PASSPHRASE=2fa26d2563f04b9e02e4bf5984b82fb77aa90a4ff21971b4a8c99846158df899
###< lexik/jwt-authentication-bundle ###
```

5. Run this command to create the database:
   `php bin/console doctrine:database:create`

## Running the Project

1. Start the Symfony development server:
   `symfony serve`

2. Access to the routes definition in your web browser at `http://localhost:8000/api`.

3. Import the postman collection from the repo to test the queries.
