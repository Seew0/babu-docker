# Docker Container

```
$ docker container run <image>
```
is the command you need to run a container but there are multiple options you have to specify to run a container efficiently such as

flags | function | example
----- | --------- |---------
p | expose a port| -p <container_port>:<host_port>
d | runs in detach mode | -d
e| sets specific env for image to run| -e MONGO_INITDB_ROOT_USERNAME=admin
v| specifies a volume to setup btw host and user| -v volume:<path_in_container(named volume)
net| specifies a network on which container should be setuped| --net <network_name>
name | assigns a name to the container | --name < name > 
----
and more ... <br>

basic example for running a container 

```
$ docker run --name some-nginx -d -p 8080:80 nginx:latest
```
