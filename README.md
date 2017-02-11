# Docker AWS Apache WSGI
AWS Apache WSGI base image based with Python 3.4.2

# Instructions
To build the base Docker image:

```
docker build -t onsdigital/docker-aws-apache-wsgi:python-3.4.2-onbuild .
```

This image assumes you have a requirements.txt and will install the
packages automatically via ONBUILD commands.

It sets up a default HEALTHCHECK to look for http://localhost/healthcheck you
should ensure this returns HTTP response code 200 if the service is healthy.
