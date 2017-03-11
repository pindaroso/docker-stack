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
