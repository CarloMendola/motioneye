# Dockerfile for motioneye image

This is a **Dockerfile** to build a docker image for **motioneye** based on **debian**:9.5.

[![Docker Automated build](https://img.shields.io/docker/automated/carlomendola85/motioneye.svg)](https://hub.docker.com/r/carlomendola85/motioneye/)
[![Docker Build Status](https://img.shields.io/docker/build/carlomendola85/motioneye.svg)](https://hub.docker.com/r/carlomendola85/motioneye/)

# Docker run example
`docker run -d --name motioneye --restart=unless-stopped --device /dev/video0 -p8765:8765 carlomendola85/motioneye:latest`

# Automated build issue
Currently automated builds with tag **latest** won't run on raspberrypi (armhf), but I pushed an image built form my own raspberry.
To run motion on **RaspberryPi** try:
`docker run -d --name motioneye --restart=unless-stopped --device /dev/video0 -p8765:8765 carlomendola85/motioneye:armhf`

