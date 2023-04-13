# MySQL Server

|ACTION|WINDOWS|GNU/Linux & MacOS|
|--:|:--|:--|
|Démarrer le serveur|`mysqld.exe --console`|`sudo systemctl start mysql`|
|Initialiser le répertoire data|`mysqld.exe --defaults-file=<path>/my.ini --initialize`|`usr/local/mysql/bin/mysqld --defaults-file=<path>/my.ini --initialize`|
