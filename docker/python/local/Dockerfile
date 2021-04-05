FROM python:3.8.5

ENV PYTHONUNBUFFERED 1
RUN mkdir /workspace
WORKDIR /workspace
ADD ./docker/python/local/requirements.txt /workspace/
RUN pip install --upgrade pip
RUN pip install -r requirements.txt