FROM maven:3.6.1-jdk-8-slim

RUN apt-get update -y
RUN apt-get install git-core -y

RUN mkdir -p /root/dev-env

RUN git config --system user.name "Tiago Baeta"
RUN git config --system user.email "tbaeta@illfact.lab"

COPY settings.xml /root/.m2/

CMD ["/bin/bash"]