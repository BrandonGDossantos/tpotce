FROM docker.elastic.co/beats/filebeat:6.4.2

USER root

COPY ./dist/filebeat.yml /opt/filebeat.yml

RUN cp /opt/filebeat.yml /usr/share/filebeat/filebeat.yml && \
    chown root:filebeat /usr/share/filebeat/filebeat.yml
