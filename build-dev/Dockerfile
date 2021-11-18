FROM python:3.6
LABEL maintainer 'Nikita Klementiev'

RUN useradd www && \
    mkdir /app && \
    mkdir /log && \
    chown www /log

USER www
VOLUME /log
WORKDIR /app
EXPOSE 8080

ENTRYPOINT ["/usr/local/bin/python"]
CMD ["run.py"]
