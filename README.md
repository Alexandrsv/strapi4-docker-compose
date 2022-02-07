# strapi4 + postgresql + docker-compose

Пример любительского развертывания strapi4 с postgresql при помощи docker-compose

## Что с этим делать:

**Если проект с нуля**

Склонируй репозиторй в подготовленную папку
```
git clone https://github.com/Alexandrsv/strapi4-docker-compose.git .
```
Создай 2 папки - для strapi и данных postgres
```
mkdir ./pg_data ./strapi
```
Установить strapi 
```
cd ./strapi
npx create-strapi-app@latest .
```
![This is an image](https://i.imgur.com/A1Ahx8T.png)

Наоплни .env своими данными по примеру .env.example Strapi и postgresql подхватят данные из переменных. 
```
cd ..
nano .env
```
Запусти контейнер
```
docker-compose up -d


```
**Для существующего проекта**

Все как и для нового, только вместо установки strapi нужно склонировать существующий проект в папку strapi и подправить .env в корне
