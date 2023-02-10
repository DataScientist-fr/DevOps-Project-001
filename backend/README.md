# TODO-List Backend application

## Install requirements
```
pip install -r requirements.txt
```
> This will install all the required packages for the application :
> - Django
> - Django REST Framework


## Setup Database

Create or migrate the database with the following command:
```
python todo/manage.py migrate
```

Create a superuser for the application:
```
python todo/manage.py createsuperuser
```


## Run the application
```
python todo/manage.py runserver
```
> This will run the application on port 8000.  
> You can access the application on http://localhost:8000