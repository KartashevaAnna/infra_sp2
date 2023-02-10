# Api_yamdb

## This is an API project where I train to use docker.
### The following stack is used:
- Docker
- Gunicorn
- Nginx
- Python
- Django
- Django REST Framework
- Simple JWT
- Postgres


### Description:
The project collects user reviews on various titles. 
The titles are split per genre and category. An average rating is built based on separate user ratings. 
One user can specify only one rating per title.

You may find a detailed API description at http://127.0.0.1:8000/swagger/.

### Instructions:
To run the project, 
- install the docker, run it
- open linux shell in infra_sp2/infra/ and run the following commands:
- - docker-compose exec web python manage.py migrate
- - docker-compose exec web python manage.py createsuperuser
- - docker-compose exec web python manage.py collectstatic --no-input
- - docker-compose exec web python manage.py loaddata fixtures.json

### Author:
Anna Kartasheva, Yandex Praktikum Student
