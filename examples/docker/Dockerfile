FROM python:2.7.11
MAINTAINER Fiona Hasanaj
ENV MAINTENANCE_DATE 03.28.2016

# install necessary software
RUN apt-get -y update && apt-get install -y vim  && apt-get install -y git && pip install rosette_api

COPY run_python.sh /python/examples/run_python.sh
RUN chmod 755 /python/examples/run_python.sh
WORKDIR /python/examples

# allow interactive bash inside docker container
CMD ./run_python.sh

VOLUME ["/source"]
