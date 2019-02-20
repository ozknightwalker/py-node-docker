# py-node-docker
Python Node Docker Image

[![Build Status](https://travis-ci.org/ozknightwalker/py-node-docker.svg?branch=master)](https://travis-ci.org/ozknightwalker/py-node-docker)

Based Images:

https://hub.docker.com/_/node/ 8.15.0-alpine
https://hub.docker.com/_/python 3.6.8-alpine

This image is based off the python v3.6.8 image and node v8.15.0 alpine based from the official docker image.

## Pull from Docker Hub
```command
docker pull jcdin/py-node:latest
```
##Run image
```command
docker run -it --rm  jcdin/py-node:latest /bin/sh -c "python -V && pip --version && node -v && npm -v && yarn --version"
```
this will return the python, pip, node, npm, and yarn package version

Use as base image
```Dockerfile
FROM jcdin/py-node:latest
```