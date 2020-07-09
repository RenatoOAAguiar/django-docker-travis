1. `docker-compose run app sh -c "django-admin.py startproject app ."`
2. `docker-compose run app sh -c "python manage.py startapp core"`
3. Change default user model:
    - Go to settings file;
    - Add AUTH_USER_MODEL = 'app.Class'
4. `docker-compose run app sh -c "python manage.py makemigrations core"`