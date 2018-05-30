# hping easily on docker
## usecase
You can use this when you cannnot install hping3 or you don't want to install it in your machine. 

## When you want to use this on docker machine
```bash
$ docker-machine create --driver=virtualbox hping
$ eval $(docker-machine env hping)
```

## build image
```bash
$ docker build -t hping:latest ./
```

## run
```bash
$ docker run hping:latest hping3 -S -p 80 ****.com 
```
