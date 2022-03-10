# MySQL 5.7 & php my admin & Mongodb

## Run:

`docker-compose up -d`

## Services
- ### mysql:
```
'db' => [
    'class' => 'yii\db\Connection',
    'dsn' => 'mysql:host=0.0.0.0;port=3307;dbname=syarah',
    'username' => 'root',
    'password' => 'root',
    'charset' => 'utf8',
    'attributes' => [PDO::ATTR_CASE => PDO::CASE_LOWER],
],
```
- ### mongodb:
```
'mongodb' => [
    'class' => '\yii\mongodb\Connection',
    'dsn' => 'mongodb://0.0.0.0:27018/yii2logs',
    'options' => [
        'username' => 'root',
        'password' => 'root',
    ]
],
```
- ### php myadmin
  - Visit http://localhost:8080

## To stop all services:

`docker-compose down`