docker run --name wordpress -d -v /Users/alexcpl/code/wordpress/wp-content:/var/www/html/wp-content -p 80:80 --link mariadb:mysql wordpress:php7.2-apache
docker run --name mariadb -e MYSQL_ROOT_PASSWORD=password -d -v /Users/alexcpl/code/wordpress/database:/var/lib/mysql -p 3306:3306 mariadb:latest
