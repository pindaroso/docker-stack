[![Build Status](https://travis-ci.org/stilesb/docker-stack.svg?branch=master)](https://travis-ci.org/stilesb/docker-stack)

# docker-stack

*Stack and Nix docker image using minimal Debian base*

## Setup

**Requirements**

* Docker

**Building**

`make`

**Usage**

`docker pull stilesb/stack:latest`

Extending via Dockerfile:

```Dockerfile
FROM stilesb/stack:latest
WORKDIR /home/robot/code
ADD . .
RUN stack setup
RUN stack build
```

## Notes

```bash
$ docker images
REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
stilesb/stack       latest              b8d74f8e4c12        8 minutes ago       485.5 MB
```
