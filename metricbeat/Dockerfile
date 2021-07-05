FROM docker.elastic.co/beats/metricbeat:7.13.2
COPY metricbeat.yml /usr/share/metricbeat/metricbeat.yml
USER root
RUN chmod go-w /usr/share/metricbeat/metricbeat.yml \
&& chown root:metricbeat /usr/share/metricbeat/metricbeat.yml \
&& mkdir -p /data/elk/metricbeat/modules.d \
&& chown -R root:metricbeat /data/elk/metricbeat
USER metricbeat