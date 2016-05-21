# django-memcache
Django memory caching

# Dependencies
1. Setting up env

```
    sudo apt-get install python python-dev python-pip libmemcached-dev memcached python-memcached
    sudo pip install pylibmc python-memcached django
```

2. Setting up memcache server (default location is 127.0.0.1:11211)

```
    sudo service memcached start
```

3. Setting up project

```
    cd ~
    git clone https://github.com/kendricktan/django-memcache.git
    cd django-memcache/memcache
    python manage.py makemigrations
    python manage.py migrate
    python manage.py runserver
```

4. Navigate to:
```
    127.0.0.1:8000 # add questions to database
    127.0.0.1:8000/db_cache # query database (cached) dump
    127.0.0.1:8000/db_nocache # query database (non-cached) dump
```    
