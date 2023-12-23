FROM almalinux:8
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
COPY oxer-html /usr/share/nginx/html/
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 8080
LABEL NAME="RAVIKISHORE"\
      COURSE="DOCKER"\
      DURATION="25HOURS"
ADD https://httpd.apache.org/download.cgi#apache24 /tmp/
ADD https://github.com/techworldwithsiva/dockerfiles/blob/master/ADD/Dockerfile /tmp/