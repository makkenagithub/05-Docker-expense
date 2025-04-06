FROM mysql:8.0  
# this mysql is using debian OS
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1 
# create expense group and add expense user to it. Commands are different in Debion OS
RUN groupadd expense && \
    useradd -g expense expense && \
    chown -R expense:expense /var/lib/mysql /var/run/mysqld /docker-entrypoint-initdb.d
ADD scripts/*.sql /docker-entrypoint-initdb.d
USER expense
# with the above docker file code, the image size is of  590 MB, same size 








#BEFORE BEST PRACTICE IMPLEMENTATION - Docker image size is 590MB with below file
# Instead of taking almalinux base OS and installing mysql, we can use official MYSQL image
# OFFICIAL MYSQL IMAGE.
FROM mysql:8.0  
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1 
#    MYSQL_DATABASE=transactions \
#    MYSQL_USER=expense \
#    MYSQL_PASSWORD=ExpenseApp@1

ADD scripts/*.sql /docker-entrypoint-initdb.d

