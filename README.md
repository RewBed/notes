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
`sudo certbot certonly --webroot -w /var/docker/okocrm-test/app/okocrm/web -d test.arkadiikur.ru`

## Docker

### список контейнеров
`docker container ls`

### выполнить команду в контейнере

`docker exec -it <container-name> bash`
