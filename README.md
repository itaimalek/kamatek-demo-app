# kamatek-demo-app
In this excersise you will dockerize a Python demo application.
This is a simple Python Flask web application. The app provides system information and a realtime monitoring screen with dials showing CPU, memory, IO and process information.

The application requires Python 3.8 or higher !

You'll need to fork this repository, and create your own Dockerfile making this code base into a docker Image that can be run anywhere 😎.  

Please do the whole excersise in WSL2 !

## Run the App locally:
_It is recomended to use [PyEnv](https://github.com/pyenv/pyenv) to run locally_
* Install requirements with `requirements.txt`
* Run the application with `python3 run.py`
* Once ran test the app in your browser

## Dockerize your application:
* Create a Dockerfile  that will COPY this codebase, build the app and would be able to run a container once turned into an image.
* Container from that image should:
  * Run the application as a different user from `root`
  * Run on port determined at `docker build` command with environment variable `PORT`
* Build an image from your Dockerfile (make sure to use your docker hub repo as suffix (i.e `<my docker hub repository>/<image name>:<tag>`
* Run your container locally and expose it to your local machine port
* Test it on your browser
* Push your image to your Docker Hub repository

## Build and Run using Docker Compose
* create a docker-compose file for building and running your image

_Search docker hub for the correct base image for you !_

_use this [dockerfile reference](https://docs.docker.com/engine/reference/commandline/build/) for more information on dockerfile !_

_use this [docker-compose video](https://www.youtube.com/watch?v=j2wf_WHjjpc) for training how to build via docker-compose_

Good Luck !
😊
