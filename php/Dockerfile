FROM php:7.4-fpm

# Instalacja dodatkowych zależności
RUN apt-get update && apt-get install -y 
    # Dodaj tutaj swoje zależności, jeśli są potrzebne

# Konfiguracja PHP-FPM
COPY ./php-fpm/www.conf /usr/local/etc/php/php-fpm.d/www.conf

WORKDIR /var/www/html

EXPOSE 9000

CMD ["php-fpm"]


