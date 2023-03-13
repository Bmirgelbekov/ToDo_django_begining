# Setup Django Project

1. Создать виртуальное окружение 
`python3 -m venv venv`

2. Активировать виртуальное окружение 
`source venv/bin/activate`

3. Создать файл requirements.txt
`touch requirements.txt`

4. Записать зависимости/библиотеки
```
django
djangorestframework
psycopg2-binary
python-decouple
```
5. Установить библиотеки
`pip install -r requirements.txt`

6. Развернуть проект
`django-admin startproject <project_name> .`

7. Создать базу данных для проекта
`createdb <db_name>`

8. Настроить базу данных в переменной DATABASES в файле setting.py

9. создать приложение 
`python3 manage.py startapp <app_name>`

10. Зарегистрировать приложение/занести в список INSTALLED_APPS в файле settings.py

11. Занести в INSTALLED_APPS rest_framework

12. Создать миргации
`python3 manage.py makemigrations`

13. Применить миргации 
`python3 manage.py migrate`

14. Создать супер-пользователя
`python3 manage.py createsuperuser`

15. Запустить сервер
`python3 manage.py runserver [port]`