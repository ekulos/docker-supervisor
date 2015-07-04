# Docker Supervisor

This repository contains **Dockerfile** of [Supervisor](http://supervisord.org/).

### Base Docker Image

* [dockerfile/ubuntu](http://dockerfile.github.io/#/ubuntu)

### Installation

1. Install [Docker](https://www.docker.com/).

2. Build an image from Dockerfile: `docker build -t="jslucas/docker-supervisor" https://github.com/jslucas/docker-supervisor`)

### Usage

    docker run -it --rm jslucas/docker-supervisor

#### Run with custom config directory

    docker run -d -v <config-dir>:/etc/supervisor/conf.d jslucas/docker-supervisor
