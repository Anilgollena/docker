version: '3.3'

services:
  db:
    image: mysql:8.0.19
    command: '--default-authentication-plugin=mysql_native_password'
    volumes:
      - db_data:/var/lib/mysql
    restart: always
    environment:
      - MYSQL_ROOT_PASSWORD=Anil1234
      - MYSQL_DATABASE=mydb
      - MYSQL_USER=Anil
      - MYSQL_PASSWORD=Anil123

  wordpress:
    image: wordpress:latest
    ports:
      - "80:80"
    restart: always
    environment:
      - WORDPRESS_DB_HOST=db
      - WORDPRESS_DB_USER=anil
      - WORDPRESS_DB_PASSWORD=Anil123
      - WORDPRESS_DB_NAME=gollena

volumes:
  db_data:
