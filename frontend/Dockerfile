# take nginx official. It takes latest by default
FROM nginx
# copy the code from local to conatiner
COPY code /usr/share/nginx/html
RUN rm -rf /etc/nginx/nginx.conf
COPY nginx.conf /etc/nginx/nginx.conf
# COPY frontend.conf /etc/nginx/deafult.d/frontend.conf
