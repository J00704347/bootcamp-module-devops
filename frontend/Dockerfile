FROM nginx:1.18.0
#software version of image , https://hub.docker.com/
EXPOSE 80/TCP

WORKDIR /usr/share/nginx/html

COPY . .
#COPY [--chown=<user>:<group>] <src>... <dest>

#RUN docker run --name some-nginx2 -v $(pwd):/usr/share/nginx/html:ro -d -p 8087:80 nginx
#excecute commands, see example
#RUN /bin/bash -c 'source $HOME/.bashrc; \
#echo $HOME'
#docker run --name some-nginx -v /some/content:/usr/share/nginx/html:ro -d nginx

#ENTRYPOINT ["gunicorn", "-w", "3", "-b", "0.0.0.0:8000", "app:app"]
#ENTRYPOINT ["executable", "param1", "param2"]
#un contenedor solo puede corres un proceso de ejecucionld