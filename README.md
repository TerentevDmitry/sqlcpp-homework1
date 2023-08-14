# Домашнее задание к занятию «Введение в БД. Типы БД»

### Задание 1
<details>
Спроектировать схему (таблицы и связи между ними) для музыкального сайта.

Требования:

- На сайте должна быть возможность увидеть список музыкальных жанров.
- Для каждого жанра можно получить список исполнителей, которые исполняют в соответствующем жанре.
- Для каждого исполнителя можно получить список его альбомов.
- Для каждого альбома можно получить список треков, которые в него входят.
- У жанра есть название.
- У исполнителя есть имя (псевдоним) и жанр, в котором он исполняет.
- У альбома есть название, год выпуска и его исполнитель.
- У трека есть название, длительность и альбом, которому этот трек принадлежит.

Результатом работы является изображение в формате PNG, содержащее схему БД.

Для создания схем можно воспользоваться удобной платформой [app.diagrams.net](https://app.diagrams.net/) или любым другим графическим редактором.

[Краткая инструкция](https://github.com/netology-code/sqlcpp-homeworks/blob/main/common/readme.md) по созданию схем БД на платформе [app.diagrams.net](https://app.diagrams.net/).
</details>

### Задание 2 (подготовка к следующей лекции)
<details>
  
Необходимо установить PostgreSQL на свой ПК.

<details>

<summary>Windows</summary>

[Видео-инструкция](https://embed.new.video/uyjUq9B3qYo6BbbkzG71Ny)

[Ссылка на PostgreSQL для Windows](https://www.enterprisedb.com/downloads/postgres-postgresql-downloads)

</details>

<details>

<summary>Linux (на примере Ubuntu 20.04)</summary>

[Видео-инструкция](https://embed.new.video/cRQW4Z2YnxZUxzKRLWwnPF)

Команды для установки:

```bash
# PostgreSQL
sudo apt update && sudo apt install postgresql-12

# pgAdmin4
wget --quiet -O - https://www.postgresql.org/media/keys/ACCC4CF8.asc | sudo apt-key add -
echo "deb http://apt.postgresql.org/pub/repos/apt/ `lsb_release -cs`-pgdg main" |sudo tee  /etc/apt/sources.list.d/pgdg.list
sudo apt update && sudo apt install pgadmin4
```

</details>

<details>

<summary>Mac OS X</summary>

[Видео-инструкция](https://kinescope.io/80f47a42-67a5-4e6e-9dbf-a4cc1ad1e799)

Команды для установки:

```bash
brew install postgres

postgres -V

pg_ctl -D /usr/local/var/postgres start

createuser -P -s postgres
```
  
</details>
</details>

### Задание 3 (подготовка к следующей лекции)
<details>
На следующей лекции мы будем использовать программу DBeaver Community для работы с СУБД. Это бесплатная программа, вы можете заранее скачать ее [по ссылке](https://dbeaver.io/download/) и установить на свой компьютер.

_Обратите внимание, что данное задание является рекомендацией, для полноценного участия в лекции DBeaver вам не потребуется, вы можете установить эту программу позже (или вообще использовать что-то другое)._
</details>
