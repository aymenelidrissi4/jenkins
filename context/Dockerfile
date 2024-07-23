FROM ubuntu:22.04
RUN apt-get update && apt-get install -y wget openjdk-17-jre
RUN mkdir -p /var/opt/jenkins
WORKDIR	/var/opt/jenkins
RUN wget https://get.jenkins.io/war-stable/2.452.3/jenkins.war
EXPOSE 8081
CMD ["java", "-jar", "jenkins.war", "--httpPort=8081"]