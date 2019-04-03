FROM karolbaran/openliberty:jee8-microprofile
LABEL maintainer="Karol Baran" description="Openliberty Java EE 8 + MicroProfile 2.2 + Postgres"

ADD http://central.maven.org/maven2/org/postgresql/postgresql/9.4.1212/postgresql-9.4.1212.jar ${INSTALL_DIR}lib/postgresql-9.4.1212.jar

COPY postgres-driver.xml ${CONFIG}configDropins/defaults/