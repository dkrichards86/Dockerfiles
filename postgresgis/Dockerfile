FROM postgres:9.6.12
LABEL maintainer="Keith Richards"
LABEL version="1.0.0"
LABEL description="PostgreSQL 9.6.12 with PostGIS installed"

RUN apt-get update && \
	apt-get install -y postgresql-9.6-postgis-2.3 && \
	apt-get install -y postgresql-9.6-postgis-2.3-scripts 
RUN echo "host all  all    0.0.0.0/0  md5" >> /var/lib/postgresql/data/pg_hba.conf
EXPOSE 5432