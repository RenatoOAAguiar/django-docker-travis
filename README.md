1. `docker-compose run app sh -c "django-admin.py startproject app ."`
2. `docker-compose run app sh -c "python manage.py startapp core"`
3. Change default user model:
    - Go to settings file;
    - Add AUTH_USER_MODEL = 'app.Class'
4. `docker-compose run app sh -c "python manage.py makemigrations core"`
5. `Learn about flake8`
6. `docker-compose run app sh -c "python manage.py createsuperuser"`
7. `docker-compose run --rm app sh -c "python manage.py startapp user"`
8. Patch change only fields provided, put change all
9. In ManyToManyField, if object is passed with param, the order of object need to be respected, the object passed there need to be before.
But, if the object name is in string quotes, this will be not necessary.
