FROM docker.elastic.co/beats/filebeat:6.4.2

USER root
COPY dist/filebeat.yml /usr/share/filebeat/filebeat.yml
RUN chmod a-w /usr/share/filebeat/filebeat.yml

# Start cowrie
WORKDIR /usr/share/filebeat
USER filebeat
CMD ["/usr/local/bin/filebeat", "-e", "-c", "/usr/share/filebeat/filebeat.yml"]
