# stock_rest_api

This project is a the api for the stock tracker.
(https://github.com/GabrielVDN/stock-tracker)

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes. 

### Prerequisites

First of start with cloning the git repository:

```
git clone https://github.com/GabrielVDN/stock_rest_api.git
```
### Installing

Next follow these steps, start with creating a virtual environment:

```
python -m venv venv
```

Activate it: 

```
venv\scripts\activate.bat
```

Install the requirements:

```
pip install -r requirements.txt
```

Chsnge your working directory:

```
cd stock_rest_api
```

Make the necessary migrations:

```
python manage.py migrate
```

Create the necessary user:

```
python manage.py createsuperuser
```
Use 'gabriel' as username and '1' as password.
If you want to use your own credentials you will have to adjust the authorizations of the requests in stock-tracker.

Run the server:

```
python manage.py runserver
```
You can now acces the api on this address: http://127.0.0.1:8000/products/
