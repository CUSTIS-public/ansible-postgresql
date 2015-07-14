# Ansible PostgreSQL playbook

Этот playbook предназначен для установки PostgreSQL 9.4 на Centos 6x

Протестирован на Centos 6.6

## Основные шаги

* Подготовка хоста
* Установка PostgreSQL
* Установка Oracle Instant Client 11.2.0.4
* Установка Ora2Pg 

## Комментарии

## Требования

* Ansible 1.6 или выше
* Файлы дистрибутива Oracle Instant Client должны находится в /install папке хоста, с которого запускается ansible 
**  oracle-instantclient11.2-basic-11.2.0.4.0-1.x86_64.rpm
**  oracle-instantclient11.2-devel-11.2.0.4.0-1.x86_64.rpm
**  oracle-instantclient11.2-sqlplus-11.2.0.4.0-1.x86_64.rpm
**  oracle-instantclient11.2-jdbc-11.2.0.4.0-1.x86_64.rpm
* Файл дистрибутива Ora2Pg(ora2pg-15.2.tar.gz) должен находится в /install папке хоста, с которого запускается ansible

Поддерживаемые версии PostgreSQL:

* `9.4`

Поддерживаемые версии Oracle Client:

* `11.2.0.4`

Поддерживаемые версии Ora2Pg:

* `15.2`


## Запуск

```bash
ansible-playbook -i hosts setup.yml
```

## Лицензия

Этот playbook распространяется под лицензией:
[Apache 2.0 license](http://www.apache.org/licenses/LICENSE-2.0.html).
