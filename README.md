# django-postgresql


## for environment
### ________________________________________________________For Linux___________________________________

 ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   deactivate
 ```
### ______________________________________________________For Windows__________________________________________
 ```bash
 python -m venv .venv
 source .venv/Scripts/activate 
 deactivate
 ```
_______________________________________________________________________________________________________

## ----------------------------for Django----------------------------------
 ```bash
docker exec -it hotel_project-web-1 python manage.py makemigrations
docker exec -it hotel_project-web-1 python manage.py migrate
 ```
_______________________________________________________________________________________
#### to create superuser====>
```bash
docker exec -it hotel_project-web-1 python manage.py createsuperuser
```

### _________________________________Access the PostgreSQL container____________________________

![alt text](https://github.com/aa-nadim/django-postgresql/blob/main/toSeeDBinDBeaver.png?raw=true)

#### to Connect===>
 ```bash
docker exec -it postgres_db psql -U myuser -d mydatabase
```

#### See all DB===>
 ```bash
\l
```
#### to Connect espacific DB and USER===>
```bash   
\c mydatabase
```
#### to see table data, you can any query like===>
 ```bash
SELECT * FROM hotels_hotel;
```
#### to See all relations
 ```bash
\dt
```
#### to exit====>
 ```bash
\q
```
___________________________________________________

![alt text](https://github.com/aa-nadim/django-postgresql/blob/main/toSeeDB.png?raw=true)