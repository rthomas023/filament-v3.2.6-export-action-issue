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
## License 

[MIT](https://choosealicense.com/licenses/mit/)
