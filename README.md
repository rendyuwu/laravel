### How to use

#### Create a Dockerfile & insert this configuration

```
FROM rendyuwu/laravel:latest

# Copy code to /var/www
COPY --chown=www:www-data . /var/www

# add root to www group
RUN chmod -R ug+w /var/www/storage
```
