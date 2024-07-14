# Django Rest API Auth

## About The Project

This is a django rest api with authentication to be used as reference for new projects and to bootstrap new projects.

### Built With:

- [Python](https://www.python.org/) - Python is a programming language that lets you work quickly and integrate systems more effectively.
- [Django](https://www.djangoproject.com/) - Django makes it easier to build better web apps more quickly and with less code.
- [SQLite](https://www.sqlite.org/) - SQLite is a C-language library that implements a small, fast, self-contained, high-reliability, full-featured, SQL database engine.

<!-- GETTING STARTED -->

## Getting Started

<!-- PLACEHOLDER FOR PROJECT OVERVIEW -->

### Prerequisites

In order to run this project locally you will need to:

- Clone and install this repository - https://github.com/pedrovsiqueira/django_rest_auth.

### Installation

1. Clone the repo

```sh
git clone https://github.com/pedrovsiqueira/django_rest_auth
```

2. Run the app

```sh
python3 manage.py runserver
```

3. Use postman to access the following endpoints

```sh
http://127.0.0.1:8000/api/auth/signup
http://127.0.0.1:8000/api/auth/login/
http://127.0.0.1:8000/api/auth/test_token/

Use the following cURLs

cURL for Sign Up

curl --location 'http://127.0.0.1:8000/api/auth/signup/' \
--header 'Content-Type: application/json' \
--data-raw '{
    "username": "pedrovsiqueira",
    "password": "Pass1234*",
    "email": "pedro@gmail.com"
}'

cURL for Login

curl --location 'http://127.0.0.1:8000/api/auth/login/' \
--header 'Content-Type: application/json' \
--data '{
    "username": "pedrovsiqueira18",
    "password": "Pass1234*"
}'

cURL for test_token
curl --location 'http://127.0.0.1:8000/api/auth/test_token/' \
--header 'Authorization: Token 829d8debe9e9fa62eafa872d6deb868fe2b72c7b'

Users endpoint

{
    "user": {
        "username": "pedro",
        "first_name": "Pedro",
        "last_name": "Siqueira",
        "email": "pedro@gmail.com",
        "password": "123456",
        "cpf": "238.050.690-65" #random CPF generated
    },
    "type_user": {
        "type": "people"
    }
}

```

<!-- CONTACT -->

## Contact

Pedro Siqueira - [email](mailto:pedro.v.siqueira@gmail.com) - [linkedin](https://www.linkedin.com/in/pedrovsiqueira/) - [portfolio](http://pedrosiqueira.com.br/)
