FROM jenkins/jenkins:lts


ENV JAVA_OPTS -Djenkins.install.runSetupWizard=false
ENV CASC_JENKINS_CONFIG /var/jenkins_home/casc.yaml
COPY jcasc/plugins.txt /usr/share/jenkins/ref/plugins.txt

ENV JENKINS_ADMIN nama_admin 
ENV JENKINS_PASS password
RUN /usr/local/bin/install-plugins.sh < /usr/share/jenkins/ref/plugins.txt
COPY jcasc/casc.yaml /var/jenkins_home/casc.yaml


#USER jenkins
EXPOSE 8080

