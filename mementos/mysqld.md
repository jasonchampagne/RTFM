# MySQL Server

## Démarrer le serveur

|Windows|GNU/Linux et MacOS|
|:--|:--|
|`mysqld.exe --console`|`sudo systemctl start mysql`|

## Initialiser le répertoire data

|Windows|GNU/Linux et MacOS|
|:--|:--|
|`mysqld.exe --defaults-file=<path>/my.ini --initialize`|`usr/local/mysql/bin/mysqld --defaults-file=<path>/my.ini --initialize`|
