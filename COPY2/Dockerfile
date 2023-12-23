
# Use an official AlmaLinux base image
FROM almalinux:8

# Install Nginx using dnf
RUN dnf install -y nginx

# Remove the default Nginx index.html
RUN rm -rf /usr/share/nginx/html/index.html

# Copy your HTML content to the Nginx web server root
COPY oxer-html /usr/share/nginx/html/

# Start Nginx with the correct CMD and expose the default Nginx port
CMD ["nginx", "-g", "daemon off;"]
EXPOSE 80

# Download Apache HTTP Server
ADD https://www.apache.org/dist/httpd/httpd-2.4.51.tar.gz /tmp/

# Download a sample Dockerfile from a GitHub repository
ADD https://raw.githubusercontent.com/techworldwithsiva/dockerfiles/master/ADD/Dockerfile /tmp/
