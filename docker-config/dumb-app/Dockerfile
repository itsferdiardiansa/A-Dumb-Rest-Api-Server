from python:3.7-alpine

MAINTAINER <ferdi.ardiansa@yahoo.com> 

ENV PYTHONUNBUFFERED 1

# RUN apt-get update && \
#     apt-get install vim

COPY requirements.txt /requirements.txt
RUN pip install -r /requirements.txt

RUN mkdir /app
WORKDIR /app
COPY ./app /app

RUN adduser -D user
USER user