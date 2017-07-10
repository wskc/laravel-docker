# laravel-docker
Run Laravel Apps in seconds with this docker-compose configuration :rocket:

```bash
docker-compose up -d
```
  
Container names:
* laravel_web (nginx)
* laravel_php (php7)
* laravel_db (mariadb)

Edit `default.conf` (e.g. `server_name`) and `docker-compose.yml` (e.g. db environment) to your needs and include them in your (dev) projects root.

**NB: Be sure to use *db* as `DB_HOST` in your `.env`**

Default database config:
```yml
MYSQL_ROOT_PASSWORD: 'justice'
MYSQL_USER: 'laravel'
MYSQL_PASSWORD: 'laravel'
MYSQL_DATABASE: 'laravel'
```
