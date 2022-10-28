# Jenkins-pipeline

## Description
This repo contains my personal project for jenkins CI/CD pipeline.

How to run jenkins 

```
mkdir /var/jenkins_home
chown -R 1000.1000 /var/jenkins_home
docker run -d -p 8080:8080 -p 5000:5000 --name jenkins -v /var/jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```
