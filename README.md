# Folding at home on Docker

Docker image for Folding@home on linux

Github : [![https://github.com/InfraBuilder/docker-foldingathome](https://img.shields.io/badge/Github-infraBuilder%2Fdocker--foldingathome-lightgrey)](https://github.com/InfraBuilder/docker-foldingathome)

Docker : [![https://hub.docker.com/r/infrabuilder/foldingathome](https://img.shields.io/badge/Docker-infraBuilder%2Ffoldingathome-blue)](https://hub.docker.com/r/infrabuilder/foldingathome)


## Availables tags

- [lastest (Dockerfile)](https://github.com/InfraBuilder/docker-foldingathome/blob/master/Dockerfile) - ![Docker Image Size (tag)](https://img.shields.io/docker/image-size/infrabuilder/foldingathome/latest)![GitHub last commit (branch)](https://img.shields.io/github/last-commit/InfraBuilder/docker-foldingathome/master)

## How to run this image

Start folding with no GPU (GPU=false) but every CPU cores (CPUS=0) :

```
docker run -d --name foldingathome \
    -e USER="yourusername" \
    -e TEAM="yourteam" \
    -e PASSKEY="yourpasskey" \
    -e GPU="yourusername" \
    -e CPUS="0" \
    infrabuilder/foldingathome
```

Start folding with only 1 CPU core (CPUS=1) :

```
docker run -d --name foldingathome \
    -e USER="yourusername" \
    -e TEAM="yourteam" \
    -e PASSKEY="yourpasskey" \
    -e GPU="yourusername" \
    -e CPUS="1" \
    infrabuilder/foldingathome
```

## What if I have no team ?

Feel free to join infraBuilder team : 236450

## How to generate a passkey :

Go to : https://apps.foldingathome.org/getpasskey

*More information on https://foldingathome.org/support/faq/points/passkey/*

## Statistics

Visit https://stats.foldingathome.org/donors
