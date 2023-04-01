# App Deployed in Heroku

In order to deploy the application, i used the following tutorial:
https://www.youtube.com/watch?v=8UwQqQoUWp4 

And Heroku documentation:
https://devcenter.heroku.com/articles/container-registry-and-runtime

This where the steps that I followed:

```
heroku container:push web -a colfuturo-project-docker
```

```
heroku container:release web -a colfuturo-project-docker
```

```
heroku open -a colfuturo-project-docker
```

According to the documentation, the 'EXPOSE' command in Heroku doesn't work, so I changed the Dockerfile, so it uses the $PORT environment variable.


Link to the deployed application:

https://colfuturo-project-docker.herokuapp.com/