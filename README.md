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

Наоплни .env своими данными(их подхватят и strapi и postgresql)
```
cd ..
nano .env
```
Запусти контейнер
```
docker-compose up -d
```
