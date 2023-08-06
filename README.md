# taski-docker

## О проекте

Приложение позволяющее добавлять, удалять и редактировать задачи.

## Содержание проекта

-  CI-CD workflow,
- docker-compose.production.yml &nbsp;&nbsp;&nbsp; docker с загрузкой образов из docker.hub
- docker-compose.yml
  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  docker с локальным build образов
- backend
- frontend

<br/>
<br/>


<details close>
<summary><h2 style="display: inline">Запуск проекта локально <h3 style="display: inline">▶️</h3></h2></summary>

Для запуска проекта необходимо иметь на установленные: node.js, python, pip.

### клонировать проект:

```
git clone git@github.com:MiOlga36/taski-docker.git
```

### frontend:

```shell
cd frontend
npm i
rpm run dev
```

### backend:

```shell
cd backend
python3 -m venv venv

# windows:
  source venv/scripts/activate

pip install -r requirements.txt
python manage.py migrate
python manage.py runserver
```


</details>




<br/>


<details close>
<summary><h2 style="display: inline">Техническое задание <h3 style="display: inline">▶️</h3></h2></summary>

Настроить запуск проекта taski-docker в контейнерах и CI/CD с помощью GitHub Actions

## Чек-лист для проверки перед отправкой задания

- Проект Taski доступен по доменному имени, указанному в `tests.yml`.
- Пуш в ветку main запускает тестирование и деплой Kittygram, а после успешного деплоя вам приходит сообщение в
  телеграм.

</details>

<br/>
Автор проекта: Ольга М
