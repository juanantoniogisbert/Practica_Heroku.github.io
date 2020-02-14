- Primer paso instalar heroku cli

Fichero Procfile
    web: gunicorn djangobackend.wsgi --log-file -


Fichero requirements.txt
    gunicorn

```
$ sudo snap install --classic heroku
```

despues 

```
$ heroku login
```
![Alt text](images/terminalLogin.png)
![Alt text](images/cap3.png)
![Alt text](images/capLoginBrow.png)
![Alt text](images/capLoginBrow.png)

Creem el repositori 
añadim projecte 
add/commit/push a master

```
$ heroku create
```
![Alt text](images/herokucreate.png)


```
$ heroku git:remote -a practicaheroku01
```
![Alt text](images/cap4.png)


```
$ git push heroku master
```

Hemos tenido un error y tenemos que escribir el siguiente comando
![Alt text](images/caperror.png)

```
$ heroku config:set DISABLE_COLLECTSTATIC=1D
$ git push heroku master
```
![Alt text](images/capfinal.png)

```
$ heroku ps:scale web=1
```
![Alt text](images/capFun.png)



```
https://practicaheroku01.herokuapp.com/admin/login/?next=/admin/
```

Dins de practica resources/Heroku Postgres/Settings

Configuracion de settings

![Alt text](images/capSetings.png)

practicaheroku01/More/Run Console

![Alt text](images/superuser.png)

![Alt text](images/despHero.png)

![Alt text](images/hotels.png)

Configutación 

![Alt text](images/addons.png)

![Alt text](images/installaddon.png)


A continuación vamos a realizar una prueba de aplicación en entorno local.

Para ello ejecutamos el siguiente comando.
```
$ heroku local web
```
![Alt text](images/local1.png) 

Pantalla de login.

![Alt text](images/local.png)

Pantalla de administración (Después de iniciar sesión)