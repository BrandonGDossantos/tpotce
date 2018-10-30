FROM prima/filebeat:6

COPY dist/filebeat.yml /filebeat.yml
USER root
RUN chown root:filebeat /filebeat.yml
USER filebeat