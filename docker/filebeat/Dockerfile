FROM docker.elastic.co/beats/filebeat:6.4.2

USER root
# Include dist
ADD dist/ /opt/dist/

USER filebeat
RUN cp /opt/dist/filebeat.yml /usr/share/filebeat/filebeat.yml&& \
    chown root:filebeat /usr/share/filebeat/filebeat.yml
