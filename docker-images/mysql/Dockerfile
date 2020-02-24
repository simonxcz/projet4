FROM mysql:5.7

ADD my.cnf /etc/mysql/
ADD init_priv.sql /
ADD dump.sql /

CMD service mysql start
   # \mysql
   # \GRANT ALL PRIVILEGES ON logicaldoc.* TO logicaldoc@'%' identified by 'password'