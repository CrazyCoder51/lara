# info0303-projet

## Récupération du dépôt

```
git clone https://gitlab-mi.univ-reims.fr/mali0020/info0303-projet
cd info0303-projet
composer install
cp .env.example .env
php artisan key:generate
php artisan storage:link
php artisan migrate:fresh --seed
npm install
npm run build
php artisan db:seed --class=NewsSeeder
php artisan db:seed --class=TeamsSeeder
php artisan db:seed --class=UsersSeeder
php artisan db:seed --class=EventSeeder
php artisan db:seed --class=RoundSeeder
php artisan db:seed --class=ResultSeeder

```

Remplacez `cp` par `copy` si vous êtes sous *Windows*.