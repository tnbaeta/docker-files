FROM jenkins/ssh-slave

# Install selected extensions and other stuff

ADD apache-maven-3.6.1-bin.tar.gz /opt

RUN mv /opt/apache-maven-3.6.1 /opt/maven

ENV M2_HOME=/opt/maven
ENV MAVEN_HOME=/opt/maven
ENV PATH=${M2_HOME}/bin:${PATH}

RUN mkdir -p /root/.m2/
ADD settings.xml /root/.m2
