# Authentication Service

REST API for user authentication built with Laravel 13 using Laravel Sanctum.

## Features

- User registration
- User authentication (login)
- User logout
- Bearer Token authentication
- Protected API endpoints

## Technologies

- PHP 8.x
- Laravel 13
- Laravel Sanctum
- SQLite

## API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | /api/register | Register a new user |
| POST | /api/login | Authenticate user |
| POST | /api/logout | Logout and revoke current token |
| GET | /api/user | Get authenticated user |

## Installation

```bash
composer install
php artisan migrate
php artisan serve
```

Server:

```
http://127.0.0.1:8000
```

Authentication:

```
Authorization: Bearer <token>
```

## Implemented security

- Password hashing
- Token-based authentication (Laravel Sanctum)
- Protected routes
- Token revocation on logout