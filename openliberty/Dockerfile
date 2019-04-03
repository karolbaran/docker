FROM karolbaran/java:11
LABEL maintainer="Karol Baran" description="OpenLiberty 19.0.0.3"
ENV RELEASE 2019-03-21-1636
ENV VERSION 19.0.0.3
ENV INSTALL_DIR /opt
ENV CONFIG ${INSTALL_DIR}/wlp/usr/servers/defaultServer/
ENV DEPLOYMENT_DIR ${CONFIG}/dropins/

RUN curl -O -L https://public.dhe.ibm.com/ibmdl/export/pub/software/openliberty/runtime/release/${RELEASE}/openliberty-${VERSION}.zip && \
    unzip openliberty-${VERSION}.zip -d ${INSTALL_DIR} && \
    rm openliberty-${VERSION}.zip
EXPOSE 9080 9443
ENTRYPOINT /opt/wlp/bin/server run defaultServer