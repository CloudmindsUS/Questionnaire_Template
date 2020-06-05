# Questionnaire Template

This is a template for the health questionnaire which allows the administrator to create a survey with basic questions and manange different groups of users with different acess permissions to use it. The web application has a admin interface and a non-admin for other users.

## Prerequisites

1. Python 3.5 or higher. Prefer to use in virtual environment such as virtualenv or conda.
2. Django. If you do not have Django installed in your environment, please follow the office document provided by Django (https://www.djangoproject.com/download/).
3. Right now this template is developed using embedded Sqlite datebase. So no need to worry about the database setup. However, a MySql version is coming as well. More introduction will come when that version is ready.

## Setup

1. Create a virtual envrionment in your system and activate it.
2. Clone this repository and then navigate to its root where you can see the manage.py file.
3. ```pip install -r requirements.txt```

## Start the Project

In order to find more information about how Django works, please go to the official website (https://www.djangoproject.com/).

1. Migrate th database: ```python manage.py migrate```
2. Create the admin: ```python manage.py createsuperuser```
3. Start the local server: ```pyhon manage.py runserver```
4. Go to the website: ```127.0.0.0:8000``` or ```127.0.0.0:8000/admin```

## Functions & TO Do List

1. - [] Upgrade the database structure:
   - [x] Admin:
    - [x] Register on both backend and the admin pannel
    - [x] Login & logout
    - [x] Manage user groups
    - [x] Create & Edit surveys
    - [x] Read history logs on the changes
    - [x] View & manage survey results
   - [] Users:
    - [] Login & logout
    - [x] Access & finish the survey
2. - [] Switch to Google Material design template instead of django-material to have a better and more robust frontend UI design.
3. - [] Deploy the web application on clound server such as Heroku and AWS:
    - [] HeroKu:
      - [x] Finish the local development
      - [x] Modify settings.py so that Django app is ready to publish
      - [x] Add any necessary files/requirements to the app
      - [x] Push Django web app to Git and then to Heroku after Heroku is ready
      - [-] Gather static files
      - [] Finish the deploy
    - [] AWS:
      - onto Amazon Lightsail
      - onto AWS Elastic Beanstalk
    - [] Google Cloud:
      - 1. Finish the local development
      - 2. Change the local database to a Cloud SQL server & run it locally via a proxy
      - 3. Modify settings.py so that Django can talk to the new database
      - 4. Add any other necessary files/requirements to the app
      - 5. Gather static files
      - 6. Finish the deploy
