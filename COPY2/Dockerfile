
# Use an official AlmaLinux base image
FROM almalinux:8
ENV APP_HOME=/app
WORKDIR ${APP_HOME}

# Install Nginx using dnf
RUN yum install -y nginx

# Remove the default Nginx index.html
RUN rm -rf /usr/share/nginx/html/index.html

# Copy your HTML content to the Nginx web server root
COPY oxer-html /usr/share/nginx/html/

# Start Nginx with the correct CMD and expose the default Nginx port
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80

# Download Apache HTTP Server
ADD https://httpd.apache.org/download.cgi#apache24 ./

# Download a sample Dockerfile from a GitHub repository
ADD https://raw.githubusercontent.com/techworldwithsiva/dockerfiles/master/ADD/Dockerfile ./

LABEL COURSE="devops"\
      DURATION="25HOURS"\
      IMAGE="LEO"
