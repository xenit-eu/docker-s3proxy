FROM docker.io/xenit/openjdk:jdk-7-trusty
LABEL maintainer="Roxana Angheluta <roxana.angheluta@xenit.eu>"

RUN mkdir /opt/s3proxy
ADD s3proxy run-docker-container.sh /opt/s3proxy/

ENV \
    LOG_LEVEL="info" \
    S3PROXY_AUTHORIZATION="aws-v2-or-v4" \
    S3PROXY_IDENTITY="local-identity" \
    S3PROXY_CREDENTIAL="local-credential" \
    S3PROXY_CORS_ALLOW_ALL="false" \
    S3PROXY_CORS_ALLOW_ORIGINS="" \
    S3PROXY_CORS_ALLOW_METHODS="" \
    S3PROXY_CORS_ALLOW_HEADERS="" \
    S3PROXY_IGNORE_UNKNOWN_HEADERS="false" \
    JCLOUDS_PROVIDER="filesystem" \
    JCLOUDS_ENDPOINT="" \
    JCLOUDS_REGION="" \
    JCLOUDS_REGIONS="us-east-1" \
    JCLOUDS_IDENTITY="remote-identity" \
    JCLOUDS_CREDENTIAL="remote-credential" \
    JCLOUDS_KEYSTONE_VERSION="" \
    JCLOUDS_KEYSTONE_SCOPE="" \
    JCLOUDS_KEYSTONE_PROJECT_DOMAIN_NAME=""
    
EXPOSE 80
VOLUME /data

ENTRYPOINT ["/opt/s3proxy/run-docker-container.sh"]





