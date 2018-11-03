FROM docker.elastic.co/beats/filebeat:6.4.2

USER root
COPY dist/filebeat.yml /usr/share/filebeat/filebeat.yml
RUN chmod a-w /usr/share/filebeat/filebeat.yml

WORKDIR /usr/share/filebeat
USER filebeat
CMD ["filebeat", "-e", "-c", "filebeat.yml"]
