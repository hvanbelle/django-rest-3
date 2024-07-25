# django-rest-3

## Links
- https://www.django-rest-framework.org/tutorial/quickstart/

## Commands 1 
- pip install djangorestframework
- pip install django # not needed, done by previous
- pip install python-dotenv
- django-admin startproject tutorial .
- cd tutorial
- django-admin startapp quickstart
- cd ..
- python manage.py migrate
- python manage.py createsuperuser --username admin --email admin@example.com
- python manage.py runserver

## Commands 2
```
bash: curl -u admin -H 'Accept: application/json; indent=4' http://127.0.0.1:8000/users/
Enter host password for user 'admin':
{
    "count": 1,
    "next": null,
    "previous": null,
    "results": [
        {
            "url": "http://127.0.0.1:8000/users/1/",
            "username": "admin",
            "email": "admin@example.com",
            "groups": []
        }
    ]
}
```