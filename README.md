# Setup for DevOps

This guide is talking Docker, GitLab, Jenkins, etc.

More stuff will be added later.

## Docker

TODO: How to install docker and docker-compose?

## GitLab

Please ref to [docker-gitlab](https://github.com/sameersbn/docker-gitlab)

Download latest image, and go to folder `docker/gitlab`

```
docker-compose up
docker-compose stop
docker-compose start
```

## Jenkins

At this moment, the docker image of Jenkins is based on 2.7.1 LTS release.

Please ref to [docker-jenkinsci](https://github.com/jenkinsci/docker)

Download latest image, and go to folder `docker/jenkins`

Since Android appt requires 32 libs, we have to build one customized docker image.

```
docker build -t jenkins-android:2.7.1 .
docker-compose up
docker-compose stop
docker-compose start
```