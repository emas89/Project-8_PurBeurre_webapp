# PUR BEURRE Web App
## A nutritional advisor that helps users to eat healthier foods

![Pur Beurre Homepage](https://github.com/emas89/Project-8_PurBeurre_webapp/blob/master/purbeurre/static/purbeurre/img/thumb.jpg)

### Project based on OpenFoodFacts data (https://fr.openfoodfacts.org/)
#### Demo here: https://purbeurre-webapp.herokuapp.com/

# Setup
-----------------------------------------------
## 1. Requirements :
* Python 3.x
* Django 2.0.7
* **pip** package management system
* PostgreSQL
* Using a virtual environment is highly recommended
* Dependencies in **requirements.txt** (use `pip install -r requirements.txt` to install them)
------------------------------------------------
## 2. Database :
* PostgreSQL because of project's hosting on Heroku
* **DB's structure implementation** : use `manage.py migrate` command
* **DB update** : use `manage.py api_off` command to populate it with latest using OpenFoodfacts API
------------------------------------------------
## 3. Environment Variables and Heroku Deployment :
This project is ready to deploy on Heroku platform. In order to run it, please set following environment variables :
* `Django Secret Key` -> Secret key used by Django to generate CSRF token;
* PostgreSQL DB name for local use;
* PostgreSQL password for local use;
* PostgreSQL username for local use;
* `ENV` -> App environment: it can be DEVELOPMENT or PRODUCTION.

To deploy the application on Heroku, please set `ENV=PRODUCTION` by using **Heroku Postgres** and **Whitenoise**.
