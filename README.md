# notes

## MySql

### дамп  
base - название базы  
/tmp/dump.sql - путь до файла сохранения  
`mysqldump -v -h 127.0.0.1 -u root -p base > /tmp/dump.sql`
  
### восстановить из дампа
`mysql -u root -p base < /tmp/dump.sql`

## Certbot

### выпустить сертификат
`sudo apt install letsencrypt`
`sudo certbot certonly --standalone --agree-tos --preferred-challenges http -d domain-name.com`

## Docker

### список контейнеров
`docker container ls`

### выполнить команду в контейнере

`docker exec -it <container-name> bash`
