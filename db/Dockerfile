FROM postgres:17

# install build dependencies
RUN apt-get update && apt-get -y upgrade \
  && apt-get install -y git build-essential postgresql-server-dev-17

RUN postgres --version
RUN git clone https://github.com/fboulnois/pg_uuidv7
RUN cd pg_uuidv7 && make && make install && ls -la
