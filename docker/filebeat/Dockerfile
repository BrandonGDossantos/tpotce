FROM docker.elastic.co/beats/filebeat:6.4.2

# Include dist
ADD dist/ /root/dist/

USER root
RUN cp /root/dist/filebeat.yml /usr/share/filebeat/filebeat.yml&& \
    chown root:filebeat /usr/share/filebeat/filebeat.yml
USER filebeat