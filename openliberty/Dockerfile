FROM karolbaran/java:11
LABEL maintainer="Karol Baran" description="OpenLiberty 19.0.0.4"
ENV RELEASE 2019-05-15_0301
ENV VERSION 19.0.0.5-cl190520190515-0301
ENV INSTALL_DIR /opt
ENV CONFIG ${INSTALL_DIR}/wlp/usr/servers/defaultServer/
ENV DEPLOYMENT_DIR ${CONFIG}dropins/

RUN curl -O -L https://public.dhe.ibm.com/ibmdl/export/pub/software/openliberty/runtime/nightly/${RELEASE}/openliberty-all-${VERSION}.zip && \
    unzip openliberty-all-${VERSION}.zip -d ${INSTALL_DIR} && \
    rm openliberty-all-${VERSION}.zip
EXPOSE 9080 9443
ENTRYPOINT /opt/wlp/bin/server run defaultServer
