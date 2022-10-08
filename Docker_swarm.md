# Swarm

swarm is basically a tool to helps create services by distributing work across nodes 

just like good-aulad ek kaam bol do karta rahega jabtak koi bhi dikkat aye <bold>JAB TAK TUM NA ROKO</bold>

<li>it was first released in 2016 summer via swarmkit toolkit
<li> it was then updated in 2017 via secrets and stacks

```
$ docker swarm
$ docker node
$ docker service 
$ docker stack
$ docker secret
```

Swarm is not available in a fresh installl

```
$ docker info
```

look for swarm if inactive
then execute

``` 
$ docker swarm init
```

```
$ docker service
$ docker node
$ docker update
```

docker node is used mainly to assign positions and stuff to swarm members

swarm is basically robin and you are batman jo bolo kardeta aur karta rehta

with docker service u can start services for eg
```
docker service create <image> <command>
```

docker update and docker service update can be used to change config of  a running container according to circumstances

# Multi-Node Swarm 


## PWD(play with docker)
<li> is an online solution but does not work most of the time

## Cloud Services
<li>AWS,Azure or Google

## Vm
<li> make your VM with oracle virtualbox or the best Virt-Manager

<br>

# Setting up Multi-node service

<li> Setup your alternative instance
<li> install docker on it with <a href="https://get.docker.com/">docker</a> or setup it manually
<br>
<br>

```
$ docker swarm init 
```
you will get a join token

```
$ docker swarm join --token [TOKEN] [PORT]
```

paste it in your instance or 2nd node 

connection successful

you can check nodes with

```
$ docker node ls
```

change the permissions of a node with
```
$ docker node promote/demote [node-name]
```

start service

```
$ docker service create --[Options] [image] [port]
```


