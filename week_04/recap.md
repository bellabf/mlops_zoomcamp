Goals:

1) The idea is to take the pickle file and put it as a docker application.

The steps are more of less 
 1.1) virtual env
 1.2) a script for predictions
 1.3) script into a flask app
 1.4) packaging to docker.

Breakdown: 
* get the exact version of sklearn we were using
* create pip env 
* create predict to handle the predictions
* create flask application inside prediction
* connect with test to test it out
* install gunicorn (to use a production deployment)
* use gunicorn for production (a proper WSGI server)

```bash 
gunicorn --bind=[adress] [application_script]:app
```

* you only need the library resquests to test, so you can install it as dev dependency 
* create the dockerfile image per intructions
* execute the dockerfile image per instructiosn too 

2) Use the same thing connecting to the mlflow repo