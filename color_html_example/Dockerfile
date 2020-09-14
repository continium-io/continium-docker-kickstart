FROM nginx
ENV AUTHOR=DockerEnv

WORKDIR /usr/share/nginx/html
COPY Color_docker.html /usr/share/nginx/html

CMD cd /usr/share/nginx/html && sed -e s/DockerEnv/"$AUTHOR"/ Color_docker.html > index.html ; nginx -g 'daemon off;'




