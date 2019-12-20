FROM fabric8/java-alpine-openjdk8-jre
RUN apk update && \
    apk upgrade && \
    apk add ffmpeg && \
# clean apk cache
    rm -rf /var/cache/apk/* && \
    rm -rf *.apk

CMD ["/sbin/init"]
