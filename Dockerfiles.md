# Dockerfiles 

Custom docker images can be made with DockerFiles
with command
```
$ docker build -t <name> -f <dockerfile> <path_where_to build>
```
Dockerfile Format 

```
FROM [some base image]

ENV [specific enviroment variable for the project to run]

RUN [sh commands to run to setup the image]

COPY [host_files] [path_in_container]

WORKDIR [to set a specific work dir]

EXPOSE [exposes certain port for image]

VOLUME [specify what volume to connect to]

USER [specify a user]

CMD [runs specific command on startup]
```

example of a Dockerfile

```
FROM python:3.9.1-alpine3.12

RUN pip install flask

WORKDIR /app
COPY rest-api.py .
RUN chmod u+x rest-api.py
RUN chown xfs rest-api.py

USER xfs 
CMD [ "python", "./rest-api.py"]
```