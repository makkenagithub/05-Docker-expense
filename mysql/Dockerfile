









#BEFORE BEST PRACTICE IMPLEMENTATION - Docker image size is 590MB with below file
# Instead of taking almalinux base OS and installing mysql, we can use official MYSQL image
# OFFICIAL MYSQL IMAGE.
FROM mysql:8.0  
ENV MYSQL_ROOT_PASSWORD=ExpenseApp@1 
#    MYSQL_DATABASE=transactions \
#    MYSQL_USER=expense \
#    MYSQL_PASSWORD=ExpenseApp@1

ADD scripts/*.sql /docker-entrypoint-initdb.d

