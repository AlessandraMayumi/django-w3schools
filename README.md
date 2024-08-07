# django-w3schools
Study Django with W3Schools

https://www.w3schools.com/django/index.php

```sh
# create project
django-admin startproject my_tennis_club
cd my_tennis_club
# migrate
python manage.py migrate
# start server
python manage.py runserver
```

Create App, page members

```sh
# create app 'members'
python manage.py startapp members
# make migrations
python manage.py makemigrations members
python manage.py migrate
# view the SQL statement
python manage.py sqlmigrate members 0001
# python interpreter to add records
python manage.py shell
>>> from members.models import Member
>>> member = Member(firstname='Emil', lastname='Refsnes')
>>> member.save()
>>> Member.objects.all().values()
```