FROM nginx:1.18-alpine

RUN mkdir /workspace
WORKDIR /workspace
COPY ./docker/nginx/prod/default.conf /etc/nginx/conf.d/default.conf
COPY ./docker/nginx/prod/uwsgi_params /etc/nginx/uwsgi_params
COPY src/ /workspace/