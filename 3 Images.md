#Images

they are the snapshots from which we start containers they can either be built or pulled by [dockerhub](https://hub.docker.com/)

How to pull an image

```
$ docker image pull <image-name:version>
```
check available images 
```
$ docker image ls
$ docker image ls -a
```

deletion of images
```
$ docker image rm <first 3 chars of image-id>
```

images can be built with DOCKERFILES