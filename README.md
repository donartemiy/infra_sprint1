# infra_sprint1

kittygram - готовый к деплою сайт по добавлению котиков с выбром цвета шерстки, года рождения.


## Стек
 - Python 3.10.6
 - Django
 - React

## Установка
Настройка окружения
```bash
git clone git@github.com:donartemiy/infra_sprint1.git

# Backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
cd infra_sprint1/backend
python manage.py migrate
python manage.py createsuperuser

# Заполнить переменные окружения по аналогии с файлом .env_example, переименовать файл
vi infra_sprint1/backend/kittygram_backend/.env_exmaple
mv .env_exmaple .env

# Frontend
curl -fsSL https://deb.nodesource.com/setup_18.x | sudo -E bash - &&\
sudo apt-get install -y nodejs
npm i
```

## Запуск проекта
```bash
# Запуск backend
cd infra_sprint1/backend
python manage.py runserver 0.0.0.0:8000

# Запуск frontend
cd taski/frontend/
npm run start
```

# Автор
- donartemiy
