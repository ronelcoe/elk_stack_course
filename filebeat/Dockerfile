FROM docker.elastic.co/beats/filebeat:7.13.2
COPY filebeat.yml /usr/share/filebeat/filebeat.yml
USER root
RUN chmod go-w /usr/share/filebeat/filebeat.yml \
&& chown root:filebeat /usr/share/filebeat/filebeat.yml \
&& mkdir -p /data/elk/filebeat/config \
&& chown -R root:filebeat /data/elk/filebeat
USER filebeat