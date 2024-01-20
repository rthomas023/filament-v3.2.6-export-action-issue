# Filament v3.2.6 Export Action issue
This repository is a clean install of Laravel 10 and Filament v3.2.6 that was created to present an issue with the Export Action when using **redis** as the **QUEUE_CONNECTION** driver instead of the **sync** driver.

## Installation

```bash
git clone git@github.com:rthomas023/filament-v3.2.6-export-action-issue.git
cd filament-v3.2.6-export-action-issue
composer install
cp .env.example .env
php artisan key:generate
php artisan migrate
php artisan serve
```
## Filament Login Credentials
Email: admin@admin.com
Password: password

## Note
After you copy the `env.example` to `.env`, remember to update:
`QUEUE_CONNECTION=sync` to `QUEUE_CONNECTION=redis`
`REDIS_HOST=127.0.0.1`

Assuming you have Redis running and if on a different, you'll need to update that.

## License 

[MIT](https://choosealicense.com/licenses/mit/)
