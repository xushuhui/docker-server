FROM mysql:5.7.24

# set timezome
ENV TZ=Asia/Shanghai
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
#COPY /etc/my.cnf /etc/mysql/conf.d
#EXPOSE 3306

#CMD ["mysqld"]