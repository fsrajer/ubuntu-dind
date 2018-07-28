# ubuntu-dind
A docker-in-docker image, always up-to-date image that uses the most stable and latest Ubuntu image.

## Build
```bash
docker build --tag ubuntu-dind --build-arg UBUNTU_VERSION=16.04 .
```

## Run
```bash
docker run --privileged -it -d --name foo_dind ubuntu-dind
docker exec -it foo_dind /bin/bash
```

## Credits 

This docker is based on jpetazzo's dind. Credits to them.
