Link to the project in docker hub:
[Docker hub link](https://hub.docker.com/repository/docker/sebitasrb09/colfuturo_project/general)

In this same folder, is the Dockerfile. It would not work by itself, but is here just to check it.

# ColfuturAnalisis

Bienvenidos al proyecto Colfuturo Analisis! En este proyecto evaluó los datos abiertos de la organización sobre los beneficiarios del credito-beca. Este es un proyecto que no esta relacionado con la organización.

Welcome to the Colfuturo Analysis Project! In this project open data from Colfuturo is analized, the data is related to the beneficiaries of the scholarship. This is a project that is not related to the organization. The project is in Spanish.

## Docker
In order to use the docker, create the container with the following comand:

```
docker build . -t colfuturo
```
After that, you can run the following:

```
docker run -p 8501:8501 colfuturo
```

Great! Now go to your browser, localhost:8501, or go here once you have done the previous steps: [Colfuturo](http://localhost:8501)