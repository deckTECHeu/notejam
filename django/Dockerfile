FROM python:2.7-alpine

ENV PYTHONUNBUFFERED 1

COPY ./requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

RUN mkdir /notejam
WORKDIR /notejam
COPY ./notejam /notejam

RUN adduser -D user
USER user
