1. Pertama, update package dengan perintah composer:

        composer update jeroennoten/laravel-adminlte

2. Kemudian, update  asset AdminLTE

        php artisan adminlte:update

3. Backup file view blade yang berada di `resources/views/vendor/adminlte`

4. Publish file view baru:

        php artisan adminlte:install --only=main_views --force

5. Backup file config `config/adminlte.php`

6. Publish file config baru

        php artisan adminlte:install --only=config
