# instead of taking alma linux as base os and installing node js version 20, we can use official node js image with version 20.
FROM node:20
# backend uses 8080 port. EXPOSE command is for port information purpose. It does not open the port
EXPOSE 8080
# we have to give private IP of mysql container. Its IP is not constant , it changes frequently. 
# Hence we use container name here, to connect backend to DB. While running mysql container, give container name as 'mysql'
ENV DB_HOST="mysql"

RUN mkdir /opt/server
WORKDIR /opt/server
COPY package.json .
COPY *.js .
# install the dependencies
RUN npm install
CMD ["node", "index.js"]




