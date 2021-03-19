# originally based on dockerhub official postgres image
ARG version=latest
FROM postgres:${version}

ARG dbuser=postgres
ENV POSTGRES_USER $dbuser

ARG dbpassword=
ENV POSTGRES_PASSWORD $dbpassword

ARG dbname=db_lavaserver
ENV POSTGRES_DB $dbname

ARG dbport=5432
ENV POSTGRES_PORT $dbport

RUN localedef -i en_US -c -f UTF-8 -A /usr/share/locale/locale.alias en_US.UTF-8
ENV LANG en_US.UTF-8

