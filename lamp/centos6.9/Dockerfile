FROM centos:6.9

RUN yum -y update && yum -y install wget \
    && cd ~ && wget http://dl.wdlinux.cn:5180/lanmp_laster.tar.gz \
    && mkdir lanmp_laster && cd lanmp_laster \
    && tar -zxf ../lanmp_laster.tar.gz \
    && echo 1 | sh *.sh \
    && cd ~ && rm -rf lanmp_laster*

COPY startservices /usr/local/bin/

EXPOSE 80 8080

ENTRYPOINT ["startservices"]

CMD ["/bin/bash"]
