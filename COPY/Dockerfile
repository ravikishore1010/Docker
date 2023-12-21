FROM centos8
RUN yum install nginx -y
RUN rm-rf /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
LABEL NAME="RAVIKISHORE"\
      COURSE="DOCKER"\
      DURATION="25HOURS"
COPY mrk /usr/share/nginx/html
EXPOSE 8080