FROM ubuntu:22.04
RUN apt-get update && apt-get install -y wget unzip openjdk-17-jre
RUN mkdir -p /var/opt/sonar
WORKDIR	/var/opt/sonar
RUN wget https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.6.0.92116.zip
RUN unzip sonarqube-developer-10.6.0.92116.zip
ENV SONAR_JAVA_PATH=$JAVA_HOME
WORKDIR	/var/opt/sonar/sonarqube-developer-10.6.0.92116/bin/linux-x86-64
EXPOSE 9000
CMD ["tail", "-f", "/dev/null"]
# CMD ["./sonar.sh"]