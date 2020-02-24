FROM tomcat

ADD logicaldoc.war /usr/local/tomcat/webapps

WORKDIR /tmp
RUN apt-get update
RUN apt-get install -y wget
RUN wget http://repo.mysql.com/mysql-apt-config_0.8.13-1_all.deb
RUN apt-get update
RUN apt-get install -y ./mysql-apt-config_0.8.13-1_all.deb 
# RUN apt-get install -y mysql-server

RUN /usr/local/tomcat/bin/catalina.sh start