# django-gunicorn-nginx-postgres

The goal of this project is to learn docker but can be used as the basis for real projects.

## Requirements

 * Docker 1.10.0+
 * Compose 1.6.0+

## Up and Running

Assuming you've just cloned this repository, the following steps
will get you up and running in no time!

##  Make our local directories.

```
   mkdir -p  logs media static postgres
```

##  Create the Django project using the docker-compose command.

```
   docker-compose run django django-admin.py startproject myproject .
```

## Change the ownership of the new files.

```
    sudo chown -R $USER:$USER .
```


## Lift all services (detached/background mode).

```
    docker-compose up -d
```

Access your instance at `localhost:8000`
