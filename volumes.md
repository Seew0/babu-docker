# VOLUMES

if you run a container all the changes to make in it all 
and all the information generated in the container gets
deleted when the container is stopped to fix this volumes 
are used to store the data in the container in the host machine 
volumes are located in 
```
/var/docker/volumes
```
there are multiple types of volumes
____________________
|name|explanation|expample|
|----|------------|--------|
named|creates a named volume in host| -v <volume_name>:<path_in_container>
unamed(DECREPATED)| creates a random volume in host |-v <path_in_container>

<br>

# Binds mounts

bindind a certain file in host with the container normally used during development for eg

```
$ docker run -v  <host_file_path>:<container_file_path> <image>
```
