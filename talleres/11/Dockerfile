FROM python:3.7-alpine
#software version of image , https://hub.docker.com/
EXPOSE 8000/TCP

WORKDIR /opt/app

COPY . .
#COPY [--chown=<user>:<group>] <src>... <dest>

RUN pip install -r requirements.txt
#excecute commands, see example
#RUN /bin/bash -c 'source $HOME/.bashrc; \
#echo $HOME'
ENTRYPOINT ["gunicorn", "-w", "3", "-b", "0.0.0.0:8000", "app:app"]
#ENTRYPOINT ["executable", "param1", "param2"]
#un contenedor solo puede corres un proceso de ejecucion