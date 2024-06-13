FROM docker.elastic.co/beats/filebeat:8.13.4
USER root

COPY logs/ /usr/share/filebeat/logs/
COPY --chown=root:filebeat filebeat.yml /usr/share/filebeat/filebeat.yml

RUN chmod go-w /usr/share/filebeat/filebeat.yml