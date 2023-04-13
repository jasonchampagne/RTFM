# MySQL Server

## Démarrer le serveur

|WINDOWS|GNU/LINUX ou MACOS|
|:--|:--|
|`mysqld --console`|`sudo systemctl start mysql`|

## Initialiser le répertoire data

|WINDOWS|GNU/LINUX ou MACOS|
|:--|:--|
|`mysqld --defaults-file=<path>/my.ini --initialize`|`usr/local/mysql/bin/mysqld --defaults-file=<path>/my.ini --initialize`|
