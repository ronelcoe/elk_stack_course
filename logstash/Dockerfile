FROM docker.elastic.co/logstash/logstash:7.10.2
WORKDIR /data/elk
COPY pipelines.yml /usr/share/logstash/pipelines.yml
COPY logstash.yml /usr/share/logstash/logstash.yml

USER root
RUN chmod go-w /usr/share/logstash/logstash.yml \
&& mkdir -p /data/elk/logstash/pipeline \
&& chown -R root:logstash /data/elk/logstash/

USER logstash