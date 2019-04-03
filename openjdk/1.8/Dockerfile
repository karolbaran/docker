FROM centos:7
MAINTAINER Karol Baran
RUN yum update -y && \
    mkdir -p /usr/lib/jvm/ && \
    yum -y install unzip && \
    curl -O -L https://download.java.net/openjdk/jdk8u40/ri/jdk_ri-8u40-b25-linux-x64-10_feb_2015.tar.gz && \
    tar xvf jdk_ri-8u40-b25-linux-x64-10_feb_2015.tar.gz -C /usr/lib/jvm && \
    yum clean all && \
    rm jdk_ri-8u40-b25-linux-x64-10_feb_2015.tar.gz && \
    rm -rf /var/cache/yum
ENV JAVA_HOME /usr/lib/jvm/java-se-8u40-ri
ENV PATH "$PATH":/${JAVA_HOME}/bin:.: