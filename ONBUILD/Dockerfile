FROM almalinux:9
RUN dnf install nginx -y
RUN rm -f /urs/share/nginx/html/index.html
#this instruction runs when someone runs this image
ONBUILD COPY index.html /usr/share/nginx/html
CMD ["nginx", "-g", "daemon off;"]
