FROM tomcat:8
MAINTAINER Jether Rodrigues<jetherrodrigues@gmail.com>

ENV APPLICATION_LINK_WAR http://jenkins.jenkins.6c6d6e4a.svc.dockerapp.io:9090/job/simple_servlet/ws/target/example.war

RUN wget ${APPLICATION_LINK_WAR} -O /usr/local/tomcat/webapps/app.war

EXPOSE 8080