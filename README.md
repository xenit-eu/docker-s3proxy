# Docker image to access storage backends via s3 API

## Overview

This is the repository building a Xenit specific docker image for s3proxy. Upstream project here: https://github.com/gaul/s3proxy.

The image is automatically built by [jenkins-2](https://jenkins-2.xenit.eu) and published to hub.xenit.eu/public.

```
docker pull hub.xenit.eu/public/s3proxy:1.6.2
```

Base image is [docker.io/xenit/openjdk:jdk-7-trusty](https://cloud.docker.com/u/xenit/repository/docker/xenit/openjdk), maintained by Xenit with security updates.

Image tags follow the version number of the s3proxy artifact from Maven central.