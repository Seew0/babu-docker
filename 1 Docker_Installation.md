
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

![image](https://user-images.githubusercontent.com/96205648/200181932-a38890fc-7712-4344-9b0d-2d07c85dfb79.png)

  
<br>

### Congratulation you installed docker on your system successfully

Now for docker-compose

```
$ paru -S docker-compose 
```

very cool
