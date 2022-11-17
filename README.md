## :gear: QUICK INSTALL:

### Requirements:

- Git.
- Composer.
- PHP >= 8.0
- MySQL/MariaDB.
- Redis (Optional).
- or Docker.


**Commands:**

```bash
# Start the API (this is my alias for: docker-compose up -d --build).
$ make up

# To create the database and import test data from scratch.
$ make db

# Checkout the API.
$ curl http://localhost:8081

# Stop and remove containers (it's like: docker-compose down).
$ make down
```

### :video_camera: VIDEO #3

[Using Redis Cache.](https://youtu.be/qX_TVjxEZSc)

### :movie_camera: VIDEO #4

[Deploy Slim PHP on Heroku.](https://youtu.be/-F09LCgNuGg)


## :traffic_light: TESTING:

Run all PHPUnit tests with `composer test`.

```bash
$ composer test
> phpunit
PHPUnit 9.5.10 by Sebastian Bergmann and contributors.


### ENDPOINTS:

#### INFO:

- Help: `GET /`

- Status: `GET /status`


#### USERS:

- Login User: `POST /login`

- Create User: `POST /api/v1/users`

- Update User: `PUT /api/v1/users/{id}`

- Delete User: `DELETE /api/v1/users/{id}`
