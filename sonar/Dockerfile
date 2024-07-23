FROM ubuntu:22.04
RUN apt-get update && apt-get install -y wget openjdk-17-jre
RUN mkdir -p /var/opt/sonar
WORKDIR	/var/opt/sonar
RUN wget https://binaries.sonarsource.com/CommercialDistribution/sonarqube-developer/sonarqube-developer-10.6.0.92116.zip?_gl=1*13sammm*_gcl_au*MjEwNzQ2ODA3NC4xNzIxNzQxNzA1*_ga*MzgwMzY4ODIzLjE3MTIwMTE2MjA.*_ga_9JZ0GZ5TC6*MTcyMTc0MTcwNS4yLjEuMTcyMTc0MjI0MS4yMi4wLjA.
RUN unzip sonarqube-developer-10.6.0.92116.zip
ENV SONAR_JAVA_PATH=$JAVA_HOME
EXPOSE 9000
CMD ["tail", "-f", "/dev/null"]