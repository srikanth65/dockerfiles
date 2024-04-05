FROM almalinux:8
RUN yum install nginx -y
COPY index.html /usr/share/nginx/html/
EXPOSE 80/tcp
ENV TEST="Test ENV variable"
CMD ["nginx", "-g", "daemon off;"]