# laravel-tagsearch-sample
Laravel using tag (like Qiita, Wantedly visit)

# Install

```
docker-compose build
docker-compose run --rm nodejs npm install
docker-compose run --rm web composer install
docker-compose run --rm web php artisan key:generate
docker-compose run --rm web php artisan migrate
```

# Run server

```
docker-compose up -d
```

go to http://localhost:8000
