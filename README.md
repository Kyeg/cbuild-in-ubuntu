Build & Run the docker image (Ubuntu 24.04)
```
$ cd cbuild-in-ubuntu
$ docker build -t cbuild-in-ubuntu -f Dockerfile.cbuild .
$ docker run -it -h cbuild-in-ubuntu -v ./workdir:/root/workdir --name cbuild-in-ubuntu cbuild-in-ubuntu
```

Remember your container name/id, so that you can start it again.
```
$ docker start -i <container-name or container-id>
```