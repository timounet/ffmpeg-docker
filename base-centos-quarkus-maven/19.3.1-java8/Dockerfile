FROM quay.io/quarkus/centos-quarkus-maven:19.3.1-java8
USER root
# RUN yum update -y && yum upgrade -y
RUN yum -y install epel-release
RUN rpm -Uvh http://li.nux.ro/download/nux/dextop/el7/x86_64/nux-dextop-release-0-5.el7.nux.noarch.rpm
RUN yum install ffmpeg ffmpeg-devel -y
RUN ffmpeg -version
# clean  cache
RUN yum clean packages -y
RUN yum clean headers -y
RUN yum clean metadata -y
RUN yum clean all -y
USER 1001
CMD ["/sbin/init"]
