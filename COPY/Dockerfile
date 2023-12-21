FROM centos:8
RUN yum install nginx
RUN rm-rf /usr/share/nginx/html/index.html
CMD ["nginx", "-g", "daemon off;"]
LABEL NAME="RAVIKISHORE"\
      COURSE="DOCKER"\
      DURATION="25HOURS"
COPY website /usr/share/nginx/html
EXPOSE 8080