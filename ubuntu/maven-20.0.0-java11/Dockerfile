FROM tperdriau/ubuntu-graalvm:maven-20.0.0-java11
USER root
RUN apt-get -q update

RUN apt-get -q install ffmpeg -y

# Clean
RUN apt-get -q clean
RUN apt-get -q autoclean
RUN apt-get -q autoremove

USER 1001
WORKDIR /project

CMD mvn
