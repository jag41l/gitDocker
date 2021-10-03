FROM ubuntu
RUN apt update && \
    apt-get  install -y openjdk-11-jdk && \
    apt-get purge --auto-remove && \
    apt-get clean && \
    mkdir ajedrez
COPY serverajedrez.jar /ajedrez
COPY ./www /ajedrez/www
WORKDIR /ajedrez

CMD /bin/java -jar serverajedrez.jar
EXPOSE 7777 80
