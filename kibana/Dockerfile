FROM nginx

ENV KIBANA_VERSION 4.0.1
ADD https://download.elasticsearch.org/kibana/kibana/kibana-$KIBANA_VERSION-linux-x64.tar.gz /tmp/kibana.tar.gz
RUN tar xzf /tmp/kibana.tar.gz -C /tmp
RUN mv /tmp/kibana-$KIBANA_VERSION-linux-x64 /opt/kibana

EXPOSE 5601

CMD /opt/kibana/bin/kibana
