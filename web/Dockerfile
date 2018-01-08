FROM python:3.5

ENV PYTHONUNBUFFERED 1
# Install dependencies
RUN apt-get update -qq && apt-get install -y cron vim curl git nginx \
    && rm -rf /var/lib/apt/lists/*

RUN mkdir /web
WORKDIR /web
COPY . /web
RUN pip install -r requirements.txt
