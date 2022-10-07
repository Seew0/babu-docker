
# Installation on archlinux
```
$ sudo pacman -Syu
$ sudo pacman -S docker 
$ sudo systemctl enable docker.service
```

then switch to root to use it without bs 

```
$ sudo su
```

now basic conformation stuff

```
$ docker info
$ docker image pull hello-world
$ docker container run hello-world
```
<img src="docker1.png" width=500>
  
<br>

### Congratulation you installed docker on your system successfully

Now for docker-compose

```
$ paru -S docker-compose 
```

very cool
