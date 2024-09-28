# Docker-files
Set of docker files for everyday use



### Check version
```
docker --version
```


## docker image build from docker file
```
docker build -t sample-name .
```

### docker image run
```
docker run -p 80:80 sample-name
```

## docker image run detached mode
```
docker run -d -p 80:80 sample-name
```
### list all running containers
```
docker ps
```
### List all containers
```
docker ps -a
```

### to stop container
```
docker stop container-id
```


### TO Start Container 
```
docker start container-id
```

### to log in to the container
```
docker exec -it <container_id> /bin/sh
```
### to check logs 
```
docker logs <container_id>
```