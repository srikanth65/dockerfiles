FROM almalinux:8
RUN yum install nginx -y
RUN rm -rf /usr/share/nginx/html/index.html
# COPY index.html /usr/share/nginx/html/
ADD https://chromium.googlesource.com/external/github.com/GoogleCloudPlatform/appengine-gcs-client/+/refs/heads/halgrimur-patch-3/java/example/war/index.html /tmp/
ADD /tmp/index.html /usr/share/nginx/html/
EXPOSE 80/tcp
ENV TEST="Test ENV variable"
CMD ["nginx", "-g", "daemon off;"]