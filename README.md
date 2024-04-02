# http-hello-world

This is a very basic Python + Flask application that simply respons "Hello, World" to HTTP requests. It is packaged in a Docker container and exposes port 5000.

Use it for testing or as a starting point for something nice.

## Instructions

* run `initdevenv.sh` to install requirements (Flask only, see `requirements.txt`)
* run `build.sh` to create and run the docker container

### Push to docker

After running and testing with `build.sh`, run the following in your terminal:

```
    docker login
    docker tag flask-hello-world yourusername/flask-hello-world:latest
    docker push yourusername/flask-hello-world:latest

    
```

* Replace yourusername and the tag latest as necessary, ask ChatGPT or do some Googling.

### Shortcut?

* The image is already available on Docker Hub as `chrfrenning/flask-hello-world:latest`