This repository contains code derived from https://testdriven.io/blog/dockerizing-flask-with-postgres-gunicorn-and-nginx/.
This provides instructions on how to set up Docker and implement a Flask application through Postgres on the containers.

After storing and altering the code, we can build a docker image using

```
$ docker-compose build
```

After the image is built, we run the container with

```
$ docker-compose up -d
```

Through this process we can test if the web integration is working by using

```
$ curl http://localhost:PORTNUMBER
```

Ultimately, this project's goal was to use production evironments, Nginx and Gunicron, in order to create a webs service through the server that allows users to upload media and static messages. This was hosted on Docker using Postgres.
