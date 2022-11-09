# Jenkins-pipeline

## Description
This repo contains my personal project for jenkins CI/CD pipeline.


How to build Docker jenkins

```
cd docker
docker build -t jenkins:jscac .
```

How to run jenkins 

Create folder jenkins_home and change ownership to 1000.1000
```
mkdir /var/jenkins_home
chown -R 1000.1000 /var/jenkins_home
```

Run jenkins docker and mount jenkins_home folder
```
docker run -d -p 8080:8080 -p 5000:5000 --name jenkins -v /var/jenkins_home:/var/jenkins_home jenkins/jenkins:lts
```
