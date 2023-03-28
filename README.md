# Cinema API

API project for cinema management written on DRF

### Features

* JWT Authentication
* Admin panel /admin/
* Documentation at /api/doc/swagger/
* Management of orders and tickets
* Creating movies with genres, actors
* Creating cinema halls
* Adding movie sessions
* Filtering movies and movie sessions

## Installing using GitHub

Install Postgres and create db

```
git clone https://github.com/Nexxel05/Cinema_api.git
cd Cinema_api
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver 
```

You can create environmental variables either 
directly in terminal, like below

```
set POSTGRES_HOST=<your db hostname>
set POSTGRES_DB=<your db name> 
set POSTGRES_USER=<your db user> 
set POSTGRES_PASSWORD=<your db password> 
set SECRET_KEY=<your db secret key>
```

or create .env in project root directory and store 
values there like shown in .env_sample.

## Run with Docker

Docker should be installed

```
docker-compose build
docker-compose up
```

## Getting access
1. Navigate to /api/user/register/ and create user
2. Navigate to api/user/token/ and get your token
