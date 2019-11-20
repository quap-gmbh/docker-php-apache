# PHP Docker Container with Apache Webserver

Using PHP.earth docker images: https://docs.php.earth/

Works with PHP Version 7.3

## Build
`docker build -t mstoelzle/docker-php-apache -f Dockerfile .`

## Run:
`docker run -it --rm  -p 8080:80 -v /path_to_repo:/var/www/localhost/htdocs mstoelzle/docker-php-apache`

or run directly in application folder:

`docker run -it --rm  -p 8080:80 -v `pwd`/:/var/www/localhost/htdocs mstoelzle/docker-php-apache`