# s3proxy docker image

## Overview

This is the repository building a Xenit specific docker image for s3proxy. Upstream project here: https://github.com/gaul/s3proxy.

The image is automatically built by [jenkins-2](https://jenkins-2.xenit.eu) and published to [hub.xenit.eu](hub.xenit.eu/public). Base image is docker.io/xenit/openjdk:jdk-7-trusty, maintained by Xenit with security updates.

Image tags follow the version number of the s3proxy artifact from Maven central.