FROM python:3.8.5

ENV PYTHONUNBUFFERED 1
RUN mkdir /workspace
WORKDIR /workspace
ADD ./docker/python/requirements.txt /workspace/
RUN pip install --upgrade pip
RUN pip install -r requirements.txt
COPY src/ /workspace/
CMD uwsgi --socket :8001 --module app.wsgi --py-autoreload 1 --logto /tmp/tmp.log