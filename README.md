# Drupal 8 Nginx Dockerfile

## Build image

    docker build -t drupal8/nginx .

## Usage

    docker run /
        -d /
        -p 8080:80 /
        -v <CONF_DIR>:/etc/nginx/conf.d /
        -v <LOGS_DIR>:/var/log/nginx /
        -v <APP_DIR>:/var/www/html /
        drupal8/nginx
