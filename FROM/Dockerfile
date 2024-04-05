FROM almalinux:8
RUN yum install nginx -y
EXPOSE 80/tcp
ENV MY_NAME="John Doe"
ENV MY_DOG=Rex\ The\ Dog
ENV MY_CAT=fluffy
CMD ["nginx", "-g", "daemon off;"]